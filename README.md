# DCoder AI Backend

Flask backend for DCoder AI chatbot that integrates with Google's Gemini AI.

## Local Development

1. Clone this repository
2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Create a `.env` file with your Gemini API key:
   ```
   GEMINI_API_KEY=your_actual_api_key_here
   ```
5. Run the application:
   ```bash
   python app.py
   ```

## Deployment

This backend is configured for deployment on Render, Railway, or similar platforms.

### Environment Variables Required:
- `GEMINI_API_KEY`: Your Google Gemini API key

### API Endpoints:
- `GET /` - API information
- `GET /health` - Health check
- `POST /ask` - Ask AI questions

## Getting Gemini API Key

1. Go to [Google AI Studio](https://aistudio.google.com/app/apikey)
2. Create a new API key
3. Copy the key and use it as environment variable

## Project Structure
dcoder-backend/
│── app.py              # Main Flask application
│── requirements.txt    # Python dependencies
│── README.md           # Project documentation
│── .gitignore          # Git ignore rules
