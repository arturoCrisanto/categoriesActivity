## Activity: Book Management API

# Objective:

Build a Book Management API using Node.js and Express, following the given project structure. Use the provided mock data to represent books and implement basic CRUD operations.

---

## Project Structure:

```javascript
book-api/
├── controllers/
│   └── booksController.js  // Business logic for books
├── models/
│   └── booksModel.js      // Mock data for books
├── routes/
│   └── booksRoutes.js     // API routes for books
├── app.js                 // Main application file
└── package.json           // Project configuration
```

## Mock Data:

In the `models/booksModel.js` file, define the following mock data:

```javascript
// Mock data for books
const books = [
  {
    id: 1,
    title: "The Great Gatsby",
    author: "F. Scott Fitzgerald",
    genre: "Fiction",
    publicationDate: "1925-04-10",
  },
  {
    id: 2,
    title: "1984",
    author: "George Orwell",
    genre: "Dystopian",
    publicationDate: "1949-06-08",
  },
  {
    id: 3,
    title: "Moby-Dick",
    author: "Herman Melville",
    genre: "Adventure",
    publicationDate: "1851-10-18",
  },
  {
    id: 4,
    title: "To Kill a Mockingbird",
    author: "Harper Lee",
    genre: "Fiction",
    publicationDate: "1960-07-11",
  },
];

module.exports = books;
```

## Instructions:

### Set Up the Project:

- Initialize a Node project using.

```javascript
npm init -y
```

- Install Express nodemon and dotenv

```bash
npm i express nodemon dotenv
```

### Create Mock Data:

In the `models/` directory, create a `booksModel.js` file with the mock data provided above.

### Create Routes:

In the `routes/` directory, create routes for:

- GET `/books`: Retrieve all books.
- GET `/books/genre/:genre`: Filter books by genre.

### Implement Controller Logic:

In the `controllers/` directory, implement the logic to handle the routes. Use the mock data for the operations.

### Start the Server:

Set up Express in `server.js` and test the API using `Postman`.
