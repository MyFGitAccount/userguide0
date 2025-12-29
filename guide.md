# EFS Platform User Guide

**Educational Facilitation System**  
*Last updated: December 29, 2025*

Welcome to **EFS** — a student-centric platform designed to make university life easier with smart tools for timetable planning, group formation, questionnaire exchange, course materials, and more.

---

## Table of Contents

- [1. Introduction](#1-introduction)
- [2. Getting Started](#2-getting-started)
  - [2.1 Creating an Account](#21-creating-an-account)
  - [2.2 Logging In](#22-logging-in)
  - [2.3 Logging Out](#23-logging-out)
- [3. Dashboard](#3-dashboard)
- [4. Timetable Planner (Calendar)](#4-timetable-planner-calendar)
- [5. Study Group Formation](#5-study-group-formation)
- [6. Questionnaire Exchange](#6-questionnaire-exchange)
- [7. Learning Materials](#7-learning-materials)
- [8. Course Catalog](#8-course-catalog)
- [9. My Profile](#9-my-profile)
- [10. Admin Features](#10-admin-features)
  - [10.1 Admin Panel](#101-admin-panel)
  - [10.2 Course Editor](#102-course-editor)
- [Troubleshooting & Notes](#troubleshooting--notes)

---

## 1. Introduction

### What is EFS?

EFS is a comprehensive educational platform that helps students:

- Plan timetables without conflicts  
- Find study group members  
- Exchange questionnaire responses for credits  
- Access & share course materials  
- Browse and request new courses  
- Manage personal profile & academic info  

**Key Concepts**

| Concept          | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| **Credits**      | Currency of the platform. Earn 1 credit by filling questionnaires, spend 3 to post one |
| **Roles**        | Student (default) / Admin (extra privileges)                                |
| **Approval Flow**| New accounts & new course requests require admin approval                  |

---

## 2. Getting Started

### 2.1 Creating an Account

1. Go to **Register** (usually linked from login page)
2. Fill in:
   - Student ID (SID)
   - Email (student email)
   - Password (min. 6 characters)
   - **Student ID Card Photo** (clear image, max 5MB — **required**)
3. Submit → You'll see:  
   *"Account Request Submitted! Waiting for admin approval."*
4. Wait for email confirmation from admin

> **Tip**: Use a clear, well-lit photo of your student card — blurry images may be rejected.

### 2.2 Logging In

1. Go to **Login**
2. Enter:
   - Email
   - Student ID
   - Password
3. Click **Login**

Successful login → redirected to **Dashboard**

### 2.3 Logging Out

Click the **Logout** button in the top-right corner (next to your SID & credits).

---

## 3. Dashboard

Your personal homepage after login.

### What you'll see

- Welcome message with your SID
- Quick stats:
  - Your current **credits**
  - Total courses on platform
  - Your active group requests
  - Your questionnaires
- **Quick Actions** cards (shortcuts to main features)
- Recent activity feed
- **Admin only**: Pending approval alerts

---

## 4. Timetable Planner (Calendar)

**Path:** Sidebar → 📅 Timetable Planner

### Main features

- Select courses from available list
- Visual weekly timetable (color-coded blocks)
- **Automatic conflict detection** (shows overlapping courses + campuses)
- Statistics: total courses, conflicts, estimated credits
- **Save** your timetable
- **Export** as PNG image

> **Pro tip**: Check conflicts before saving — red warnings help you avoid timetable disasters!

---

## 5. Study Group Formation

**Path:** Sidebar → 👥 Group Formation

### How it works

1. **Create your request** (or edit existing one)
   - Major (required)
   - Description
   - Contact info (email required)
   - Desired groupmates
   - Optional: GPA, DSE score
2. **Browse** other students' requests
3. Use **search** (major/description)
4. Click **Contact** to send invitation message

---

## 6. Questionnaire Exchange

**Path:** Sidebar → 📝 Questionnaire Exchange

### Credit economy

- **Post** a questionnaire → costs **3 credits**
- **Fill** someone else's → earn **1 credit**

### Actions

- See your credits & stats
- Post new questionnaire (description + Google Form link)
- View your own questionnaires (progress, delete)
- Browse & fill others' questionnaires → earn credits

> Important: You must actually fill the form before claiming the credit!

---

## 7. Learning Materials

**Path:** Sidebar → 📚 Learning Materials

### Workflow

1. Select course from dropdown
2. View list of materials (name, size, downloads, description)
3. **Download** files
4. **Admins only**: Upload new materials

---

## 8. Course Catalog

**Path:** Sidebar → 🎓 Course Catalog

### Features

- Search by code or title
- View detailed course info:
  - Description
  - Timetable table
  - Available materials (with download)
- **Request new course** (code + title) → waits for admin approval
- Quick button: **Add to Timetable**

---

## 9. My Profile

**Path:** Sidebar → 👤 My Profile

### You can update:

- Contact: email, phone
- Academic: major, year of study, GPA, DSE score
- Skills (comma separated)
- About me text

Photo change is supported but currently limited in UI.

---

## 10. Admin Features

### 10.1 Admin Panel

**Path:** Sidebar → ⚙️ Admin Panel

Tabs:
- **Pending Accounts** — approve/reject new users (+ see student card)
- **Pending Courses** — approve/reject new course requests
- **All Users** — manage credits, delete users
- **Statistics** — overview of platform usage

### 10.2 Course Editor

**Path:** /course-editor (may be linked from admin panel)

- Select existing course
- Edit basic info (code, title, description)
- Manage timetable sessions (add/remove)
- Save changes

---

## Troubleshooting & Notes

| Problem                                | Possible Solution                                      |
|----------------------------------------|--------------------------------------------------------|
| Can't login                            | Account still pending approval? Check email.           |
| Photo upload fails                     | File > 5MB or not an image? Try smaller/clearer photo  |
| No courses/materials appear            | New platform? Wait for admin to add content            |
| Questionnaire credit not awarded       | Make sure you actually filled the form                 |
| Want a new course                      | Use Course Catalog → Request new course                |

Questions? Contact your university admin or platform maintainer.

---

**Happy studying with EFS!** 🚀

Made with ❤️ by [Your Name / Team]  
Repository: https://github.com/[your-username]/efs-platform  
