# ZERO_BITE


# 🍱 FoodRescue – Food Wastage Reduction and Donation Platform

## 1. Project Description

FoodRescue is a web-based platform designed to reduce food wastage by connecting restaurants that have surplus food with NGOs that can collect and distribute it to people in need.

Restaurants can post details about available surplus food, while NGOs can browse donations, request food, and coordinate pickup. The platform aims to reduce food wastage and make food donation easier, faster, and more organized.

**Project Type:** Software Engineering Mini Project  
**Case Study:** Case 31 – Food Wastage Reduction App  
**Development Methodology:** Agile using Scrum

## 2. Problem Statement

Restaurants and hotels often have surplus food that may go to waste, while NGOs and charitable organizations need food to support people in need. A lack of communication and coordination between food providers and NGOs makes it difficult to distribute surplus food efficiently.

FoodRescue aims to solve this problem by providing a common platform where restaurants can list surplus food and NGOs can find, request, and collect suitable donations.

## 3. Objectives

- Reduce avoidable food wastage.
- Connect restaurants with NGOs through a common platform.
- Allow restaurants to post and manage food donations.
- Enable NGOs to search and request available food.
- Track donation requests and pickup status.
- Maintain records of donations and collections.
- Apply Agile and Scrum practices during development.
- Develop a user-friendly and reliable application.

## 4. Proposed Technology Stack

| Component | Technology |
|---|---|
| Frontend | HTML, CSS, JavaScript, Bootstrap |
| Backend | Python Flask |
| Database | MySQL |
| Version Control | Git and GitHub |
| Testing | Python unittest or pytest |

*Note: This is our proposed technology stack. Update it if the team selects different technologies.*

## 5. User Roles

### Restaurant
- Register and log in.
- Manage restaurant profile.
- Post surplus food details.
- Edit or cancel donation listings.
- View donation requests and their status.
- View previous donations.

### NGO
- Register and log in.
- Manage NGO profile.
- Browse available food donations.
- Search and filter donations.
- Request available food.
- Coordinate food pickup.
- View collection history.

### Administrator
- Monitor registered users.
- Monitor donation activities.
- Manage reported accounts or donation listings.
- View donation statistics and reports.

## 6. Application Workflow

The main workflow of FoodRescue is as follows:

1. **User Registration:** Restaurants and NGOs register on the platform.
2. **Login:** Registered users log in using their credentials.
3. **Food Donation Posting:** Restaurants provide food details such as food type, quantity, location, and pickup time.
4. **Data Validation:** The application validates the submitted information and stores the donation in the database.
5. **Donation Discovery:** NGOs browse available donations and search for suitable food.
6. **Donation Request:** An NGO submits a request for an available donation.
7. **Request Processing:** The restaurant reviews the request and accepts or declines it.
8. **Pickup Coordination:** The restaurant and NGO coordinate the pickup details.
9. **Status Update:** The donation status is updated as the process progresses.
10. **Completion:** After collection, the donation is marked as completed.
11. **History and Reports:** Donation records can be reviewed by authorized users and administrators.

### Workflow Diagram

```text
        START
          |
          v
  User Registration/Login
          |
          v
   Restaurant Posts Food
          |
          v
  Validate and Save Donation
          |
          v
  Donation Listed for NGOs
          |
          v
    NGO Views Donations
          |
          v
    NGO Requests Food
          |
          v
 Restaurant Reviews Request
          |
          v
   Request Accepted?
       /       \
     No         Yes
     |           |
     v           v
 Update/Close   Arrange Pickup
 Request            |
                    v
              Collect Food
                    |
                    v
           Mark as Completed
                    |
                    v
              Save History
                    |
                    v
                   END
```

## 7. Main Modules

1. **Authentication Module:** Handles registration, login, and logout.
2. **User Management Module:** Maintains restaurant and NGO profiles.
3. **Food Donation Module:** Allows restaurants to create, edit, and manage donation listings.
4. **Donation Discovery Module:** Allows NGOs to view and search available food.
5. **Request Management Module:** Handles donation requests and acceptance or rejection.
6. **Pickup Management Module:** Maintains pickup information and donation status.
7. **History Module:** Displays previous donations and collections.
8. **Admin Module:** Supports monitoring and reporting.
9. **Testing Module:** Verifies functionality, database operations, and system integration.

## 8. Agile Methodology – Scrum

FoodRescue will be developed using the Agile methodology with the Scrum framework. Development will be divided into short iterations called sprints.

