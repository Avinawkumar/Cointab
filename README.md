# Assignment

## Description

This documentation outlines the implementation details for the Cointab SE-ASSIGNMENT, a simple 2-page website developed using Node.js, Express, and MongoDB. The website interacts with the 'https://jsonplaceholder.typicode.com/' API to display user information and posts. The user data is stored in a MongoDB database, and the application provides functionality to add users, view user details, fetch posts, bulk add posts, and download posts in Excel format.

## System Architecture

The system follows a server-client architecture, where the Node.js server handles HTTP requests from the client, interacts with the MongoDB database for data storage, and communicates with the 'https://jsonplaceholder.typicode.com/' API to fetch external data.

## Features

- Add users, view user details, fetch posts, bulk add posts.
- Download the Post data in Excel format.


## Technologies Used

- Node.js
- Express.js
- MongoDB
- HTML
- CSS
- JavaScript


## Installation

  ### For Backend

   1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/cointab.git
    cd backend
    ```

  2. Install dependencies:

    ```bash
    npm install
    ```

  3. Set up your MongoDB connection by creating a `.env` file in the root directory with the following content:

    ```env
    mongourl=your-mongodb-connection-string
    port = your-port
    ```

  - Replace `your-mongodb-connection-string` with your MongoDB connection string.
  - Replace `your-port` with your port number.

  4. Run the application:


 ### For Frontend
 
   1. Navigate to the frontend directory:

    ```bash
    cd frontend
    ```


    
## Routes


### User Routes

| Method | Endpoint             | Description              | 
| ------ | ---------------------| ------------------------ | 
| GET   | `/user/get`     |      Check the user present in database   |
| POST   | `/user/post`        | Add the user in database  |
| GET   | `/user/:id`       | Getting data of user by id        | 





### Post Routes

| Method | Endpoint             | Description              |
| ------ | ---------------------| ------------------------ | 
| POST   | `post//bulkadd`     | Add the Post data     |
| GET   | `post/checkUserId/:userId`       | 	Check the user post is available |

    


