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

e8f96fa7-38e3-4ce3-9e8b-af5cbded9cal
POST: register(birthdate,csrf_token,password,role,username)


Check what kind of alerts are found in the version.
Note

Do a broader test because there are now more pages. Make sure all pages are tested. Check lecture recording

Save the ZAP report in markdown format.
Fill in the table as the testing progresses.
The test can find new pages, for example

| **Page / Feature** | **Guest** | **Reserver** | **Administrator** |
|:----|:----:|:----:|:----:|
| `/` (index)                | | | |
| └─ View resource form      | ❌ | ✅ | ✅ note added |
| └─ Create new resource     | ❌ *1 | ❌ *2 | ✅ *3 |

# Tips
## 🧩 1. Web Page Structure

A web application is typically divided into **URLs** (routes) and **HTTP methods** that define how users interact with the application.

### Common structure:
- **Public pages** (accessible without login)
  - `/`
  - `/login`
  - `/register`
- **Protected pages** (require authentication)
  - `/resources`
  - `/reservation`
  - `/profile`
- **Admin/privileged pages**
  - `/admin/users`
  - `/admin/settings`

---

## 🛠 2. Typical Functionalities to Test

| **Type**              | **Examples**                                 |
|-----------------------|----------------------------------------------|
| View content          | Dashboard, listings, read-only pages         |
| Form submissions      | Login, registration, create/edit resources   |
| Data modification     | Edit profiles, create reservations, delete   |
| Privileged actions    | User management, access control, settings    |
| API calls             | `/api/*` endpoints for frontend/backend      |

---

## 🔐 3. What to Focus on in Authorization Testing

### ✅ **Access Control Rules**
- Can **unauthenticated users** (Guests) access protected pages?
- Can **Reserver** role access Admin-only functions?
- Are **API endpoints** enforcing role-based restrictions?

### ✅ **Horizontal Privilege Escalation**
- Can user A access or modify data of user B?
  - e.g., `/api/reservations/1` or `/profile?id=5`

### ✅ **Vertical Privilege Escalation**
- Can a low-privilege user (e.g., Reserver) perform Admin actions?
  - Submit forms to `/admin` routes
  - Modify user roles via hidden parameters

---

## 🔍 4. Testing Approach

1. **Map pages & APIs**
   - Use tools like **wfuzz**, **ffuf**, or **dirb** to discover hidden paths.
   - Map both **GET** and **POST** endpoints.

2. **Test as different roles**
   - Guest (unauthenticated)
   - Authenticated user (e.g., Reserver)
   - Administrator

3. **Inspect functions on each page**
   - Buttons, forms, APIs, links
   - Backend-side restrictions (not just hidden in UI)

---

## 🎯 5. Goal of Authorization Testing

- Ensure **least privilege** principle (users can only do what they should).
- Detect **bypass vectors** (direct object references, hidden APIs).
- Confirm both **frontend** and **backend** enforce authorization properly.

---

> Tip: Combine **manual testing** and **automated fuzzing** for maximum coverage!
