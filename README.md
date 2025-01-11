Project Description:
This project is a simple Airbnb-like application built using Node.js, Express, and EJS. 
It provides the ability for users to view a list of registered homes, 
and for hosts to add new homes to the platform.
The app dynamically updates the navigation and page content based on the active page, 
and allows for seamless transitions between viewing homes and adding new ones.


Features:
Home Page: Displays a list of registered homes with details such as name, location, price, and rating.
Add Home Page: Hosts can add new homes to the platform by filling out a form.
Dynamic Navigation: The navigation bar highlights the active page, giving users a clear indication of where they are in the app.
Home Registration: Hosts can submit their home details, which are added to the list of registered homes.
Responsive UI: The app uses TailwindCSS for a clean, responsive design.
Installation:
Clone the repository:

git clone https://github.com/your-username/airbnb-clone.git
Navigate to the project directory:

cd airbnb-clone
Install the required dependencies:

npm install
Start the application:


npm start
Open your browser and navigate to http://localhost:3000 to access the app.

Project Structure:
/airbnb-clone
│
├── /views
│   ├── home.ejs          # Home page template
│   ├── add-home.ejs      # Add home page template
│   ├── home-added.ejs    # Confirmation page for home added
│   └── /partials
│       └── nav.ejs       # Navigation bar partial
├── /routes
│   ├── hostRouter.js     # Routes for home registration
│   └── userRouter.js     # Routes for viewing homes
├── /public
│   ├── /styles
│   └── /images
├── app.js                # Main entry point for the app
├── package.json          # Project dependencies
└── README.md             # Project documentation
How It Works:
Home Route (/):

The userRouter renders the home page, which displays the list of registered homes.
Homes are stored in an array (registeredHomes) and displayed dynamically in the front-end.
Add Home Route (/host/add-home):

The hostRouter renders the form where hosts can submit new homes.
On form submission, the home details are added to the registeredHomes array, and a success message is shown.
Dynamic Navigation:

The navigation bar is dynamically updated based on the current page (Home or Add Home).
The active page is highlighted using TailwindCSS classes.
Home Registration:

Hosts can register their homes, which are stored in the registeredHomes array.
After a successful submission, a confirmation page is shown.
Technologies Used:
Node.js: JavaScript runtime for building the back-end server.
Express: Web framework for routing and handling HTTP requests.
EJS: Templating engine for rendering dynamic views on the front-end.
TailwindCSS: Utility-first CSS framework for styling the application.
How to Contribute:
Fork the repository.
Create a new branch (git checkout -b feature-name).
Commit your changes (git commit -am 'Add feature').
Push to the branch (git push origin feature-name).
Create a new Pull Request.
