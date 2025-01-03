
# WanderLust: Vacation Rental Platform

[Live Demo](https://wanderlust-2341.onrender.com)

## Overview
**WanderLust** is a vacation rental platform, similar to Airbnb, that allows users to explore and book unique accommodations worldwide. Built using the **MERN stack** (MongoDB, Express.js, React.js, and Node.js), WanderLust provides a seamless experience for both travelers and hosts to list, discover, and book short-term stays.

## Key Features
- **Search & Discovery**: Find properties by location, date, price range, and other filters.
- **Booking System**: Real-time booking with integrated availability calendars.
- **User Authentication**: Secure login and registration for guests and hosts.
- **Host Listings**: Hosts can manage property listings with photos, pricing, and availability.
- **Reviews & Ratings**: Guests can leave reviews and rate properties based on their experience.
- **Favorites**: Save properties to a favorites list for future bookings.

## Technology Stack
- **Frontend**: React.js for dynamic UI.
- **Backend**: Node.js and Express.js for handling server-side logic and API endpoints.
- **Database**: MongoDB for managing users, properties, and bookings.
- **Authentication**: JWT (JSON Web Tokens) for secure user sessions.

## Key Components
1. **User Authentication**: 
   - Secure login and registration for both guests and hosts.
   - JWT-based token system for session management.
2. **Property Listings**:
   - Hosts can list properties with details like descriptions, images, pricing, and available dates.
3. **Search & Filter**:
   - Allows users to search properties by location, dates, and price range with advanced filters (amenities, type of property, etc.).
4. **Booking System**:
   - Users can book available properties in real-time, with calendar integration for availability.
5. **Reviews & Ratings**:
   - Guests can submit reviews and ratings after their stay, helping future travelers make informed decisions.
6. **Favorites**:
   - Users can save their favorite properties for quick access and future bookings.

## Live Demo
Check out the live version of WanderLust: [WanderLust Live](https://wanderlust-2341.onrender.com)

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/wanderlust.git
    ```
2. Install the necessary dependencies for both the server and client:
    ```bash
    cd wanderlust
    npm install
    cd client
    npm install
    ```
3. Set up the environment variables for the backend in a `.env` file:
    ```bash
    MONGO_URI=your-mongodb-connection-string
    JWT_SECRET=your-jwt-secret
    ```
4. Start the development server:
    ```bash
    cd wanderlust
    npm run dev
    ```
   This will start both the client and server concurrently.

## API Endpoints
1. **User Authentication**:
   - `POST /api/users/register`: Register a new user.
   - `POST /api/users/login`: Log in a user and return a JWT.
   
2. **Property Listings**:
   - `GET /api/properties`: Retrieve all properties.
   - `POST /api/properties`: Create a new property listing (Host feature).
   - `GET /api/properties/:id`: Retrieve details of a specific property.

3. **Bookings**:
   - `POST /api/bookings`: Create a booking for a property.
   - `GET /api/bookings`: Retrieve bookings for a user or host.

4. **Reviews**:
   - `POST /api/reviews`: Submit a review for a property.
   - `GET /api/reviews/:propertyId`: Retrieve all reviews for a specific property.

## Future Enhancements
- **Payment Integration**: Add Stripe or PayPal integration for handling payments.
- **Dynamic Pricing**: Implement dynamic pricing based on seasons or demand.
- **Host Dashboard**: Create a dashboard for hosts to manage properties, bookings, and earnings.
- **Messaging System**: Enable direct communication between guests and hosts.
- **Enhanced Search Filters**: Add filters like pet-friendly, proximity to landmarks, etc.

## Contribution
We welcome contributions! Feel free to open a pull request to suggest enhancements or fix bugs.

## License
This project is licensed under the MIT License.
