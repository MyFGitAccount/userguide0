# EFS Platform User Guide

Welcome to the EFS (Educational Facilitation System) Platform! This guide provides step-by-step instructions on how to use the platform's features. EFS is designed to enhance your learning experience by offering tools for timetable planning, group formation, questionnaire exchanges, access to learning materials, course browsing, and more.

This guide is structured by feature, starting from account creation and login. If you're an administrator, refer to the dedicated Admin Features section at the end.

---

## 1. Introduction

### What is EFS?
EFS is an educational platform for students and administrators. Key features include:
- **Timetable Planner**: Build and export your course schedule.
- **Group Formation**: Find study partners based on majors, GPA, and preferences.
- **Questionnaire Exchange**: Post and fill questionnaires to earn credits.
- **Learning Materials**: Access and upload course resources.
- **Course Catalog**: Browse courses, view details, and request new ones.
- **Dashboard**: Overview of your stats and quick actions.
- **Profile**: Manage personal information.
- **Admin Tools**: Approve accounts/courses, manage users, and edit courses (admin-only).

### Key Concepts
- **Credits**: Earned by filling questionnaires (1 credit each) or added by admins. Used to post questionnaires (3 credits each).
- **Roles**: Students (default) and Admins (with extra privileges).
- **Approvals**: New accounts and course requests require admin approval.

---

## 2. Getting Started

### 2.1 Creating an Account
1. Navigate to the registration page (usually `/register` or linked from the login page).
2. Fill in the form:
   - **Student ID (SID)**: Your unique student identifier (e.g., 12345678).
   - **Email**: Your student email (e.g., student@example.com).
   - **Password**: At least 6 characters. Confirm it in the next field.
   - **Student Card Photo**: Upload a clear image of your student ID card (max 5MB, required for verification).
3. Submit the form. You'll see a success message: "Account Request Submitted! Your account request has been sent for admin approval."
4. Wait for admin approval via email. Once approved, you can log in.

**Note**: If the photo is too large or invalid, you'll get an error. Accounts are pending until approved.

### 2.2 Logging In
1. Go to the login page (`/login`).
2. Enter your **Email**, **Student ID (SID)**, and **Password**.
3. Click "Login".
4. If successful, you'll be redirected to the Dashboard. Errors (e.g., invalid credentials) will display above the button.

**Forgot Password?** (Not implemented in the provided code—contact support if needed.)

### 2.3 Logging Out
From any page, click the "Logout" button in the top navigation bar (next to your SID and role).

---

## 3. Dashboard

The Dashboard is your home page after login (`/dashboard`).

### Features
- **Welcome Message**: Greets you by SID.
- **Stats Grid**:
  - Your Credits: Available balance.
  - Total Courses: Platform-wide courses.
  - Group Requests: Your active group formation requests.
  - Questionnaires: Your created questionnaires.
- **Quick Actions**: Links to key features (e.g., Timetable Planner, Group Formation). Icons and descriptions guide you.
- **Recent Activity**: Lists recent events (e.g., "Welcome to EFS Platform!").
- **Admin Alert** (Admins only): Shows pending approvals with a link to the Admin Panel.

**Tips**: If data fails to load, click "Retry". Use the sidebar menu to navigate.

---

## 4. Timetable Planner (Calendar)

Access via sidebar: "📅 Timetable Planner" (`/calendar`).

### Features
- **Course Selection**: Toggle courses from the list to add/remove from your timetable.
- **Timetable View**: Displays a weekly grid (Mon-Sat) with time slots. Selected courses appear as colored blocks with details (code, time, room).
- **Conflict Detection**: Highlights overlapping courses with details (e.g., day, time, campuses).
- **Stats**: Total courses, conflicts, and credits (assuming 3 per course).
- **Actions**:
  - Save Timetable: Saves to your account (login required).
  - Export as PNG: Downloads the timetable as an image.

**How to Use**:
1. Select courses from the sidebar list.
2. View the timetable and check for conflicts.
3. Save or export as needed.

**Note**: Courses are fetched from the platform. Conflicts consider weekday and time overlaps.

---

## 5. Group Formation

Access via sidebar: "👥 Group Formation" (`/group-formation`).

### Features
- **My Group Request**: View/edit/delete your request. Includes major, description, desired groupmates, GPA, etc.
- **Create/Edit Request**:
  - Fill form: Major (required), Description, Email (required), Phone, Desired Groupmates, GPA, DSE Score.
  - Submit to post or update.
