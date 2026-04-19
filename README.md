# AutoSales - Car Sales Website

A simple car sales website built with Node.js and Docker.

## Features
- Responsive design
- Featured car listings
- Modern UI with gradient backgrounds
- Health check endpoint for Docker

## Files
- `index.html` - Frontend HTML with CSS
- `server.js` - Node.js HTTP server
- `Dockerfile` - Docker containerization
- `package.json` - Project metadata

## Local Development

### Run without Docker
```bash
node server.js
```
Then visit `http://localhost:3000`

## Docker Setup

### Build Docker Image
```bash
docker build -t autosales-app .
```

### Run Docker Container
```bash
docker run -p 3000:3000 autosales-app
```

Then visit `http://localhost:3000`

### Check Container Health
```bash
docker ps
```

## Environment Variables
- `PORT` - Server port (default: 3000)

## API Endpoints
- `GET /` - Serves the main website
- `GET /health` - Health check endpoint (returns JSON)
- `GET /index.html` - Direct access to HTML file
