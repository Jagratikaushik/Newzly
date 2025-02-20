# Newsly

## Overview
This project is **Newsly**, a news summarizer that fetches and processes news based on user-selected durations and topics. It consists of a **Next.js frontend** and a **FastAPI backend** integrated with the Mira API for news processing.

## Installation and Setup
Follow these steps to set up and run the project:

### 1. Clone the Repository
```sh
git clone <your-repo-url>
cd <your-repo-folder>
```

### 2. Install Dependencies
```sh
npm install
```

### 3. Configure the Backend
- Navigate to the backend folder:
  ```sh
  cd backend
  ```
- Create a `.env` file and add your Mira API key:
  ```sh
  echo "MIRA_API_KEY=your_mira_api_key" > .env
  ```
- To obtain a Mira API key:
  1. Go to [Mira Network](https://flows.mira.network/).
  2. Create an account.
  3. Generate an API key and add it to the `.env` file.

### 4. Install Backend Dependencies
```sh
pip install -r requirements.txt
```

### 5. Start the Backend Server
```sh
uvicorn main:app --reload
```

### 6. Start the Frontend
- Open a **new terminal**.
- Navigate back to the main project folder:
  ```sh
  cd ..
  ```
- Run the frontend:
  ```sh
  npm run dev
  ```

## Usage
Once the frontend and backend are running, open your browser and navigate to `http://localhost:3000` to interact with Newsly.

## Features
- Interactive UI
- Multi-language support
- Monthly, weekly, and daily news
- Option to add news of your favorite topic
- Caching is implemented

## Backend Requirements
Create a `requirements.txt` file in the backend folder with the following dependencies:
```txt
fastapi
pydantic
dotenv
mira-sdk
uvicorn
httpx
```
Install them using:
```sh
pip install -r requirements.txt
```

