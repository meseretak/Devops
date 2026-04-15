# HNG Stage 1 – Personal API

A minimal REST API built with Python/Flask, deployed on a Linux VPS with Nginx reverse proxy.

## How to Run Locally

```bash
git clone https://github.com/meseretak/hng-api.git
cd hng-api
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python app.py
```

API will be available at `http://localhost:5000`

## Endpoints

| Method | Endpoint  | Response |
|--------|-----------|----------|
| GET    | /         | `{"message": "API is running"}` |
| GET    | /health   | `{"message": "healthy"}` |
| GET    | /me       | `{"name": "Meseret Akalu", "email": "meseretinsa@gmail.com", "github": "https://github.com/meseretak"}` |

All endpoints return `Content-Type: application/json` and HTTP status `200`.

## Live Deployment

https://meseretwollo.duckdns.org
