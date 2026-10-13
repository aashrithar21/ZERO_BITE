# FoodRescue — Project Scope

## 1. Purpose
This document defines the features, boundaries, and limitations of the FoodRescue web application.

## 2. In Scope

The first version of FoodRescue will include:

1. **User Registration and Login:** Separate accounts and role-based access for restaurants, NGOs, and administrators.
2. **Restaurant Food Listings:** Restaurants can create, view, edit, and cancel surplus-food listings.
3. **Browse Available Food:** NGOs can view and filter available food donations.
4. **Donation Requests:** NGOs can request donations, and restaurants can accept or reject requests.
5. **Pickup Coordination:** Users can view pickup details and track collection status.
6. **Donation History:** Restaurants and NGOs can view their relevant donation and request records.
7. **Admin Dashboard:** Administrators can manage user accounts and view basic platform statistics.

## 3. Out of Scope

The initial version will not include:

- Online payments.
- A separate delivery-partner or volunteer role.
- Live GPS tracking or route optimization.
- Dedicated Android or iOS applications.
- AI-based food-demand prediction.
- Automated SMS or WhatsApp notifications.

These features may be considered for future enhancements.

## 4. Target Users

- **Restaurants:** Publish and manage surplus-food listings.
- **NGOs:** Find food donations and request collection.
- **Administrators:** Manage user accounts and monitor platform activity.

## 5. Technology Boundaries

- Frontend: HTML, CSS, JavaScript, Bootstrap
- Backend: Python Flask
- Database: MySQL
- Version control: Git and GitHub

## 6. Assumptions and Limitations

- Restaurants and NGOs provide accurate information.
- Restaurants and NGOs coordinate the actual food collection.
- The platform records donation details but does not transport food.
- Food listings must include appropriate pickup deadlines and handling information.
- The project is developed as an academic mini-project and is not intended to guarantee food safety or replace applicable regulations.

## 7. Completion Criteria

The MVP will be considered complete when the seven in-scope features work together, core workflows pass documented tests, and the team can demonstrate a donation from listing creation through collection and history recording.
