| **Page / Feature** | **Guest** | **Reserver** | **Administrator** |
|:----|:----:|:----:|:----:|
| `/` (index)                | | | |
| └─ View resource form      | ❌ | ✅ | ✅ note added |
| └─ Create new resource     | ❌ *1 | ❌ *2 | ✅ *3 |


Tasks in order:
# 2. Create a new page on Github (markdown) and add the following table to the page
# 3. First testing technique: Browser

Familiarize yourself with the functionality of the version as comprehensively as possible.
create users with different roles
make reserveable resources
make reservations
...
Fill in the table as the testing progresses.

Quest 1:
Account: quest1@gmail.com
Password: quest123

| **Page / Feature** | **Guest** | **Reserver** | **Administrator** |
|:----|:----:|:----:|:----:|
| `/` (index)                | | | |
| └─ View resource form      | ❌ | ✅ | ✅ note added |
| └─ Create new resource     | ❌ *1 | ❌ *2 | ✅ *3 |

# 4. Second testing technique: ZAP

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
