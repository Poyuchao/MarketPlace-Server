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

## Install Dependencies
3. **npm install**

## Start the Server
4. **npm start**


## API Endpoints

Our backend server provides a comprehensive suite of API endpoints to manage users, products, and shopping cart functionalities. Below is a detailed list of available endpoints and their purposes.

### User Management

- **Authenticate User Login**
  - `POST /login`
  - Logs in a user with their credentials.

- **Register New User Account**
  - `POST /register`
  - Registers a new user account with the required information.

- **Request Password Reset Code**
  - `POST /ForgetPassword`
  - Sends a password reset code to the user's email.

- **Reset User's Password**
  - `POST /reset`
  - Allows a user to reset their password using a verification code.

### Product Management

- **Fetch All Products**
  - `GET /products`
  - Retrieves a list of all products available.

### Shopping Cart Operations

- **Retrieve User's Shopping Cart**
  - `GET /api/cart`
  - Fetches the current state of a user's shopping cart.

- **Add Item to Cart**
  - `POST /api/cart/add`
  - Adds a specified item to the user's shopping cart.

- **Increase Item Quantity**
  - `POST /api/cart/increaseQuantity`
  - Increases the quantity of a specific item in the user's cart.

- **Decrease Item Quantity**
  - `POST /api/cart/decreaseQuantity`
  - Decreases the quantity of a specific item in the user's cart.

- **Remove Item from Cart**
  - `POST /api/cart/remove`
  - Removes a specified item from the user's shopping cart.

- **Reset User's Cart**
  - `POST /api/cart/resetCart`
  - Resets the user's cart to empty, removing all items.

- **Save Current Cart State**
  - `POST /api/cart/save`
  - Saves the current state of the user's shopping cart.

### Static Files

- **Serve Images**
  - `GET /images`
  - Serves images stored on the server, typically for product images.

- **Serve Database File**
  - `GET /db`
  - Directly serves the `db.json` file, offering raw access to the mock database for debugging or direct queries.

### Miscellaneous

- **Fetch User Data**
  - `GET /getUserData`
  - Retrieves specific user data, such as usernames and their shopping carts, providing insight into user behavior and cart contents.

## Running the Server

Start the server to listen on the specified port in your `.env` file, or it will default to port 3001. With the server running, you're now ready to handle requests and manage data efficiently for **Taiwan Good Stuff**.

Remember to check back for updates to our API and new features. We're constantly working to improve our platform and appreciate your support and feedback!

