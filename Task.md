# First testing technique: Browser

## Conclusion
I created couple accounts to test functionality. Interesting found in this step was account age had to be 15, if wanted to make reservations.
That is the particular reason for many accounts. Result is that both reserver and admin can access resources and reservations. Tried to login from else where gets: Invalid CSRF Token. No matter, what account I tried.


#### Reserver 1 Account:
Email: quest1@gmail.com
Password: quest123

#### Reserver 2 Account:
Email: realquest@gmail.com
Password: quest123

#### Admin 1 Account:
Email: admin@gmail.com
Password: admin123

#### Admin 2 Account (wrongly chose admin using quest in email):
Email: quest2@gmail.com
Password: quest123

## Table
| **Page / Feature** | **Role** | **Success / Fail** | **Reason of Fail** |
|:----|:----:|:----:|:----:|
| /resources    | Reserver 1 | ✅| - |
| /reservation   | Reserver 1 | ❌ | User must be over 15 years old to make a reservation |
| /resources    | Reserver 2 | ✅| - |
| /reservation   | Reserver 2 | ✅ | - |
| /resources    | Admin 1| ✅| - |
| /reservation   | Admin 1 | ❌ | User must be over 15 years old to make a reservation |
| /resources    | Admin 2 | ✅| - |
| /reservation   | Admin2 | ✅ | - |


# Second testing technique: ZAP

## Conclusion
Found some new pages using manual scan and spider like seen picture under. Also made couple reports, but include only best one.
Pages listed to new list below. Most interesting find was /api/reservations did not work, but if I put /api/reservations/5, then it returns reservation of that id. Turns out 0 to 2 is empty, but starts from id 3. Report contains total of 4 alerts. One is authentication alert, that is made by account I used so it's nothing. Second is session alert, that is accessable by putting /api/session.



## Alerts
- No Anti CSRF Tokens
- Authentication Request Identified
- Session Management Response Identified
- User Agent Fuzzer

![image](https://github.com/user-attachments/assets/b654b201-246a-4f5a-8ac8-d781c3f7b083)

| **Page / Feature** | **Role** | **Success / Fail** | **Reason of Fail / Outcome** |
|:----|:----:|:----:|:----:|
| /api/resources    | Admin | ✅ | Lists every existing resource with ID, name and description. |
| /api/resources/id    | Admin | ✅ | Return corresponding resource. |
| /api/reservations    | Admin | ❌ | Return not, so it does not print every reservation. |
| /api/reservations/id    | Admin | ✅ | 3 and above returns id, token, resource_id, start time and end time. |
| /api/session   | Admin | ✅ | Returns account and role. |
| /api/resources    | Reverver | ✅ | Same as Admin |
| /api/resources/id    | Reserver | ✅ | Same as Admin |
| /api/reservations    | Reserver | ❌ | Same as Admin |
| /api/reservations/id    | Reserver | ✅ | Same as Admin |
| /api/session   | Reserver | ✅ | Same as Admin |
| /api/resources    | Quest | ✅ | Same as Admin |
| /api/resources/id    | Quest | ❌ | Unauthorized |
| /api/reservations    | Quest | ❌ | Same as Admin |
| /api/reservations/id    | Quest | ✅ | Same as Admin |
| /api/session   | Quest | ❌ | Unauthorized |

# Third testing technique: wfuzz and http

### What kind of pages can be found using common words?
wfuzz -c -w /usr/share/wordlists/dirb/common.txt --hc 404 http://localhost:8000/FUZZ

![image](https://github.com/user-attachments/assets/33a421fe-0b7d-4717-8246-7064c1d00c2e)

It got most pages.

### Is there an API folder and pages under it?
wfuzz -c -w /usr/share/wordlists/dirb/common.txt --hc 404 http://localhost:8000/api/FUZZ

![image](https://github.com/user-attachments/assets/440b6b0e-347d-4ea3-94b3-c4f07f29d689)

Interestingly it does not see, that session is under api. Picture below shows it is under api, but could be that it is not authorized to access it, what is the reason for 401.

![image](https://github.com/user-attachments/assets/dad6c91d-105d-491c-9b7f-8db573118580)


### Are there any pages in the reservations folder whose name is a number between 1-1000?
wfuzz -c -z range,1-1000 --hc 404 http://localhost:8000/api/reservations/FUZZ
![image](https://github.com/user-attachments/assets/032b3ede-48ab-46e7-b74f-d4e51f30f973)

This actually explains why i dont get anything using 0 to 2, but 3 and above.

### When the page is found, then what the page contains?
http http://localhost:8000/api/reservations/1  
![image](https://github.com/user-attachments/assets/1ceb2575-72f8-4791-86ca-becdedd82113)

Yes as expected it does not return it, but I tried to put 3 and it returns the reservation.

http http://localhost:8000/api/reservations/3  
![image](https://github.com/user-attachments/assets/d2c294d4-f18d-44aa-8da8-f899b342eecd)

# The final step of the test

QUEST IS MISSING FROM FIRST STEP PAGES

✔️ List of available pages ✔️
| **Page / Feature** | **Working Roles** |
|:----|:----:|
| / (index)    | Quest, Reserver, Admin |
| /login    | Quest, Reserver, Admin |
| /register    | Quest, Reserver, Admin |
| /resources    | Reserver, Admin |
| /reservation   | Reserver, Admin |
| /api/resources  | Quest, Reserver, Admin |
| /api/resources/id  | Reserver, Admin |
| /api/reservations | - |
| /api/reservations/id  | Quest, Reserver, Admin |
| /api/session | Reserver, Admin |


✔️ Following an iterative approach repeat browser testing.

2. If something needs to be changed in the table, change it.


