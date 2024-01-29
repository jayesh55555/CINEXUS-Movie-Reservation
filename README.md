# COSMOS APP 

## Tech stack
Android, Kotlin, Django, AWS-EC2, AWS-RDS(MySQL), Angular

## Design Choices:

### Application Components:
- Frontend: Native Android app for members, an Angular app for theater employees, ensuring a tailored experience for each user.
- Backend: Django for the main backend, providing a robust and scalable framework.
- Database: AWS RDS MySQL for data storage, which is a reliable choice with the ability to scale.
- Cloud Hosting: AWS EC2 instances with Auto Scaling and Load Balancer, ensuring high availability and scalability.

### User Roles:
- Members: Regular and Premium membership options with distinct features, encouraging user engagement.
- Theater Employees (Admins): Angular app for specialized tasks like managing movie schedules, theaters, and viewing analytics.
- All Users: Access to common functionalities like viewing the home page, membership options, and registration.

### APIs:
- Input/Output: JSON format for APIs ensures consistency and ease of parsing, promoting interoperability.
- Error Handling and Validation: Inclusion of error handling and input validation in APIs enhances the application's robustness.

### UI Functionality:
- Web/Mobile UI: Considering both web and mobile interfaces ensures a broad user base.
- Role-Based Access: APIs and UI functionalities are role-specific, maintaining security and providing a tailored experience.

### Functionality:
- Booking Tickets: Including an online service fee adds a revenue stream.
- Membership Features: Regular and Premium membership options with associated perks and fees.
- Rewards System: Encourages user loyalty through points accumulation.
- Cancellation and Refund: Provides flexibility for users.
- Employee Features: Analytics dashboard, scheduling, and configuration options for admins.

### Infrastructure:
- Cloud Deployment: AWS services (EC2, RDS) offer scalability, reliability, and easy management.
- Auto Scaled EC2 Cluster: Ensures resource efficiency and high availability.
- Load Balancer: Distributes traffic evenly, preventing overload on individual instances.

### Mock Data:
- Database with Mock Data: Allows testing and development without affecting the production environment.

### Technology Stack:
- Kotlin, Django, Angular: A diverse but well-integrated stack, covering both mobile and web development needs.

### Additional Considerations:
- Location-Based Functionality: Allowing users to select locations for viewing schedules aligns with a multi-location membership model.
- Discount Configuration: Offering flexibility with discount prices for specific showtimes contributes to business strategy.

## XP Core Values Maintained by Team

### Communication <br>

- **Team Collaboration:** <br>

    - Intra-Team Communication: Regular team meetings, whether virtual or in-person, facilitated open communication channels. This allowed team members to discuss progress, challenges, and ideas freely.
    - Cross-Functional Collaboration: As your project involved different technologies (Kotlin for Android, Django for the backend, Angular for the employee section), effective communication was crucial to ensure smooth integration and alignment between different components.
    - Clear Documentation: Thorough documentation of APIs, database schemas, and other project components was crucial for effective communication. This made it easier for team members to understand and work on different aspects of the project.

### Feedback <br>

- **Iterative Development:**

    - Continuous Feedback Loops: Regular iterations and demonstrations of features allowed stakeholders, including the client, to provide feedback early in the development process. This iterative approach ensured that the project aligned closely with the client's expectations.

- **Code Reviews:**

    - Peer Code Reviews: Implementing a process of peer code reviews allowed team members to share knowledge, identify potential issues, and maintain code quality. This feedback loop was instrumental in catching and addressing issues early on.

- **User Testing:**

    - User Feedback Sessions: If applicable, conducting user testing sessions for the Android app and web interfaces provided valuable insights. Direct feedback from potential end-users helped refine the user experience and fix any usability issues.
    
- **Retrospectives:**

    - Regular Retrospectives: Holding retrospectives at the end of each iteration or milestone encouraged the team to reflect on what went well and what could be improved. This continuous improvement mindset allowed the team to adapt and enhance their processes.

