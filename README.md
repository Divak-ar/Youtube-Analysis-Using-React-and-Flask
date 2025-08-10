# YouTube Analytics Dashboard

Full-stack application for analyzing YouTube channels, videos, and trending content using YouTube Data API v3.

## Features

- Channel analytics with subscriber metrics and content distribution
- Video analysis with engagement rates and sentiment scoring
- Regional trending data with velocity tracking
- Interactive charts and real-time visualizations

## Prerequisites

- Node.js 16+
- Python 3.8+
- YouTube Data API v3 key

## Setup

### Backend
### Backend

```bash
cd backend
pip install -r requirements.txt
```

Create `.env` file:
```env
YOUTUBE_API_KEY=your_api_key
SECRET_KEY=your_secret_key
```

Start server:
```bash
python app.py
```

### Frontend

```bash
cd frontend
npm install
npm start
```

## API Endpoints

- `GET /api/health` - Health check
- `GET /api/channel/<input>` - Channel analysis
- `GET /api/video/<id>` - Video analysis  
- `GET /api/trending/<region>` - Regional trending

## Technology Stack

**Backend**: Flask, Python, YouTube Data API v3
**Frontend**: React, Recharts, Tailwind CSS

## Usage

Analyze channels using:
- Channel URLs: `https://youtube.com/@username`
- Channel IDs: `UCX6OQ3DkcsbYNE6H8uQQuVA`
- Usernames: `@MrBeast`

## Development

Test backend connection:
```bash
cd backend && python test_api.py
```

Health check:
```bash
curl http://localhost:5000/api/health
```
