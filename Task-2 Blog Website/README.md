

# Blog Website

A simple blog website built using HTML, CSS, Node.js, and MongoDB. This application allows users to create, read, edit, and delete articles. The server-side is powered by Express and Mongoose, while the front-end is rendered using EJS templates.


https://github.com/user-attachments/assets/3c05e3e5-d715-4aec-9036-3184ad17c7e4


## Features

- **Create**: Add new blog articles.
- **Read**: View a list of all blog articles.
- **Edit**: Modify existing blog articles.
- **Delete**: Remove articles from the blog.

## Installation

### Prerequisites

Ensure you have Node.js and npm installed on your machine. You can download Node.js from [nodejs.org](https://nodejs.org/).

### Setting Up the Project


1. **Install Dependencies**

   ```bash
   npm install
   ```

   This will install all required packages listed in `package.json`.

2. **Install Dev Dependencies**

   For development, you'll need `nodemon` to automatically restart the server on file changes:

   ```bash
   npm install --save-dev nodemon
   ```

3. **Set Up MongoDB**

   Ensure you have MongoDB installed and running. You can download it from [mongodb.com](https://www.mongodb.com/try/download/community).

   Start MongoDB with the following command:

   ```bash
   mongod
   ```

   ![image](https://github.com/user-attachments/assets/6743666e-4f78-4fde-bcd3-afa431469336)


   By default, MongoDB listens on port `27017`.

## Running the Application

To start the server and run the application, use:

```bash
npm run blogwebsite
```

This command uses `nodemon` to start `server.js` and automatically restarts the server on code changes.

## Usage

1. **Access the Application**

   Open your web browser and navigate to `http://localhost:3000` to view the blog website.

2. **Create an Article**

   ![image](https://github.com/user-attachments/assets/3f90ca68-4669-466b-bb33-1842d8a9434a)


   - Go to `/new` to access the form for creating a new article.
   - Fill in the article title and content, then submit the form.

3. **Read Articles**

![image](https://github.com/user-attachments/assets/f9f69f69-9d8e-45ee-82e5-802c97819c02)


   - The home page (`/`) lists all existing blog articles.
   - Click on an article's title to view the full content.

4. **Edit an Article**

![image](https://github.com/user-attachments/assets/a393fb47-d614-449b-8ac2-0954c09a0eb5)


   - Navigate to `/edit/:id`, replacing `:id` with the article's ID.
   - Modify the article title and content, then submit the form to save changes.

5. **Delete an Article**


![image](https://github.com/user-attachments/assets/df667458-1718-4643-ad5d-f988b6242369)

   - On the article list page (`/`), click the "Delete" button next to the article you want to remove.

## Project Structure

- **`server.js`**: Main server file that sets up the Express server and connects to MongoDB.
- **`models/Article.js`**: Mongoose model for blog articles.
- **`routes/index.js`**: Route handlers for creating, reading, editing, and deleting articles.
- **`views/`**: EJS templates for rendering HTML pages.
- **`public/`**: Static files like CSS stylesheets.

## Commands

- **`npm install`**: Install all dependencies.
- **`npm install --save-dev nodemon`**: Install `nodemon` for development.
- **`npm run blogwebsite`**: Start the server with `nodemon`.



## Acknowledgments

- **Express**: Web framework for Node.js.
- **Mongoose**: MongoDB object modeling tool.
- **EJS**: Templating engine for rendering HTML.

