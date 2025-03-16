# Todo Application

A modern Todo application built with FastAPI and PostgreSQL, designed to run on Kubernetes.

## Features

- RESTful API for managing todo items
- PostgreSQL database for persistent storage
- Kubernetes-ready with health checks and metrics
- AWS EKS deployment with GitOps using ArgoCD

## Local Development

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Run the application:
```bash
uvicorn app.main:app --reload
```

## API Documentation

Once running, visit:
- Swagger UI: http://localhost:8000/docs
- ReDoc: http://localhost:8000/redoc

## Project Structure

```
.
├── app/
│   ├── __init__.py
│   ├── main.py           # FastAPI application
│   ├── models.py         # SQLAlchemy models
│   ├── schemas.py        # Pydantic schemas
│   └── database.py       # Database configuration
├── kubernetes/           # Kubernetes manifests
├── tests/               # Test files
├── requirements.txt     # Python dependencies
└── README.md           # This file
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request 