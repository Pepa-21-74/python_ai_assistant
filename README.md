# Telegram AI Assistant

AI-powered Telegram assistant with a FastAPI backend, PostgreSQL database, and Retrieval-Augmented Generation (RAG).

The project is being developed as a learning project focused on backend development, machine learning, and AI application engineering.

## Features

- Telegram bot
- REST API built with FastAPI
- PostgreSQL database
- SQLAlchemy ORM and Alembic migrations
- RAG pipeline for working with external knowledge
- ML experiments and data processing
- Automated testing
- Docker-based development environment

> Some features are planned and are not implemented yet.

## Tech Stack

- Python 3.11+
- aiogram
- FastAPI
- SQLAlchemy
- PostgreSQL
- Alembic
- Pydantic Settings
- Docker
- pytest
- Jupyter Notebook
- pandas and scikit-learn

## Project Structure

```text
src/telegram_ai_assistant/  # Application source code
    api/                    # FastAPI endpoints and schemas
    bot/                    # Telegram bot handlers
    core/                   # Configuration and shared settings
    db/                     # Database models, sessions, repositories
    services/               # Business logic
    rag/                    # RAG implementation

ml/                         # ML experiments and training
data/                       # Local datasets
tests/                      # Automated tests
alembic/                    # Database migrations
docker/                     # Additional Docker configuration
scripts/                    # Development utilities
docs/                       # Project documentation
```

## Requirements

- Python 3.11 or newer
- Docker Desktop (for containerized development)
- Git

## Setup

Clone the repository:

```bash
git clone <repository-url>
cd telegram-ai-assistant
```

Create and activate a virtual environment:

Windows PowerShell:

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

Install the project and development dependencies:

```powershell
python -m pip install --upgrade pip
pip install -e ".[dev,ml]"
```

Create a local environment file:

```powershell
Copy-Item .env.example .env
```

Set the required environment variables in `.env`.

## Running with Docker

Docker configuration is planned. The `Dockerfile` and `compose.yaml` must be configured before the application can be launched through Docker Compose.

## Testing

Run tests with:

```bash
pytest
```

## Development Status

The project is under active development. Features and setup instructions will be updated as components are implemented.

## License

No license has been selected yet.
