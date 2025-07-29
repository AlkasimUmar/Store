# Express.js & PostgreSQL CRUD API

## Setup

1. Install PostgreSQL and Node.js
2. Create a PostgreSQL database and run the following SQL to create the users table:
   ```sql
   CREATE TABLE users (
     id SERIAL PRIMARY KEY,
     name VARCHAR(100),
     email VARCHAR(100),
     age INTEGER
   );
   ```
3. Clone this repo and run:
   ```bash
   npm install
   ```
4. Update the database connection config in `index.js`.
5. Start the server:
   ```bash
   node index.js
   ```

## API Endpoints

- `GET /users` - Get all users
- `GET /users/:id` - Get a specific user
- `POST /users` - Create a new user (`name`, `email`, `age` in body)
- `PUT /users/:id` - Update a user (`name`, `email`, `age` in body)
- `DELETE /users/:id` - Delete a user

## Testing

Use Postman or similar tool to test the API endpoints.