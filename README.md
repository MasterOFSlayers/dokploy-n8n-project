# Dokploy + n8n Project

## What is this?
This project deploys **n8n** (workflow automation) using **Docker**.

## Stack
- **Dokploy** - Self-hosted PaaS deployment platform
- **n8n** - Visual workflow automation tool
- **Docker** - Containerization

## How to run n8n
`docker run -d --name n8n -p 5678:5678 -v n8n_data:/home/node/.n8n n8nio/n8n`

Then open: http://localhost:5678

## Demo Workflow
A webhook-based Joke Bot:
1. Receives a GET request at /webhook/get-joke
2. Fetches a random joke from a public API
3. Returns the joke as JSON