## Architecture Diagram

<img width="1796" alt="Architecture" src="https://github.com/gopinathsjsu/team-project-cosmos/assets/144189794/61cad8e2-320e-4972-a4bc-95b7fd8ab02f">

## Usecase Diagram

<img width="1010" alt="Screenshot 2023-12-05 at 11 34 19 PM" src="https://github.com/gopinathsjsu/team-project-cosmos/assets/144189794/9f2ca739-501c-426b-91fe-42e9659441ec">

## Deployment Diagram

<img width="1466" alt="Screenshot 2023-12-05 at 8 39 16 PM" src="https://github.com/gopinathsjsu/team-project-cosmos/assets/144189794/3e4c44da-478f-4bb6-b1f4-f2896ed4a11a">

## Sequence Diagram

![Screenshot (64)](https://github.com/gopinathsjsu/team-project-cosmos/assets/144189794/7e64a6c1-39fe-491c-802d-b82e903e93d2)

# Feature set
1. **Home/Landing Page:**
   - Provides an overview of theaters, locations, current movie schedules, and upcoming movies. Serves as the entry point for users.

2. **Membership Options:**
   - Presents Regular and Premium membership options. Regular membership is free, while Premium membership requires an annual fee of $15.

3. **Registration/Signup Page:**
   - Allows users to sign up for the Movie Theater Club, providing necessary information and creating an account.

4. **View Movie Schedules:**
   - Displays the schedules for current movie showtimes, helping users plan their theater visits.

5. **Book Tickets:**
   - Enables users to book tickets for a movie show. Includes an online service fee of $1.50 per ticket.

6. **Membership Page (For Enrolled Members):**
   - Displays movie tickets purchased, rewards points accumulated, and a list of movies watched in the past 30 days.

7. **Book Multiple Seats:**
   - Allows enrolled members to book multiple seats (up to 8) for a movie show, using rewards points or a pre-selected payment method.

8. **Cancel Tickets and Request Refund:**
   - Permits users to cancel booked tickets before showtime and request a refund.

9. **Rewards Points System:**
   - Accumulates rewards points for all members at a rate of 1 point per dollar spent. Premium members enjoy the additional benefit of the online service fee being waived.

10. **Theater Employee Section:**
    - An Angular app for theater employees (admins) to add/update/remove movies, showtimes, theater assignments, configure seating capacity, and view analytics.

11. **Analytics Dashboard:**
    - Provides theater employees with a visual representation of theater occupancy over the last 30/60/90 days. Summarizes data by location and movies.

12. **Location Selection:**
    - Allows users to choose the location they want to view schedules for, catering to a multi-location membership model.

13. **Discount Price Configuration:**
    - Permits theater employees to configure discount prices for shows before 6 pm and for Tuesday shows, offering flexibility in pricing.

14. **Cloud Deployment:**
    - Deploys the backend API and database to AWS, specifically using EC2 instances in an Auto Scaled Cluster with a Load Balancer for scalability and reliability.

15. **Web/Mobile UI:**
    - Develops a user-friendly interface for both web and mobile platforms to interact with the deployed APIs, providing a seamless user experience.

16. **Database with Mock Data:**
    - Creates a database with mock data for theaters, locations, and schedules, facilitating testing and development without impacting the production environment.


## UI Wireframes
[Figama](https://www.figma.com/file/aRjAZoxh7Zjh6l7OtjiEeE/Cosmos-App?type=design&node-id=0%3A1&mode=design&t=mnQjoabuVsWQsD4U-1)

## Sprint BurnDown Chart
[Sprint BurnDown Chart](https://docs.google.com/spreadsheets/d/1ZcI8HAixcSnnApqxAlzSDZHEiYxEO6roEYlSWF8YDKY/edit?usp=sharing)

## Project Journal
[Project Journal](https://docs.google.com/document/d/1g-rJZOsTqr15Pmve6omwRd2_0GcZj05kWZLlc52w1Fs/edit?usp=sharing)
