Project Type: E-commerce platform for groceries and other products, connecting sellers and buyers.

Tech Stack:

Client: React (with Vite), JavaScript, React Router DOM, Axios, React Hot Toast, Tailwind CSS.

Server: Node.js, Express.js, MongoDB, Mongoose, Cookie-parser, Cors, Dotenv, Cloudinary, Multer, Stripe.

Architecture:
Client (View): React components handle the user interface and interactions.
Server (Controller): Express.js routes and controllers manage requests, data processing, and responses.
Model: Mongoose models define the data structure and interact with the MongoDB database.
Separate routes and controllers exist for users, sellers, products, carts, addresses, and orders.

Key Features:
User Features:
- User registration and login.
- Product browsing and searching.
- Adding products to cart.
- Managing delivery addresses.
- Placing orders.
- Viewing order history.
Seller Features:
- Seller registration and login.
- Adding and managing products.
- Viewing order details.
General Features:
- Product categories.
- Product details page.
- Payment processing (Stripe integration).
- Image uploading (Cloudinary integration).

Implementation Steps:

1. Database Setup:
   - INSTRUCTION: Set up a MongoDB database using Mongoose. Define schemas for User, Product, and Order. Keep it simple initially with essential fields: User (name, email, password), Product (name, description, price, category, image URL), Order (userId, products, totalAmount, status).

2. User Authentication:
   - INSTRUCTION: Implement user registration and login using Express.js and Mongoose. Use bcrypt for password hashing. Create basic user routes and controllers for signup and login.
   - INSTRUCTION: Implement JWT (JSON Web Tokens) for authentication. Store the token in a cookie.

3. Product Listing and Details:
   - INSTRUCTION: Create API endpoints for fetching and displaying products. Implement basic product filtering by category.
   - INSTRUCTION: Create a product details page with essential product information.

4. Shopping Cart:
   - INSTRUCTION: Implement a basic shopping cart functionality. Allow users to add products to the cart and update quantities. Store cart data in the database or session storage.

5. Order Placement:
   - INSTRUCTION: Implement a simplified order placement process. Allow users to submit orders with their cart items and delivery address.
   - INSTRUCTION: Integrate a basic payment gateway (e.g., Stripe) for processing payments. For the MVP, you can use Stripe's test mode.

6. User Interface:
   - INSTRUCTION: Build a simple and intuitive user interface using React and Tailwind CSS. Focus on product browsing, cart management, and order placement.
   - INSTRUCTION: Create a basic product listing page, product details page, cart page, and order confirmation page.

7. Deployment:
   - INSTRUCTION: Deploy the application to a cloud platform (e.g., Heroku, Netlify, Vercel).
