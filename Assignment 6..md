**Assignment 6**

STUDENT: THABANG MOTAMPANE

STUDENT NUMBER: 251699544

**Agile Planning Documentation:**

The aim of this project is to create an online platform where customers can easily search, book, and rent boats in the city of Cape Town. This project also aims to create an environment where the boat owner can list their boats, manage availability, and communicate with customers with the help of staff members (sales assistants). The platform finally aims to streamline the boat rental process, providing a user-friendly experience for both customers and the boat owner, while ensuring secure payments, clear communication, and comprehensive booking management.

The end goal of this project is to:

-   Make the process of searching, booking, and paying for boats as seamless as possible for customers.
-   Allow the owner to easily manage their boat listings, set availability, and monitor bookings.
-   Design a system that can scale to include different types of boats, services, and locations.
-   Provide a secure payment system and offer customer/boat owner feedback mechanisms to establish trust.

I will use Scrum to manage the project, using 2-week sprints, sprint reviews, and retrospectives to track progress and improve the process. Tasks will be completed in short, time-boxed sprints (2 weeks) with regular releases. The product owner will ensure the backlog is regularly updated, prioritized, and refined.

Each sprint will consist of daily stand-ups which are 15-minute meetings to discuss progress, obstacles, and upcoming tasks. At the end of each sprint, I will demonstrate completed work to stakeholders. After each sprint review, I will reflect on what went well, what can be improved, and how to improve processes.

The product will be released iteratively, with the first version containing core features such as boat search, listing, and booking functionalities. Further releases will add advanced features like feedback systems, notifications, and admin tools.

1\. **User Story Creation**: Below is a user story table for the Boat Rental System. The aim of the user story table is to break down the system's features into small, manageable parts that can be built in iterations.

| Story ID                         | User Story                                                                                                                                                                                                       | Acceptance                                                                                                                                                                                                                                                              | Priority |
|----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------|
| Register Account US- 001         | As a customer, I want to register for an account so that I can make bookings and track my booking history.                                                                                                       | The customer can view their account information and rental history. The customer can also make rental requests or bookings.                                                                                                                                             | High     |
| Browse Available Boats US- 002   | As a customer, I want to browse a list of available boats at my preferred location, So that I can see which boats are available for rent.                                                                        | The customer can view a list of available boats based on their search criteria (location, boat type, and availability). Each boat shows relevant information such as name, type, capacity, and price per hour.                                                          | High     |
| Make Booking US-003              | As a customer, I want to reserve a boat for a specific date and time, So that I can ensure the boat will be available when I need it.                                                                            | The customer can select a boat, choose the rental date and time, and proceed with booking. The system shows available boats for the selected time, and the reservation is successfully saved.                                                                           | High     |
| Cancel Booking. US-004           | As a customer, I want to cancel a booking, So that I can free up the boat for others if my plans change.                                                                                                         | The customer can cancel a booking before the scheduled start time. A confirmation message is displayed after cancellation. The boat's availability is updated in the system.                                                                                            | High     |
| Approve rental request. US-005   | As a systems administrator, I want to approve/decline customer rental requests or bookings , so that I can notify them if the requested boat if they meet the necessary requirements to rent the requested boat. | The systems admin receives the requests or bookings and able to approve or decline the requests. A confirmation message is then sent to the customer about the status of their request.                                                                                 | High     |
| Pay for Booking. US-006          | As a customer, I want to pay for my boat booking online, So that I can complete my booking process and secure the boat rental.                                                                                   | The customer can review the booking details before proceeding with payment. Payment methods include credit card, debit card, or online payment gateway. The system processes the payment securely and confirms the reservation.                                         | High     |
| Process Payment. US-007          | As a sales assistant, I want to process payments for customer bookings, So that customers can pay for their boat rentals and complete the booking.                                                               | The sales assistant can view payment details associated with bookings. The staff can mark a payment as completed after processing it. The system generates a receipt for the customer.                                                                                  | High     |
| Send Confirmation Email. US-008  | As the system, I want to send a confirmation email to customers after a successful booking, So that customers have a record of their booking and can prepare for the rental.                                     | The system sends a confirmation email containing booking details (boat type, date, time, payment). The email is sent automatically after the booking is completed.                                                                                                      | Medium   |
| Update Boat Availability. US-009 | As the system, I want to automatically update the availability status of boats based on bookings, So that customers can only see boats that are available for the desired time.                                  | The system checks the boat's schedule and updates availability in real time when a booking is made or cancelled.                                                                                                                                                        | High     |
| Manage Boat Inventory. US-010    | As service assistant, I want to add, update, or remove boats from the system, So that the boat rental system reflects the current available inventory.                                                           | The service assistant can add new boats to the inventory with details such as name, type, capacity, location, and availability. The service assistant can update existing boat details. The service assistant can remove boats that are no longer available for rental. | High     |
| View Reports. US-011             | As the owner, I want to view various reports, such as revenue, bookings, and boat availability, So that I can analyse system performance and make informed business decisions.                               | The owner can generate and view reports based on specific criteria (e.g., date range, location, boat category). Reports include key metrics such as total revenue, number of bookings, and boats available for hire.                                                | Medium   |

2\. **Product Backlog Creation**: Below is the product backlog for the Boat Rental System which serves as the central list of all features, enhancements, bug fixes, and technical improvements needed for the product. It represents the work that needs to be done and helps ensure that the development process aligns with both user needs and business goals.

This product backlog will evolve over time, with priorities changing as new features are identified or feedback is received from users.

| Story ID | User Story               | Priority (MoSCoW) | Effort Estimate | Dependencies            |
|----------|--------------------------|-------------------|-----------------|-------------------------|
| US-001   | Register Account         | Must-have         | 5               | None                    |
| US-002   | Browse Available Boats   | Must-have         | 5               | None                    |
| US-003   | Make Booking             | Must-have         | 5               | Browse Available Boats  |
| US-004   | Cancel Booking           | Must-have         | 5               | Make Booking            |
| US-005   | Approve rental request   | Must-have         | 3               | Make Booking            |
| US-006   | Pay for Booking          | Must-have         | 5               | Approve rental request  |
| US-007   | Process Payment          | Should-have       | 3               | Pay for Booking         |
| US-008   | Send Confirmation Email  | Should-have       | 3               | Process Payment         |
| US-009   | Update Boat Availability | Must-have         | 3               | Send Confirmation Email |
| US-010   | Manage Boat Inventory    | Should-have       | 3               | None                    |
| US-011   | View Reports             | Should-have       | 3               | None                    |

3\. **Spring Planning**: Below is a sprint plan for the Boat Rental System which is a detailed breakdown of the work that will be completed during a 2 week sprint.

Sprint Planning plays a crucial role in the development for the Boat Rental System by helping the team break down the work into manageable chunks, setting clear priorities, and establishing a plan for delivering incremental value to users.

| Task ID | Task Description                                  | Assigned To                    | Estimated Hours | Status |
|---------|---------------------------------------------------|--------------------------------|-----------------|--------|
| T-001   | Implement an account registration and login form. | Front-End Dev Team             | 48 hours        | To do  |
| T-002   | Implement backend authentication.                 | Backend Dev Team               | 72 hours        | To do  |
| T-003   | Develop boat search and selection pages.          | Front-End Dev Team             | 72 hours        | To do  |
| T-004   | Implement basic booking form.                     | Front-End Dev Team             | 48 hours        | To do  |
| T-005   | Integrate a basic payment gateway for testing.    | Front-End and Backend Dev Team | 96 hours        | To do  |
