# Airbnb Clone Project

This project is a clone of the Airbnb web application, built using Node.js, Express.js, MongoDB, and other related technologies. It aims to replicate the core functionalities of Airbnb, allowing users to list their properties and book accommodations.

## Table of Contents

-   [Features](#features)
-   [Technologies Used](#technologies-used)
-   [Prerequisites](#prerequisites)
-   [Installation](#installation)
-   [Usage](#usage)
-   [Environment Variables](#environment-variables)
-   [Database Setup](#database-setup)
-   [Cloud Storage](#cloud-storage)
-   [Map Integration](#map-integration)
-   [Authentication](#authentication)
-   [Contributing](#contributing)
-   [License](#license)

## Features

-   **User Authentication:** User signup, login, and logout.
-   **Listing Management:** Users can create, edit, and delete property listings.
-   **Property Details:** Display property information, including title, description, price,country, location and images.
-   **Image Uploads:** Upload images for property listings.
-   **Booking System:** Users can book available properties.
-   **Search Functionality:** Search for properties based on location.
-   **Map Integration:** Display property locations on a map using Leaflet .
-   **Reviews:** Users can add and view reviews for listings.
-   **Admin Functionality (Optional):** Admin users can manage listings and users.
-   **Flash Messages:** display success and error messages to users.

## Technologies Used

-   **Node.js:** JavaScript runtime environment.
-   **Express.js:** Web application framework for Node.js.
-   **MongoDB:** Mongodb atlas database.
-   **Mongoose:** MongoDB object modeling tool.
-   **EJS:** Embedded JavaScript templates.
-   **Multer:** Middleware for handling file uploads.
-   **Cloudinary/AWS S3 (or similar):** Cloud storage for images.
-   **Leaflet:** JavaScript library for interactive maps.
-   **Passport.js:** Authentication middleware.
-   **Bcrypt:** Password hashing.
-   **Express-session:** Session management.
-   **Connect-flash:** Flash message handling.
-   **Dotenv:** Environment variable management.

## Prerequisites

-   Node.js (v14 or later)
-   npm (Node Package Manager)
-   MongoDB installed and running
-   Cloudinary/AWS S3 account and credentials (if using cloud storage)

## Installation

1.  Clone the repository:

    ```bash
    git clone <repository_url>
    cd <Airbnb Project>
    ```

2.  Install dependencies:

    ```bash
    npm install
    ```

3.  Create a `.env` file in the root directory and add your environment variables (see [Environment Variables](#environment-variables)).

4.  Start the server:

    ```bash
    node app.js
    ```

## Usage

1.  Open your browser and navigate to `http://localhost:3000`.
2.  Register or log in to your account.
3.  Browse listings, create new listings, or book accommodations.

## Environment Variables

Create a `.env` file in the root directory and add the following variables:

## Database Setup

1.  Ensure MongoDB is installed and running.
2.  The application will automatically create a database named `airbnb-clone` (or whatever you specify in `DB_URL`).

## Cloud Storage

1.  If using Cloudinary or AWS S3, create an account and obtain your API keys and secrets.
2.  Configure the cloud storage settings in your `.env` file.
3.  Ensure that the `cloudConfig.js` file is correctly set up to connect to your cloud storage provider.

## Map Integration

1.  Obtain a Mapbox API key and add it to your `.env` file.
2.  The application uses Leaflet to display maps. Ensure that Leaflet is correctly integrated into your views.

## Authentication

1.  The application uses Passport.js for authentication.
2.  Users can register and log in using email and password.
3.  Passwords are hashed using bcrypt for security.
4.  User sessions are managed using express-session.

## Contributing

1.  Fork the repository.
2.  Create a new branch for your feature or bug fix.
3.  Commit your changes.
4.  Push to the branch.
5.  Create a pull request.
