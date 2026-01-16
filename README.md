# Campus Issue Reporting and Tracking System

A full-stack Spring Boot application for students to report maintenance issues and staff to track/resolve them.

## Key Features
* **Role-Based Access:** Students (Report), Staff/Admin (Manage).
* **Authentication:** JWT-based login stored in HttpOnly cookies.
* **File Uploads:** Attach images to issue reports.
* **Email Notifications:** Automatic emails when issue status changes.
* **Pagination:** Server-side pagination for issue lists.

## Technical Stack
* **Backend:** Spring Boot, Spring Security, Spring Data JPA.
* **Frontend:** Thymeleaf, Bootstrap 5.
* **Database:** MySQL.
* **Beyond CRUD Features:** File Upload (Images) & Email Notifications (SMTP).

## Setup Instructions
1. **Database:** Create a MySQL database named `campus_issue_db`.
2. **Configuration:** Update `src/main/resources/application.properties` with your MySQL credentials and Gmail App Password.
3. **Run:** Execute `./mvnw spring-boot:run` or run `IssueTrackerApplication.java` from your IDE.
4. **Access:** Open `http://localhost:8080` in your browser.

## 📁 Project Structure
- `controller/`: REST and View controllers.
- `service/`: Business logic (File storage, Email, Issue logic).
- `repository/`: Data access layer.
- `entity/`: Database models.
- `security/`: JWT and Security configurations.