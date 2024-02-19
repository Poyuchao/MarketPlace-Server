# Taiwan Good Stuff - Backend Server

Welcome to the backend server repository for **Taiwan Good Stuff**, an e-commerce platform dedicated to bringing you the finest products from Taiwan. Our website is built using the React framework, leveraging technologies such as JavaScript, TailwindCSS, and HTML to provide a seamless and responsive user experience. This server is responsible for handling all backend functionalities, including user management, product listings, and shopping cart operations.

## Contributors

- **PoYu**
- **Kristen**

## Technologies

- **Node.js** and **Express.js**: For the server framework.
- **MongoDB**: For the database, with **Mongoose ODM** for data modeling.
- **Nodemailer**: For sending emails, such as password reset verification codes.
- **dotenv**: For managing environment variables.
- **CORS**: Middleware to enable cross-origin requests.

## Setup and Installation

1. **Ensure you have Node.js and npm installed** on your machine.
2. **Clone this repository** to your local machine.
   ```bash
   git clone <https://github.com/Poyuchao/MarketPlace-Server.git>

npm install

npm start


API Endpoints
User Management
POST /login: Authenticate user login.
POST /register: Register a new user account.
POST /ForgetPassword: Request a password reset code.
POST /reset: Reset the user's password with the verification code.
Product Management
GET /products: Fetch all products from db.json.
GET /api/cart: Retrieve a user's shopping cart.
POST /api/cart/add: Add an item to the user's cart.
POST /api/cart/increaseQuantity: Increase the quantity of a specific item in the cart.
POST /api/cart/decreaseQuantity: Decrease the quantity of a specific item in the cart.
POST /api/cart/remove: Remove a specific item from the cart.
POST /api/cart/resetCart: Reset the user's cart to empty.
POST /api/cart/save: Save the current state of the user's cart.
Static Files
GET /images: Serve images from the MongoDb_server directory.
GET /db: Serve the db.json file directly.
Miscellaneous
GET /getUserData: Fetch user data, specifically usernames and their carts.
Running the Server
The server can be started with the command npm start. It listens on the port specified in the .env file or defaults to port 3001.