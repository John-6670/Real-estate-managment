# Real Estate Manager App (C) - Semester 1 Project
This document outlines the features and functionalities of a real estate manager application written in C, suitable for a semester 1 project.
## Features
### User Management:
- **User Registration:** Users can create accounts with username, password, Surname, Lastname, phone number, national ID, and email.
- **Admin Account:** A pre-defined admin account exists with fixed credentials for administrative tasks.
- **Forgot Password:** Users can recover their password by verifying their identity through chosen method (National ID, phone number, or email). (Verification involves confirmation by the user, no actual emails or messages are sent).
- **2-Step Verification:** Users can enable two-step verification using their National ID, phone number, or email for added security.
- **User Settings:** Users can modify their password, phone number, email, and 2-step verification settings
### Estate Management:
- **Estate Addition:** Users can add different types of estates:
    - Residential (Sale/Rent)
    - Office (Sale/Rent)
    - Field (Sale/Rent)
- **Estate Deletion (Archiving):** Estates can be marked as deleted (archived) by the user but remain accessible to the admin.
- **Estate Reports (User):** Users can generate reports on the following criteria (all reports exclude deleted estates):
	- Total number of estates
    - Filter by Regional Municipality
    - Filter by age of the estate (construction year)
    - Filter by price range (sale estates only)
    - Filter by mortgage/rent range (rent estates only)
    - Filter by area range (square meters)
    - Filter by number of bedrooms (residential estates only)
    - Filter by floor number (residential estates only)
- **Estate Reports (Admin):** Admin have access to all user reports and additionally can view:
    - User ranking based on the number of estates added (including deleted ones)
    - Filter estates by registration date
    - Filter estates by deletion date
    - List of all users with their last activity
## Technical Implementation:
- The program is written in C, focusing on basic data structures, string manipulation, and file handling.
- User data and estate data will be stored in separate files with appropriate data types for efficient access and manipulation.
- Input validation will be implemented to ensure data integrity (e.g., checking format of National ID, email, and phone number).
- Menus will be used for user interaction and navigation.
