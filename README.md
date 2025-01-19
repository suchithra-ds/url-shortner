# URL Shortener

This project is a simple URL shortener service that allows users to convert long URLs into shorter, more manageable links. The application also leverages Redis for session management and caching.

## Features

- Shorten long URLs into concise links.
- Redirect users from short URLs to the original long URLs.
- Supports user authentication and session management.
- Utilizes Redis for performance optimization and caching.

## Prerequisites

Before running this application, ensure you have the following installed:

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)
- Redis (Ensure Redis is running locally or remotely)

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/suchithra-ds/url-shortner.git
   ```

2. **Navigate to the project directory:**

   ```bash
   cd url-shortner
   ```

3. **Install the dependencies:**

   ```bash
   npm install
   ```
4. **Set up the environment variables:**

   Create a .env file in the root of the project and add the following configuration:
   BASE_URL=http://localhost:5000/api/shorten
   BASE_URL1=http://localhost:5000
   REDIRECT_URI=http://localhost:5000/auth/callback
   PORT=5000
   CLIENT_ID=your_client_id
   CLIENT_SECRET=your_client_secret
   SESSION_SECRET=your_session_secret
   MONGO_URI=your_mongo_connection_string
   REDIS_URI=redis://localhost:6379 or your_redis_connection_string
Replace the placeholders (CLIENT_ID, CLIENT_SECRET, SESSION_SECRET, MONGO_URI, REDIS_URI) with your actual configuration values.

## Usage

1. **Start the server:**

   ```bash
   node server.js
   ```

2. **Access the application:**

   Open your browser and navigate to `http://localhost:5000`.

## Contributing

Contributions are welcome! Please fork this repository and submit a pull request for any enhancements or bug fixes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details. 
