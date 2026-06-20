# Orbit

Orbit is a task management app built with the MERN stack. It uses Redis for caching and Elasticsearch for fast todo search.

## Tech Stack

* React
* Node.js
* Express
* MongoDB
* Redis
* Elasticsearch

## Features

* Create tasks
* Delete tasks
* Full-text search with Elasticsearch
* Cached responses with Redis

## Getting Started

### Prerequisites

* Node.js
* MongoDB
* Redis
* Elasticsearch

### Installation

```bash
git clone https://github.com/Muhsin-42/Orbit.git
cd Orbit
npm install
```

### Environment Variables

Server (`.env`)

```env
MONGODB_URI=
PORT=
CLOUD_ID=
ELASTIC_USERNAME=
ELASTIC_PASSWORD=
```

Client (`client/.env`)

```env
VITE_SERVER_BASE_URL=http://localhost:8000
```

### Run

Server:

```bash
npm run dev
```

Client:

```bash
cd client
npm install
npm run dev
```

## API Endpoints

| Method | Endpoint          | Description   |
| ------ | ----------------- | ------------- |
| POST   | `/`               | Create a task |
| GET    | `/`               | Get all tasks |
| DELETE | `/:id`            | Delete a task |
| GET    | `/search/:query?` | Search tasks  |
