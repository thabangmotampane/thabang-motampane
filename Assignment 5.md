ASSIGNMENT 5

STUDENT: Thabang Motampane

STUDENT NUMBER: 251699544

USE CASES:

-   Rent boat
-   Validate customer information
-   Approve rental request
-   Generate contract
-   Make payment
-   Return boat
-   Discard boat
-   Suspend boat
-   Generate reports
-   Update licence list

ACTORS:

-   Sales assistant
-   Systems Administrator
-   Service assistant
-   Customer
-   Internet
-   Shop owner

USE CASE SPECIFICATIONS

Use Case: Rent Boat

Actor: Customer

Precondition: Customer is registered.

Postcondition: Customer details are submitted for verification.

Basic Flow:

1\. Customer inputs their details on the system.

2\. Customer uploads their skipper license on the system.

3\. Customer selects boat to rent.

Use Case: Validate Customer Information

Actor: Systems Administrator

Precondition: The customer has requested a boat to rent.

Postcondition: Boat rental is sent for approval.

Basic Flow:

1\. The systems administrator checks rental requests.

1\. The systems administrator checks and verifies the customer’s details and lisence.

Use Case: Approve Rental Request

Actor: Sales Assistant

Precondition: Boat rental is sent for approval.

Postcondition: Contract is generated for the customer.

Basic Flow:

1 . The sales assistant checks for approvals submitted from the systems administrator.

2\. The sales assistant approves the customer’s rental request.

Use Case: Generate Contract

Actor: Sales Assistant

Precondition: Rental request is approved.

Postcondition: Customer makes payment.

Basic Flow:

1\. The cashier generates a contract stipulating the terms and conditions of the servicing, collection and returning of the boat.

2\. The customer reads and signs the contract.

Use Case: Make Payment

Actor: Customer

Precondition: Contract is signed by the customer.

Postcondition: Customer receives the boat.

Basic Flow:

1\. The customer receives the quote and makes payment.

2\. The customer receives confirmation for the boat pick-up date and time.

Use Case: Return Boat

Actor: Customer and Sales Assistant

Precondition: Customer receives the boat.

Postcondition: The boat state is captured as returned.

Basic Flow:

1\. The customer returns the boat.

2\. The sales assistant checks the boat for damages.

3\. The sales assistant captures the boat’s returned state into the system.

Use Case: Discard Boat

Actor: Service Assistant and Shop Owner

Precondition: None.

Postcondition: The boat ID is removed from the system.

Basic Flow:

1\. The service assistant checks all the boats for wear and tear due to age and accidents.

2\. The service assistant sends a request to discard boats that are no longer functional.

3\. The shop owner approves the request to discard non-functional boats.

Use Case: Suspend Boat

Actor: Service Assistant

Precondition: None.

Postcondition: Boat ID status is changed to “Out of Service”.

Basic Flow:

1\. The service assistant checks for all the boats that need to undergo maintenance.

2\. The service assistant temporarily removes the boats (undergoing maintenance) from the system.

Use Case: Generate Reports

Actor: Shop Owner

Precondition: None.

Postcondition: Printed Reports.

Basic Flow:

1\. The shop owner generates various dated reports on customers, contracts and boats that will enable them to manage the business.

Use Case: Update License List

Actor: Internet

Precondition: None.

Postcondition: Boat ID status is changed to “Out of Service”.

Basic Flow:

1\. The internet updates the system’s license database with all the standards that govern the validity of a license.

2\. The internet updates the system with all valid licenses.

USE CASE DIAGRAM

[![A diagram of a person's diagram AI-generated content may be incorrect.](media/c630f57e81c4971494cf43f8d5e1491f.jpeg)](https://github.com/thabangmotampane/thabang-motampane/blob/main/Use%20case%20diagram.JPG)

TEST CASE DEVELOPMENT

| Test Case ID | Requirements ID | Description                                         | Steps                                                                                        | Expected Result                                                                                                        | Actual Result                                                                                                         | Status (Pass/Fail) |
|--------------|-----------------|-----------------------------------------------------|----------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------|--------------------|
| TC-001       | FR-001          | Customer requests to rent a boat.                   | 1. Enter personal details on registration form. 2. Upload ID and Skipper License.            | Confirmation that the request has been submitted should display.                                                       | Confirmation that the request has been submitted should display.                                                      | Pass               |
| TC-002       | FR-002          | System Administrator verifies customer information. | 1. Input Customer’s ID number to trace and verify the customer’s License in the system.      | The customer’s License should pop up from the system.                                                                  | The customer’s License should pop up from the system.                                                                 | Pass               |
| TC-003       | FR-003          | Sales Assistant Approves rental.                    | 1. Click on the customer’s request and approve rental request. 2. Send contract to customer. | 1. A notification should be sent to the customer about approval. 2. The customer should receive the contract to sign.  | 1. A notification should be sent to the customer about approval. 2. The customer should receive the contract to sign. | Pass               |
| TC-004       | FR-004          | Customer makes payment.                             | 1. Click on the payment information. 2. Input banking details to make payment.               | Payment confirmation should be sent to the sales assistant.                                                            | Payment confirmation should be sent to the sales assistant.                                                           | Pass               |
| TC-005       | FR-005          | Customer returns boat.                              | 1. Submit a report on the condition of the boat. 2.Determine extra charges to customer.      | Customer receives damages report.                                                                                      | Customer receives damages report.                                                                                     | Pass               |
| TC-006       | FR-006          | Service Assistant discards boat.                    | 1. Submit a report on the condition of the boat. 2. Submit motivation for discarding boat.   | 1. Approval request should be sent within 2 seconds.                                                                   | 1. Approval request should be sent within 2 seconds.                                                                  | Pass               |
| TC-007       | FR-007          | Service Assistant suspends boat.                    | 1. Submit report on the condition of the boat.                                               | 1. Maintenance process should display within 2 seconds.                                                                | 1. Maintenance process should display within 2 seconds.                                                               | Pass               |
| TC-008       | FR-008          | Licenses are updated.                               | 1. Schedule license updates.                                                                 | 1. licenses should update as scheduled.                                                                                | 1. licenses should update as scheduled.                                                                               | Pass               |

**Challenges in Translating Requirements to Use Cases.**

Translating system requirements into use case diagrams can be a challenging task due to various reasons. Often, system requirements provided by stakeholders are vague or incomplete. Translating these into use case diagrams can be difficult because the precise functionality or scope of the system may not be fully defined. Different stakeholders may have different interpretations of the requirements, leading to inconsistencies in the use case diagram.

As the project progresses, system requirements might change based on new information, user feedback, or unforeseen technical issues. Keeping the use case diagram aligned with evolving requirements can also be a constant challenge.

As mentioned above, translating requirements to use case diagrams involves working with multiple stakeholders such as business analysts, developers, and end-users. Each stakeholder may have different priorities and expectations, making it hard to create a diagram that satisfies everyone.

Sometimes, the technical team may focus more on the system’s architecture than on how end-users will interact with the system, leading to use cases that don’t fully capture the user’s needs.

Non-functional requirements (e.g., performance, security, scalability) are often harder to represent in use case diagrams. These requirements might influence system behaviour, but their impact isn't always straightforward to map to specific use cases.

If a system has a large number of requirements, it can lead to an overwhelming number of use cases. Creating a diagram that remains clear and easy to understand while capturing all necessary details is a balancing act.
