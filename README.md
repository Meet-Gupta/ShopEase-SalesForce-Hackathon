# ShopEase AI Customer Support System

A modern AI-powered customer support system built with Node.js, React, and OpenAI's GPT model. This system provides intelligent customer service automation with features like intent detection, natural language processing, and multi-language support.

## Features

- 🤖 AI-powered customer support using OpenAI's GPT model
- 🌐 Multi-language support with LibreTranslate integration
- 💬 Real-time chat interface using Socket.IO
- 📊 Analytics and conversation tracking
- 🔄 Automatic intent detection and response generation
- 📱 Responsive web interface
- 🐳 Docker containerization for easy deployment

## Tech Stack

- **Backend**: Node.js, Express.js
- **Frontend**: React.js
- **Database**: MongoDB
- **AI/ML**: OpenAI GPT API
- **Translation**: LibreTranslate
- **Real-time Communication**: Socket.IO
- **Containerization**: Docker & Docker Compose

## Prerequisites

- Node.js (v14 or higher)
- Docker and Docker Compose
- MongoDB (included in Docker setup)
- OpenAI API key
- Git

## Environment Variables

Create a `.env` file in the server directory with the following variables:

```env
OPENAI_API_KEY=your_openai_api_key
OPENAI_MODEL=gpt-3.5-turbo
MONGODB_URI=mongodb://mongodb:27017/shopease
PORT=3000
NODE_ENV=development
```

## Getting Started

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd shopease
   ```

2. Start the application using Docker Compose:
   ```bash
   docker-compose up --build
   ```

3. Access the application:
   - Frontend: http://localhost:3001
   - Backend API: http://localhost:3000
   - MongoDB: mongodb://localhost:27017
   - LibreTranslate: http://localhost:5000

## Development

### Backend Development

```bash
cd server
npm install
npm run dev
```

### Frontend Development

```bash
cd client
npm install
npm start
```

## API Endpoints

### AI Service Endpoints

- `POST /api/ai/process` - Process a customer query
- `POST /api/ai/detect-intent` - Detect the intent of a query
- `POST /api/ai/generate-response` - Generate a response for a specific intent
- `POST /api/ai/summarize` - Summarize a conversation

### Analytics Endpoints

- `GET /api/analytics/top-issues` - Get top customer issues

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- OpenAI for providing the GPT API
- LibreTranslate for translation services
- MongoDB for the database
- Docker for containerization 