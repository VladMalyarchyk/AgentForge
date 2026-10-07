# Backend Development

## Running the API Locally

To run the FastAPI backend:
1. Install dependencies: `pip install -r apps/api/requirements.txt`
2. Start the server: `uvicorn apps/api/app/main:app --host 0.0.0.0 --port 8000`
3. Verify health endpoint: `curl http://localhost:8000/health`