- **Browse Requests**: Search by major/description. View others' requests with details.
- **Contact**: Send a message to invite someone (prompts for your message).

**How to Use**:
1. Create a request if none exists.
2. Search and browse others' requests.
3. Click "Contact" to send an invitation.

**Note**: Your own request can't be contacted. Deletions are permanent.

---

## 6. Questionnaire Exchange

Access via sidebar: "📝 Questionnaire Exchange" (`/questionnaire`).

### Features
- **Stats**: Your credits, available questionnaires to fill, your created ones.
- **Post Questionnaire** (Costs 3 credits):
  - Description (required), Google Form Link (required), Target Responses (default 30).
  - Submit if you have enough credits.
- **My Questionnaires**: List with responses, status (e.g., active), view link, and delete button.
- **Fill Questionnaires** (Earn 1 credit each):
  - Browse list with creator, responses, description, and link.
  - Open the link, fill it externally, then click "Fill & Earn 1 Credit".

**How to Use**:
1. Post a new one if needed (check credits).
2. Fill others' by opening the link and confirming.
3. Manage your own via the sidebar.

**Note**: You can't fill your own. Target responses track progress.

---

## 7. Learning Materials

Access via sidebar: "📚 Learning Materials" (`/materials`).

### Features
- **Select Course**: Dropdown to choose a course.
- **View Materials**: Grid of cards with name, description, size, downloads, uploaded by.
- **Download**: Click to download a file.
- **Upload** (Admins only): Choose file, name, description, and submit.

**How to Use**:
1. Select a course from the sidebar.
2. Browse materials.
3. Download as needed.
4. (Admins) Upload new ones via the form.

**Note**: No materials? It shows a message. Uploads are course-specific.

---

## 8. Course Catalog (Course Viewer)

Access via sidebar: "🎓 Course Catalog" (`/courses`).

### Features
- **Search Courses**: Filter by code/title.
- **Course List**: Click to view details.
- **Details View**: Description, timetable (table with day/time/room/class no), materials (list with download links).
- **Actions**: Add to Timetable (links to Calendar).
- **Request New Course**: Enter code and title, submit for admin approval.

**How to Use**:
1. Search or browse courses.
2. Click for details.
3. Request new ones if missing.

**Note**: Timetable and materials may be empty if not set.

---

## 9. Profile Management

Access via sidebar: "👤 My Profile" (`/profile`).

### Features
- **View Mode**: Shows photo, SID, email, role, credits, contact info, academic details (major, year, GPA, DSE), skills (tags), about me, account dates.
- **Edit Mode**: Update email, phone, major, GPA, DSE score, skills (comma-separated), year of study, about me.
- **Photo**: Upload/change (preview shown).

**How to Use**:
1. Click "Edit Profile" to enter edit mode.
2. Update fields and submit.
3. Cancel to revert.

**Note**: Some fields (e.g., SID) are read-only.

---

## 10. Admin Features

Access via sidebar: "⚙️ Admin Panel" (`/admin`) (Admins only).

### 10.1 Admin Panel
- **Tabs**: Accounts (pending), Courses (pending), Users (all), Stats.
- **Pending Accounts**: View SID, email, photo. Approve/Reject.
- **Pending Courses**: View code, title. Approve/Reject.
- **All Users**: Table with SID, email, role, credits, created date. Add credits or delete (except admins).
- **Stats**: Cards for total users, courses, pending items, materials.

**How to Use**: Switch tabs, perform actions (confirm prompts appear).

### 10.2 Course Editor
Access via sidebar (if available) or quick actions: `/course-editor`.

- **Course List**: Select a course.
- **View/Edit**: Toggle edit mode.
- **Edit Form**: Update code, title, description. Add/remove timetable sessions (day, time, room, class no).
- **Save**: Submits changes.

**How to Use**:
1. Select course.
2. Edit and add sessions.
3. Save.

**Note**: Access denied for non-admins.

---

## Troubleshooting
- **Errors**: Check console or retry fetches.
- **No Internet Features**: Some tools (e.g., external links) require browser permissions.
- **Contact Support**: For issues like forgotten passwords or bugs.

This guide is based on the EFS platform's frontend code. For backend details or updates, refer to the source repository. If you need expansions or screenshots, let us know!
