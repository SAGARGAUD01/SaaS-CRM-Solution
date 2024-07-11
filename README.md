# SaaS CRM Solution

## Overview

This project is a SaaS CRM solution that provides a comprehensive suite of tools to manage client interactions and streamline operations. The key features include viewing upcoming bookings, tracking users via tagged links, writing session notes, accessing analytical data, and handling payments. 

# About me:

<a href="https://www.linkedin.com/in/sagargaud332/" target="_blank"><img alt="" src="https://img.shields.io/badge/LinkedIn-000?logo=linkedin&logoColor=0A66C2&style=for-the-badge" style="vertical-align:center" /></a>

## Features

1. **Viewing Upcoming Bookings**: Allows users to see their upcoming appointments and manage their schedules.
2. **Tracking Users via Tagged Links**: Monitors the number of users arriving via specific links.
3. **Writing Session Notes**: Enables users to document notes for each session.
4. **Accessing Analytical Data**: Provides insights such as session frequency and monthly turnover.
5. **Handling Payments**: Manages payment collection and deposits into client accounts.

## Table of Contents

- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Setup and Installation](#setup-and-installation)
- [Development Workflow](#development-workflow)
- [API Documentation](#api-documentation)
- [Testing](#testing)

## Tech Stack

**Frontend**:
- React.js
- HTML, CSS
- Axios (for API calls)

**Backend**:
- Node.js
- Express.js
- MongoDB
- Mongoose (ORM)

**Payment Gateway**:
- Stripe API

**Analytics and Tracking**:
- Google Analytics
- Firebase

**DevOps**:
- Docker
- Kubernetes
- GitHub Actions (CI/CD)

**Testing**:
- Jest
- Cypress

## Project Structure

```
root
│
├── backend
│   ├── controllers
│   ├── models
│   ├── routes
│   ├── services
│   └── index.js
│
├── frontend
│   ├── src
│   │   ├── components
│   │   ├── pages
│   │   ├── services
│   │   └── App.js
│   └── public
│
├── .gitignore
├── docker-compose.yml
├── README.md
└── package.json
```

## Setup and Installation

### Prerequisites

- Node.js (v14 or higher)
- MongoDB
- Docker
- Docker Compose

### Installation

1. **Clone the repository**:
   ```sh
   git clone https://github.com/your-repo/saas-crm.git
   cd saas-crm
   ```

2. **Install dependencies**:
   - For backend:
     ```sh
     cd backend
     npm install
     ```
   - For frontend:
     ```sh
     cd frontend
     npm install
     ```

3. **Configure environment variables**:
   - Create a `.env` file in the `backend` directory and add the following:
     ```env
     PORT=5000
     MONGO_URI=your_mongodb_uri
     JWT_SECRET=your_jwt_secret
     STRIPE_SECRET_KEY=your_stripe_secret_key
     ```

4. **Run the application**:
   - Using Docker Compose:
     ```sh
     docker-compose up
     ```
   - Without Docker:
     - Start the backend:
       ```sh
       cd backend
       npm start
       ```
     - Start the frontend:
       ```sh
       cd frontend
       npm start
       ```

## Development Workflow

### Frontend Development

1. **Component Structure**:
   - Login Component: Handles user authentication.
   - Navbar Component: Navigation bar for accessing different pages.
   - Bookings Component: Main component for displaying bookings.
   - Booking Card Component: Displays individual booking details.
   - Error Handling Component: Displays errors if any occur.

2. **API Integration**:
   - Use Axios to fetch data from the backend.
   - Handle API responses and errors.

### Backend Development

1. **Setting Up Server**:
   - Initialize a Node.js server with Express.
   - Configure middleware for authentication and error handling.

2. **Controllers and Services**:
   - Create controllers for handling requests.
   - Implement business logic in service layers.

3. **Database Schema**:
   - Design schemas using Mongoose for MongoDB.
   - Implement CRUD operations.

### API Documentation

#### Booking API

- **Get Upcoming Bookings**:
  - **Endpoint**: `/api/bookings`
  - **Method**: GET
  - **Description**: Fetches a list of upcoming bookings.
  - **Response**:
    ```json
    {
      "bookings": [
        {
          "id": "1",
          "user": "Sagar Gaud",
          "service": "Consultation",
          "date": "2024-07-01T10:00:00Z",
          "status": "Confirmed"
        },
        ...
      ]
    }
    ```

## Testing

### Unit Tests

- Use Jest for unit testing frontend and backend components.
- Write tests for individual components and services.

### Integration Tests

- Use Cypress for end-to-end testing.
- Test the integration between frontend and backend.

### Running Tests

- **Frontend**:
  ```sh
  cd frontend
  npm test
  ```
- **Backend**:
  ```sh
  cd backend
  npm test
  ```

  # Zenstreet (Technical Case)
