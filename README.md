# 🎓 Online Course Platform - Data Modeling Project

This project presents a **data model** for an Online Course Platform, focusing on building a strong database structure using **Entity-Relationship Diagram (ERD)** principles.

The platform allows students to enroll in courses, instructors to teach courses, and manage all the enrollment and payment activities in a structured way.

---

## 🗂 Project Structure

- **Students**: Information about students registered on the platform.
- **Courses**: Details of available courses.
- **Instructors**: Profiles of instructors who teach courses.
- **Enrollments**: Students enrolling in various courses.
- **Payments**: Payment records for enrolled courses.
- **Course_Instructors**: Linking multiple instructors to multiple courses (Many-to-Many relationship).

---

## 🖼 Entity-Relationship Diagram (ERD)

![ERD]([Online%20Course%20Platform.png](https://lucid.app/lucidchart/dd92bbb5-0420-4561-9269-8845a4b345be/edit?viewport_loc=-1035%2C-64%2C3921%2C1415%2C0_0&invitationId=inv_285be412-2508-4c2e-99ca-5244cbf64b62))

---

## 📑 Table Descriptions

### 1. Students
- **student_id (PK)**
- first_name
- last_name
- email
- phone
- registration_date

### 2. Courses
- **course_id (PK)**
- course_name
- description
- price
- created_date

### 3. Instructors
- **instructor_id (PK)**
- first_name
- last_name
- email

### 4. Enrollments
- **enrollment_id (PK)**
- student_id (FK)
- course_id (FK)
- enrollment_date
- status

### 5. Course_Instructors
- **id (PK)**
- course_id (FK)
- instructor_id (FK)

### 6. Payments
- **payment_id (PK)**
- student_id (FK)
- course_id (FK)
- amount
- payment_method
- payment_date

---

## 🔗 Relationships

- A **Student** can enroll in multiple **Courses**.
- A **Course** can have multiple **Students** enrolled.
- A **Course** can be taught by multiple **Instructors**.
- An **Instructor** can teach multiple **Courses**.
- Each **Payment** is linked to a specific **Student** and **Course**.

---

## 🛠 Tools Used

- **Lucidchart**: For designing the ERD diagram
- **Markdown**: Documentation
- **GitHub**: Version Control and Repository

---

## 🚀 Future Enhancements

- Add lookup tables (e.g., payment methods, enrollment status types).
- Implement the data model in a relational database (e.g., MySQL, PostgreSQL).
- Create sample SQL scripts for database creation.


