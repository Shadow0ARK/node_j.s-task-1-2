This server defines routes for /home, /about, /contact, and /greet with the logic separated for better clarity and maintenance.

Key Elements:
Controllers:

mainPage: Responds with "main page".
homePage: Responds with "home page".
aboutPage: Responds with a description about the developer.
contactPage: Responds with contact information.
greetPage: Responds with "Hello, [name]!" or defaults to "Hello, guest!".
Routes:

Routes like /home, /about, /contact, and /greet are defined and handled by corresponding controller functions.
Server:

The Express server listens on a specified port (default 6710) and routes are connected to their logic.
Installation & Running:
Install Express:

bash
Copy code
npm init -y
npm install express
Run the server:

bash
Copy code
node server.js
Available Routes:
/ – Main Page: main page
/home – Home Page: home page
/about – About Page: Developer's info
/contact – Contact Page: Instagram contact
/greet?name=YourName – Greet with optional name, defaults to "guest" if not provided.

2.Build a server with a route /greet that accepts a query parameter name and responds with
personalized greeting message, e.g., &amp;quot;Hello, [name];

Server:
Displays a form at the root (/).
Accepts a POST request on the /greet route.
Functionality:
Responds with Hello, [name]! if the user provides a name.
Defaults to Hello, Guest! if no name is provided.
Code Summary:
Middleware: Parses URL-encoded data from forms.
GET /: Sends an HTML form for the user to enter their name.
POST /greet: Receives the name from the form and responds with a personalized greeting.
This summarizes the functionality without focusing on files or structure, keeping it very brief and to the point.


Task 2:

The PDF file you uploaded contains a *Full Stack Development Task (Task 2)*. It includes two main programming exercises:

1. *Basic HTTP Server with Routes and Methods (GET, POST, PUT, DELETE):*
   - A Node.js server is created using the http module.
   - Different routes are defined (/, /about, /api/data) with corresponding HTTP methods:
     - GET for retrieving data.
     - POST for submitting data.
     - PUT for updating data.
     - DELETE for deleting data.
   - The server checks the incoming requests and responds accordingly, with a "404 Not Found" message for invalid routes.

2. *File Upload Server using Express and Multer:*
   - An Express server is created for file uploads using the multer middleware.
   - The storage engine is configured to save files in an uploads/ directory with a timestamped filename.
   - The server handles a POST request at /upload where users can upload image files (restricted to JPEG, JPG, PNG, GIF).
   - If the upload succeeds, the server sends back the uploaded file's name, and if it fails, appropriate error messages are sent.

These tasks demonstrate the use of HTTP servers, file handling, and middleware integration in a full stack environment.

If you plan to upload this to GitHub, you can create a repository and add these code files along with relevant documentation. Would you like assistance with creating a README for your repository?
