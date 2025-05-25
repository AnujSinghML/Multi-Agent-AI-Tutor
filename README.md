# Multi-Agent AI Tutor

A sophisticated AI tutoring system that uses multiple specialized agents to provide comprehensive assistance in mathematics, physics, and chemistry. The system leverages the Gemini API for natural language understanding and includes various tools for calculations and problem-solving.

## Architecture

The system consists of the following components:

### Main Components

1. **Tutor Agent**: The main orchestrator that receives user queries, identifies the subject, and delegates to appropriate sub-agents.

2. **Subject-Specific Agents**:
   - **Math Agent**: Handles mathematical queries using calculator and equation solver tools
   - **Physics Agent**: Manages physics questions with constant lookup and unit converter tools
   - **Chemistry Agent**: Processes chemistry queries with periodic table and stoichiometry tools

3. **Tools**:
   - **Calculator**: Basic and advanced mathematical calculations
   - **Constant Lookup**: Provides physical constants and their descriptions

### Technical Stack

- **Backend**: FastAPI
- **Frontend**: HTML, TailwindCSS
- **AI**: Google Gemini API
- **Deployment**: Vercel

## Setup Instructions

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd ai-tutor
   ```

2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Create a `.env` file in the root directory with your Gemini API key:
   ```
   GEMINI_API_KEY=your_api_key_here
   DEBUG=False
   ```

5. Run the development server:
   ```bash
   uvicorn app.main:app --reload
   ```

## Deployment

The application is deployed on Vercel. The deployment process is automated through GitHub integration.
[link](link)

## API Endpoints

- `GET /`: Web interface
- `POST /api/query`: Process user queries
- `GET /api/health`: Health check endpoint

## Features

- Natural language processing for query understanding
- Subject-specific agents with specialized tools
- Real-time calculations and problem-solving
- Modern, responsive web interface
- Error handling and graceful degradation


## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.



