Features
•	Frontend (React):
•	User interface to input source and multiple destinations (latitude and longitude).

•	Submit button to trigger route optimization.

•	Display of the optimized route sequence.

•	Backend (Node.js with Express):

•	API endpoint (/optimize-route) to handle optimization requests.

•	Integration with OpenRouteService API for route optimization.

•	Storage of locations and route results in MySQL.openrouteservice.org+1openrouteservice-py.readthedocs.io+1

•	Database (MySQL):

•	Tables:

•	Locations: Stores source and destination coordinates.

•	RouteResults: Stores the optimized route sequence.

•	Environment Configuration:

•	.env files for both frontend and backend to manage API keys and database credentials securely.LinkedIn+12YouTube+12openrouteservice+12

Setup Instructions
1.	Clone the Repository:
git clone https://github.com/yourusername/route-planner.git
cd route-planner

3.	Set Up the Backend:
•	Navigate to the backend directory:
cd backend
•	Install dependencies:

npm install

•	Create a .env file and add your OpenRouteService API key and MySQL credentials:

ORS_API_KEY=your_openrouteservice_api_key
DB_HOST=localhost
DB_USER=your_mysql_username
DB_PASSWORD=your_mysql_password
DB_NAME=route_planner
•	Run the server:

node index.js

4.	Set Up the Frontend:
•	Navigate to the frontend directory:

cd ../frontend

•	Install dependencies:

npm install

•	Create a .env file and add the backend API URL:

REACT_APP_API_URL=http://localhost:3000
•	Start the React application:

npm start
5.	Set Up the Database:
•	Use the provided schema.sql file to create the necessary tables and insert sample data into your MySQL database.

? Next Steps
Once you've set up the project:
•	Test the application by inputting a source and multiple destinations.
•	Verify that the optimized route is displayed correctly.
•	Ensure that the data is stored appropriately in the MySQL database.
If you need further assistance or enhancements, such as integrating a map visualization using Leaflet or Mapbox, feel free to ask!

 
 
 
Sources
