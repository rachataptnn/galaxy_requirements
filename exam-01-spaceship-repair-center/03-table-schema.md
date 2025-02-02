## User schema

|    Column Name    |     Data Type     |                       Description                      |
|-------------------|-------------------|--------------------------------------------------------|
| user_id           | INT (Primary Key) | Unique identifier for the user                         |
| first_name        | VARCHAR(255)      | First name of the user                                 |
| last_name         | VARCHAR(255)      | Last name of the user                                  |
| primary_contact   | VARCHAR(255)      | Preferred method of contact (e.g., email, holo_comm)   |
| email             | VARCHAR(255)      | Email address of the user (optional)                   |
| phone_number      | VARCHAR(50)       | Phone number of the user (optional)                    |
| holo_comm         | VARCHAR(255)      | Holographic communicator identifier                    |
| subspace_address  | VARCHAR(255)      | Subspace communication address                         |
| telepathic_link   | VARCHAR(255)      | Telepathic link identifier                             |
| address           | VARCHAR(255)      | Physical address of the user                           |
| city              | VARCHAR(100)      | City of the user                                       |
| state             | VARCHAR(100)      | State of the user                                      |
| postal_code       | VARCHAR(20)       | Postal code of the user                                |
| planet            | VARCHAR(100)      | Planet of the user                                     |
| galaxy            | VARCHAR(100)      | Galaxy of the user                                     |
| registration_date | DATE              | Date when the user registered                          |
| membership_status | VARCHAR(50)       | Status of the user membership (e.g., active, inactive) |

<br/>

## Spaceship Schema

|     Column Name    |     Data Type     |                        Description                        |
|--------------------|-------------------|-----------------------------------------------------------|
| spaceship_id       | INT (Primary Key) | Unique identifier for the spaceship                       |
| central_ss_id      | INT (Primary Key) | Unique identifier for the spaceship                       |
| name               | VARCHAR(255)      | Name of the spaceship                                     |
| model              | VARCHAR(255)      | Model type of the spaceship                               |
| manufacturer       | VARCHAR(255)      | Company or entity that manufactured the spaceship         |
| crew_capacity      | INT               | Maximum number of crew members                            |
| passenger_capacity | INT               | Maximum number of passengers                              |
| launch_date        | DATE              | Date the spaceship was launched                           |
| status             | VARCHAR(50)       | Current status (e.g., active, retired, under maintenance) |
| speed              | FLOAT             | Maximum speed in light years per hour                     |
| weapons            | BOOLEAN           | Indicates if the spaceship has weapons                    |
| fuel_capacity      | FLOAT             | Maximum fuel capacity in liters                           |
| current_location   | VARCHAR(255)      | Current location of the spaceship                         |
| launch_date        | DATE              | Date the spaceship was launched                           |
| status             | VARCHAR(50)       | Current status (e.g., active, retired, under maintenance) |
| speed              | FLOAT             | Maximum speed in light years per hour                     |
| weapons            | BOOLEAN           | Indicates if the spaceship has weapons                    |
| fuel_capacity      | FLOAT             | Maximum fuel capacity in liters                           |
| current_location   | VARCHAR(255)      | Current location of the spaceship                         |

<br/>

## Booking Schema

| Column Name        | Data Type         | Description                                         |
|--------------------|-------------------|-----------------------------------------------------|
| booking_id         | INT (Primary Key) | Unique identifier for the booking                   |
| user_id            | INT               | Identifier for the user (client)                    |
| spaceship_id       | INT               | Identifier for the spaceship                        |
| technician_id      | INT               | Identifier for the technician assigned              |
| booking_date       | DATE              | Date the booking was made                           |
| appointment_date   | DATETIME          | Scheduled date and time of the appointment          |
| status             | VARCHAR(50)       | Status of the booking (e.g., confirmed, pending)    |
| special_requests   | TEXT              | Any special requests or notes from the client       |

<br/>

## Spare Part Schema

| Column Name        | Data Type         | Description                                         |
|--------------------|-------------------|-----------------------------------------------------|
| part_id            | INT (Primary Key) | Unique identifier for the spare part                |
| name               | VARCHAR(255)      | Name of the spare part                              |
| description        | TEXT              | Description of the spare part                       |
| manufacturer       | VARCHAR(255)      | Manufacturer of the spare part                      |
| model_number       | VARCHAR(100)      | Model number of the spare part                      |
| quantity_in_stock  | INT               | Number of units available in stock                  |
| price              | DECIMAL(10, 2)    | Price of the spare part                             |
| compatibility      | VARCHAR(255)      | Compatible spaceship models or types                |

<br/>

## Technician Schema

| Column Name        | Data Type         | Description                                         |
|--------------------|-------------------|-----------------------------------------------------|
| technician_id      | INT (Primary Key) | Unique identifier for the technician                |
| first_name         | VARCHAR(255)      | First name of the user                                 |
| last_name          | VARCHAR(255)      | Last name of the user                                  |
| primary_contact    | VARCHAR(255)      | Preferred method of contact (e.g., email, holo_comm)   |
| email              | VARCHAR(255)      | Email address of the user (optional)                   |
| phone_number       | VARCHAR(50)       | Phone number of the user (optional)                    |
| holo_comm          | VARCHAR(255)      | Holographic communicator identifier                    |
| subspace_address   | VARCHAR(255)      | Subspace communication address                         |
| telepathic_link    | VARCHAR(255)      | Telepathic link identifier                             |
| expertise_area     | VARCHAR(255)      | Area of expertise (e.g., propulsion, navigation)    |
| years_of_experience| INT               | Number of years of experience                       |
| certification      | VARCHAR(255)      | Certification or qualification details              |
| availability_status| VARCHAR(50)       | Current availability status (e.g., available)       |
