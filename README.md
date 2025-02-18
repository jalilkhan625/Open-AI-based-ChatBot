# Chatbot with OpenAI API

This project is a simple chatbot interface built with HTML, JavaScript, and Bootstrap for the frontend, and Node.js with Express for the backend. The chatbot interacts with users and provides responses using OpenAI's GPT-3.5 API.

## Features
- **Interactive Chatbox:** A floating chat widget that can be toggled open or closed.
- **User & Bot Messages:** Displays user messages in blue and bot responses in gray.
- **Express Backend:** A simple API that forwards user messages to OpenAI's GPT-3.5 and returns responses.
- **CORS Support:** Ensures cross-origin requests can be handled.
- **Environment Variables:** Uses `dotenv` to securely manage the OpenAI API key.

## Technologies Used
- **Frontend:** HTML, CSS (Bootstrap 5), JavaScript
- **Backend:** Node.js, Express.js
- **API Integration:** OpenAI GPT-3.5 via `axios`

## Setup Instructions

### 1. Clone the Repository
```sh
git clone https://github.com/yourusername/chatbot.git
cd chatbot
```

### 2. Install Dependencies
```sh
npm install
```

### 3. Configure Environment Variables
Create a `.env` file in the root directory and add:
```
OPENAI_API_KEY=your_openai_api_key
PORT=5000
```

### 4. Start the Server
```sh
node server.js
```
The server will run at `http://localhost:5000`.

### 5. Open `index.html`
Simply open the `index.html` file in a browser to interact with the chatbot.

## API Endpoints
- **POST /chat**  
  - Sends a message to OpenAI and returns a response.
  - Request body:
    ```json
    { "message": "Hello, chatbot!" }
    ```
  - Response:
    ```json
    { "reply": "Hello! How can I assist you today?" }
    ```

## Future Enhancements
- Support for conversation history.
- Improved UI with animations.
- Deployment to cloud platforms (Heroku, Vercel, etc.).

## License
This project is open-source and available under the MIT License.