Each sprint will focus on a specific set of features. The team will plan the sprint, develop and test the selected features, review the working increment, and identify improvements for the next sprint.

### Scrum Activities

- **Product Backlog:** A prioritized list of features and requirements.
- **Sprint Planning:** Selecting tasks for the upcoming sprint.
- **Sprint Backlog:** The tasks selected for the current sprint.
- **Development:** Designing, implementing, and testing features.
- **Sprint Review:** Demonstrating completed functionality.
- **Sprint Retrospective:** Discussing improvements to the team's process.
- **Increment:** The working functionality delivered at the end of a sprint.

## 9. Sprint Plan

| Sprint | Goal | Planned Features |
|---|---|---|
| Sprint 1 | Project foundation | Repository setup, database foundation, registration, login, basic UI |
| Sprint 2 | Food donation management | Create, edit, cancel, and display donations |
| Sprint 3 | Donation requests | NGO requests, restaurant responses, pickup coordination, status tracking |
| Sprint 4 | History and administration | Donation history, admin monitoring, reports, and notifications if time permits |
| Sprint 5 | Testing and release | Integration testing, bug fixes, UI improvements, and final demonstration |

The sprint plan may be adjusted based on team progress and feedback.

## 10. Team Members and Responsibilities

| Team Member | Role | Responsibilities |
|---|---|---|
| Aash | Scrum Master | Facilitate Scrum activities, coordinate the team, track sprint progress, and help remove blockers |
| Sujay | Database and Testing | Design the database, maintain data integrity, prepare test cases, and test application workflows |
| Koushik | Backend Developer | Implement backend logic, routes, authentication, and donation/request processing |
| Sahithi | Frontend Developer | Design pages, forms, dashboards, layouts, and frontend integration |

All members will collaborate during reviews, integration, testing, and the final project demonstration.

## 11. Database Overview

The proposed database may contain the following tables:

- **Users:** User ID, name, email, password hash, role, and contact details.
- **Restaurant Profiles:** Restaurant ID, user ID, restaurant name, and location.
- **NGO Profiles:** NGO ID, user ID, organization name, and location.
- **Donations:** Donation ID, restaurant ID, food details, quantity, pickup time, location, and status.
- **Donation Requests:** Request ID, donation ID, NGO ID, request time, and request status.
- **Pickup Details:** Pickup ID, request ID, scheduled time, and pickup status.
- **Notifications:** Notification ID, recipient, message, and read status.

The final schema will be decided during database design. Sensitive information, including passwords, must be stored securely.

## 12. Testing Strategy

Testing will be performed throughout development.

- **Unit Testing:** Tests individual functions and validation rules.
- **Integration Testing:** Verifies interaction between the frontend, backend, and database.
- **Functional Testing:** Checks whether each feature behaves as expected.
- **Workflow Testing:** Tests the complete process from posting a donation to completing a pickup.
- **Validation Testing:** Checks missing, invalid, or inconsistent input.
- **Regression Testing:** Ensures existing features continue to work after changes.

Test cases and their results will be documented during development.

## 13. Expected Outcome

The expected outcome is a working web application that enables restaurants to publish surplus food and NGOs to discover, request, and collect suitable donations.

The project will also demonstrate software engineering concepts such as requirements analysis, modular design, database design, version control, testing, and Agile/Scrum project management.

Actual results and completed features will be documented after implementation and testing.

## 14. Future Enhancements

- Email or in-app notifications.
- Map-based donation discovery.
- Pickup-time reminders.
- Improved donation statistics and impact reports.
- Mobile application support.
- Advanced administrative analytics.

## 15. Git and GitHub Workflow

The team will use Git and GitHub for source code management and collaboration.

1. Create tasks from the Product Backlog.
2. Create a feature branch for each task.
3. Implement and test the feature.
4. Commit changes with clear messages.
5. Push the branch to GitHub.
6. Review and merge changes into the main branch.
7. Update the Scrum board and task status.

Example branch name:

```bash
feature/donation-listing
```

Example commit message:

```bash
git add .
git commit -m "Add food donation listing feature"
git push
```

## 16. Conclusion

FoodRescue aims to reduce avoidable food wastage by connecting restaurants with NGOs through an organized food donation platform. By using Agile/Scrum, the team can develop the application incrementally, test features regularly, and improve the system based on feedback.

The project combines practical software development with software engineering principles to create a solution that supports more efficient food donation and distribution.

---

**Project:** FoodRescue – Food Wastage Reduction and Donation Platform  
**Case Study:** 31  
**Methodology:** Agile with Scrum
