Ride-Sharing Platform Project
This project is a ride-sharing platform designed to enable ride-sharing options across different cities. Users can input their starting and destination cities to determine if they can share a ride based on pre-defined routes between cities. The project is implemented in C++ and uses a static dataset of cities with distances to facilitate route and cost calculation.

1) Features
Driver and User Management: Manages driver and user records using linked lists.
City Connectivity: Utilizes static data of city connections and distances for route calculations.
Ride Matching: Determines if two users can share a ride based on route overlap.
Cost Distribution: Calculates and distributes the ride cost among users if they can share a route.

File Structure
DataBase_management_src.cpp: Handles driver and user records, including linked list management.
ride_sharing.cpp: Core functionality to check if users can share rides and to calculate shared costs.
cities.txt: Contains city pairs with distances for route calculation.
driver.txt: Stores driver details such as name, license number, and contact information.
user.txt: Stores user records.

Prerequisites
A C++ compiler (e.g., GCC, MinGW).
Installation and Setup
Clone the repository:
bash
Copy code
git clone https://github.com/yourusername/ride-sharing-platform.git
Navigate to the project directory:
bash
Copy code
cd ride-sharing-platform
Compile the project using a C++ compiler:
bash
Copy code
g++ -o ride_sharing DataBase_management_src.cpp ride_sharing.cpp -std=c++11
Run the compiled executable:
bash
Copy code
./ride_sharing
Usage
Add Drivers and Users:

Add driver details in driver.txt in the format: Name, LicenseNumber, PhoneNumber
Add user details in user.txt.
Determine Ride-Sharing Eligibility:

Enter the starting and destination cities for two users.
The program will calculate if a ride-sharing route is possible and, if so, will display the cost-sharing arrangement.
Example Files
cities.txt
The cities.txt file contains city pairs and distances between them, structured as:

plaintext
Copy code
Jaipur Ajmer 132
Jaipur Alwar 150
Ajmer Bhilwara 132
...
driver.txt
The driver.txt file contains driver details in this format:

plaintext
Copy code
Mukesh Kumar, DLIN1234567890, 8764546890
Priya Sharma, DLIN0987654321, 4567822358
...
user.txt
The user.txt file stores user information in a similar structured format.
