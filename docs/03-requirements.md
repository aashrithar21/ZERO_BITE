# FoodRescue — Requirements Specification

## 1. Purpose
This document defines the functional and non-functional requirements for the FoodRescue web application.

## 2. Functional Requirements

| ID | Requirement |
|---|---|
| FR-01 | The system shall allow restaurants, NGOs, and administrators to log in using authorized accounts. |
| FR-02 | The system shall support user registration for restaurants and NGOs. |
| FR-03 | The system shall provide role-based access to application features. |
| FR-04 | Restaurants shall be able to create, view, edit, and cancel their own food listings. |
| FR-05 | Food listings shall include food type, quantity, preparation details, pickup location, pickup deadline, and handling notes. |
| FR-06 | NGOs shall be able to browse available food listings. |
| FR-07 | NGOs shall be able to filter food listings by food type and location. |
| FR-08 | NGOs shall be able to submit donation requests for available listings. |
| FR-09 | Restaurants shall be able to accept or reject donation requests. |
| FR-10 | The system shall record and display donation request statuses. |
| FR-11 | Authorized users shall be able to view pickup details and update pickup status. |
| FR-12 | Restaurants and NGOs shall be able to view their respective donation and request histories. |
| FR-13 | Administrators shall be able to view platform summary statistics. |
| FR-14 | Administrators shall be able to manage user accounts. |
| FR-15 | The system shall prevent requests for cancelled, expired, or unavailable listings. |

## 3. Non-Functional Requirements

- **Security:** Passwords must be stored using secure password hashing, and protected operations must enforce authentication and authorization.
- **Usability:** The interface must provide clear navigation, labels, and error messages.
- **Reliability:** The system must handle invalid input and failed operations without corrupting stored records.
- **Data Integrity:** Related listings, requests, and pickup records must remain consistent.
- **Maintainability:** Code should be organized into understandable frontend, backend, and database components.
- **Compatibility:** The interface should work on modern desktop browsers and adapt to smaller screens.
- **Performance:** Common actions should respond smoothly with the project's test dataset.
- **Food Safety:** The system must not present expired listings as available and must capture relevant handling and pickup information.

## 4. User Roles

### Restaurant
- Manage its account and profile.
- Create and manage food listings.
- Review donation requests.
- Coordinate pickups.
- View donation history.

### NGO
- Manage its account and profile.
- Browse and filter food listings.
- Submit donation requests.
- Coordinate collection.
- View request history.

### Administrator
- Manage user accounts.
- View platform statistics.
- Access administrative functions unavailable to ordinary users.

## 5. Validation Rules

- Required fields must not be empty.
- Quantity must be a valid positive value.
- Pickup deadlines must be valid and must not be in the past when a listing is created.
- Only the owner of a listing may edit or cancel it.
- Only authorized restaurant accounts may accept or reject requests for their listings.
- Only authorized users may update relevant pickup statuses.
- Expired, cancelled, or unavailable listings must not accept new requests.

## 6. Acceptance Criteria

The requirements will be considered satisfied when:

- Users can register and log in with the appropriate role.
- Restaurants can manage their own food listings.
- NGOs can find available food and submit requests.
- Restaurants can record request decisions.
- Pickup status can be tracked through collection.
- Users can view their relevant histories.
- Administrators can manage accounts and view statistics.
- Unauthorized actions and invalid submissions are rejected.
- The core workflows pass documented tests.

## 7. Technology Stack

- Frontend: HTML, CSS, JavaScript, Bootstrap
- Backend: Python Flask
- Database: MySQL
- Testing: Python unittest and documented manual tests
- Version control: Git and GitHub
