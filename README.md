# Multi-Agent AI Tutor

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Available-green)](https://multi-agent-ai-tutor.vercel.app/)
[![Deployment](https://img.shields.io/badge/Deployed%20on-Vercel-blue)](https://multi-agent-ai-tutor.vercel.app/)

A sophisticated AI tutoring system that implements advanced agent-based architecture for intelligent subject-specific tutoring. The system leverages Google's Gemini API and incorporates principles from Google's Agent Development Kit (ADK) to create a highly capable, context-aware tutoring experience.

## Live Demo
Visit the live application at: [https://multi-agent-ai-tutor.vercel.app/](https://multi-agent-ai-tutor.vercel.app/)

## Intelligent Agent Architecture

Our system implements a sophisticated multi-agent architecture inspired by modern AI agent frameworks, featuring:

### Core Agent System

1. **Tutor Agent (Orchestrator)**
   - Implements advanced query classification and routing
   - Maintains conversation context and learning progression
   - Employs sophisticated prompt engineering for optimal responses
   - Uses reflection and self-improvement mechanisms

2. **Specialized Subject Agents**
   - **Math Agent**
     - Domain-specific knowledge representation
     - Advanced problem decomposition
     - Step-by-step solution generation
     - Mathematical reasoning validation
   
   - **Physics Agent**
     - Conceptual understanding verification
     - Physical law application
     - Unit conversion and dimensional analysis
     - Real-world application mapping
   
   - **Chemistry Agent**
     - Chemical reaction analysis
     - Molecular structure understanding
     - Stoichiometric calculations
     - Periodic trends application

### Agent Capabilities

- **Contextual Understanding**
  - Recognizes user's learning level
  - Adapts explanations accordingly

- **Tool Integration**
  - **Calculator**: Advanced mathematical computations
  - **Constant Lookup**: Scientific constants and properties

- **Learning Enhancement**
  - Interactive problem-solving
  - Error analysis and correction

## Technical Implementation

### Modern Tech Stack
- **Backend**: FastAPI (Async-first, high-performance)
- **Frontend**: HTML, TailwindCSS (Responsive, modern UI)
- **AI Engine**: Google Gemini API (State-of-the-art LLM)
- **Deployment**: Vercel (Serverless, edge-optimized)

### System Features
- Real-time query processing
- Asynchronous operation handling
- Robust error management
- Comprehensive logging and monitoring
- Scalable serverless architecture

## Setup and Development

1. **Environment Setup**
   ```bash
   git clone <repository-url>
   cd ai-tutor
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

2. **Configuration**
   Create `.env`:
   ```
   GEMINI_API_KEY=your_api_key_here
   DEBUG=False
   ENVIRONMENT=development
   ```

3. **Local Development**
   ```bash
   uvicorn app.main:app --reload
   ```

## API Architecture

- `GET /`: Interactive web interface
- `POST /api/query`: Intelligent query processing
- `GET /api/health`: System health monitoring
- `GET /api/metrics`: Performance metrics

## Advanced Features

- **Intelligent Routing**
  - Context-aware query classification
  - Dynamic agent selection
  - Multi-agent collaboration when needed

- **Learning Optimization**
  - Adaptive difficulty levels
  - Personalized learning paths
  - Concept reinforcement
  - Progress tracking

- **System Reliability**
  - Graceful error handling
  - Fallback mechanisms
  - Performance monitoring
  - Automated recovery

## Contributing

We welcome contributions! The system is designed to be extensible, allowing for:
- New subject agent integration
- Additional tool development
- UI/UX improvements
- Performance optimizations

## License

This project is open-source and available under the MIT License.



