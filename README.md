# To-Do List Application

A simple and elegant to-do list web application built with Node.js, Express, and EJS templating. This project features separate lists for home and work tasks with a clean, user-friendly interface.

## Features

- **Dynamic Date Display**: Shows the current date in a readable format (e.g., "Monday, January 5")
- **Multiple Lists**: Separate to-do lists for home and work tasks
- **Add Items**: Easily add new tasks to your lists
- **Item Limit**: Automatically manages list size (maximum 10 items per list)
- **Responsive Design**: Clean and modern UI with custom styling
- **About Page**: Additional information page

## Technologies Used

- **Node.js**: JavaScript runtime environment
- **Express.js**: Web application framework
- **EJS**: Embedded JavaScript templating
- **Body-Parser**: Middleware for parsing request bodies
- **Nodemon**: Development tool for auto-restarting the server

## Project Structure

```
├── app.js              # Main application file
├── date.js             # Date formatting module
├── package.json        # Project dependencies
├── public/
│   └── css/
│       └── styles.css  # Application styling
└── views/
    ├── about.ejs       # About page template
    ├── footer.ejs      # Footer partial
    ├── header.ejs      # Header partial
    └── lists.ejs       # Main to-do list template
```

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd angela-yu-todolist-master
```

2. Install dependencies:
```bash
npm install
```

3. Start the application:
```bash
npm start
```

4. Open your browser and navigate to:
```
http://localhost:3001
```

## Usage

### Home List
- Access the home list at the root URL (`/`)
- Add personal tasks and daily to-do items
- Click the `+` button to add new items

### Work List
- Access the work list at `/work`
- Manage work-related tasks separately
- Same functionality as the home list

### About Page
- Visit `/about` to view additional information about the app

## Default Items

The application comes with two pre-populated items on the home list:
- Finish JS Course
- Finish Python Course

## Configuration

The server runs on **port 3001** by default. You can modify this in `app.js`:

```javascript
app.listen(3001, function () {
    console.log("server is running on port 3001");
});
```

## Development

This project uses Nodemon for development, which automatically restarts the server when file changes are detected. To start in development mode:

```bash
npm start
```

## Notes

- This project is part of Angela Yu's web development course
- The application uses in-memory storage, so data is not persisted between server restarts
- Maximum of 10 items per list (older items are automatically removed when the limit is reached)

## Future Enhancements

Potential improvements for this project:
- Add database integration for persistent storage
- Implement delete functionality for individual items
- Add the ability to mark items as complete
- Create custom lists with user-defined names
- Add user authentication
- Implement data validation

## License

ISC

## Author

Ashley
