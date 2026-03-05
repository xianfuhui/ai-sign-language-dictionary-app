					Local Deployment (Offline)
Prepare - Download the application to your device
	Platform: Node.js
	Database: MongoDB Compass
Steps to Local Deployment:
	Step 1 - Download and extract the application files to your local device
	Step 2 - Configure Environment Variables: Open the .env file located in the "source/Source" folder and edit the file with the following settings
	Explanation of .env variables:
		MONGO_URI: The URI for connecting to your MongoDB database, configured to connect to a local MongoDB server on port 27017 and use the system database.
		PORT: The port number on which the application will listen for incoming connections, set to 3000 in this configuration.
		KEY: A secret key used for security purposes within the application.
		USER_EMAIL and PASS_EMAIL: Email credentials used for account management. Ensure that PASS_EMAIL is securely managed as it might be obfuscated or encrypted.
	Step 3 - Install Dependencies: Run the following commands to install the necessary dependencies and start the application:
		npm install
		npm start
	Step 4 – Open the MongoDB Compass application: Import the JSON files from the "source/Database" folder into the database "system"
	Step 5 - Access the Application
		Open a web browser and navigate to admin site: http://localhost:3000/admin/login and login using the default account credentials:
			Username: admin
			Password: admin
		Open a web browser and navigate to user site: http://localhost:3000/user to register and login for user


					Production Deployment (Online)
Prepare – Access 3 Website applications
	Github: https://github.com/
	Render: https://render.com/
	MongoDB Atlas: https://www.mongodb.com/
Steps to Production Deployment:
	Step 1 - Go to "MongoDB Atlas" -> Go to "Database Access" -> Create user information to access the database
	Step 2 - Go to "Network Access" -> Create Network Access to Access Database
	Step 3 - Go to "Database" -> click "Browse Collections"
 	Step 4 - Insert data from the "Database" folder and the same folder as the "Source" folder.
 	Step 5 - Go to "Database" -> click "Connect"
	Step 6 - Choose "Drivers"
	Step 7 - Copy the connection link to include in the connection code to the database
	Step 8 - Go to the .env file in "Source" and replace the "MONGO_URI" path you just copied to connect to MongoDB Atlas
 	Step 9 - Push the source code to "GitHub"
 	Step 10 - Go to "Render" -> and select "Deploy a Web Service"
	Step 11 - Select the repository that has pushed the code
	Step 12 - Configure
	Step 13 - Deploy the website service
	Step 14 - Images of the website successfully deployed
