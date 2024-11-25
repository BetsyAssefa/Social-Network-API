# Social-Network-API

## Description
The Social Network API is a robust backend application designed to handle the data of a social network platform. It allows users to create and manage profiles, post thoughts, react to other users' thoughts, and add or remove friends. Built with MongoDB, Express.js, and Node.js, this API provides a scalable and efficient solution for managing dynamic social interactions.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Endpoints](#endpoints)
- [Technologies](#technologies)
- [License](#license)

---

## Features
- User Management:
  - Create, update, and delete user profiles.
  - Add or remove friends.
- Thought Management:
  - Post, update, and delete thoughts.
  - Add reactions to thoughts.
- Scalable database using MongoDB and Mongoose ODM.
- RESTful API design with organized route handling.

---

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/BetsyAssefa/Social-Network-API.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Social-Network-API
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Set up the environment variables:
   - Create a `.env` file in the root directory.
   - Add the following variables:
     ```env
     MONGODB_URI=mongodb://localhost:27017/socialNetworkDB
     PORT=3001
     ```
5. Seed the database (optional):
   ```bash
   npm run seed
   ```

---

## Usage
1. Start the server:
   ```bash
   npm start
   ```
2. Access the API at `http://localhost:3001`.

Use a tool like Postman or Insomnia to test API endpoints.

---

## Endpoints
### User Routes
- **GET /api/users** - Retrieve all users.
- **GET /api/users/:id** - Retrieve a single user by ID.
- **POST /api/users** - Create a new user.
- **PUT /api/users/:id** - Update a user by ID.
- **DELETE /api/users/:id** - Delete a user by ID.
- **POST /api/users/:id/friends/:friendId** - Add a friend.
- **DELETE /api/users/:id/friends/:friendId** - Remove a friend.

### Thought Routes
- **GET /api/thoughts** - Retrieve all thoughts.
- **GET /api/thoughts/:id** - Retrieve a single thought by ID.
- **POST /api/thoughts** - Create a new thought.
- **PUT /api/thoughts/:id** - Update a thought by ID.
- **DELETE /api/thoughts/:id** - Delete a thought by ID.
- **POST /api/thoughts/:thoughtId/reactions** - Add a reaction to a thought.
- **DELETE /api/thoughts/:thoughtId/reactions/:reactionId** - Remove a reaction.

---

## Technologies
- **Backend:** Node.js, Express.js
- **Database:** MongoDB, Mongoose
- **Utilities:** Insomnia/Postman for API testing

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contributing
Contributions are welcome! If you find any issues or want to enhance the application, feel free to open an issue or submit a pull request.

---

## Questions
For any questions or feedback, please contact me:
- **GitHub:** [BetsyAssefa](https://github.com/BetsyAssefa)
- **Email:** bitsietassefa5@gmail.com

