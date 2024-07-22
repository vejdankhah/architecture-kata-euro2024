# Architecture Kata: Euro 2024 Ticketing System
## Problem Statement
UEFA Euro 2024 is a major international football tournament that requires a robust and scalable ticketing system. The system must handle the end-to-end process of ticket sales, from initial registration and application to payment and delivery. It must support millions of users, ensure security and fairness, and provide a seamless user experience across various platforms.

### Objective
Design high-level architecture for a ticketing system for UEFA Euro 2024 that meets the requirements

### High-level requirements

#### 1. User Registration and Authentication
* Users must be able to self-register, authenticate, and manage their profiles.
* Support for social media login (e.g., Facebook, Google) and two-factor authentication.

#### 2. Ticket Application and Purchase
It should happen in 2 phases.

##### Phase 1: A lottery system for matches to ensure fairness
* The users must be able to request tickets during specific application windows.
* The users must chose fixture, and ticket category, and number of tickets.
* The users can chose to accept ticket in different category than the one requested.
* There are limitations of number of tickets that each user can request (each person 5 tickets).
* After closing the phase 1 ticket requests, the systme must perform a lottery draw, to assign the 60% of available tickets to the users.
* The users who win the lottery will be informed by system.
* The users have a limited time (couple of days only) to pay for their tickets. - Multiple payment options (credit card, PayPal, bank transfer).

##### Phase 2: First come, first serve sales
* Users can apply for tickets during specific application windows.
* Real-time availability updates and seat selection.
* The users have to pay for their tickets within a short period of time of ticket selection (minutes) to ensure fairness. - Multiple payment options (credit card, PayPal, bank transfer).

#### 3. Ticket Management, back-office
* adding fixtures
* adding stadiums details
* ticket details, categories and pricing

#### 4. Ticket delivery
* UEFA administrators will review and approve ticket assignments.
* Digital ticket delivery via mobile app and email.
* Integration with access control systems at venues.

#### 5. Ticket Managemetn, users
* Users can view, transfer, and resell their tickets.

### Non-functional requirements

#### Scalability and Performance
* Must be able to handle unexpected spikes in traffic.
* Handle millions of concurrent users during peak times.
* High availability and fault tolerance.
* Efficient load balancing and resource management.

#### Security
* Protect user data and payment information.
* Prevent fraud and unauthorized access.
* Ensure compliance with legal and regulatory requirements (e.g. Compliance with GDPR and other relevant regulations).

#### User Interface
* Responsive web application and mobile apps (iOS, Android).
* User-friendly design.

#### Payment Gateway integration
* Secure and reliable payment processing.
* Support for multiple currencies.

#### Notification System
* Email and SMS notifications for important updates (e.g. ticket confirmation, event reminders).

#### Analytics and Reporting
* Real-time dashboards for monitoring system performance and sales.
* Detailed reports for event organizers and stakeholders (e.g. sales report, unsold tickets, loss report, ...).

## Deliverables
* User journeys for the main stories
* Architecture Characteristics
* C1
* C2
* C3 (for complex containers)
* ADRs for any decision