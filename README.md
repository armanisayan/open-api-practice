# Motorsport AI Engineer Chatbot

Welcome to the **Motorsport AI Engineer**! This is a specialized RAG (Retrieval-Augmented Generation) chatbot designed to be your ultimate guide to the world of cars, motorsport, and high-performance engineering.

## Capabilities

The Motorsport AI Engineer is trained to assist with:
-   **Vehicle Tuning**: expert advice on engine mapping, suspension setups, and performance modifications.
-   **Aerodynamics**: Insights into downforce, drag reduction, and fluid dynamics for race cars.
-   **Motorsport Legends**: Detailed knowledge about icons like **Ayrton Senna**, Michael Schumacher, Lewis Hamilton, and other greats.
-   **Race Engineering**: Strategy, telemetry analysis, and track-specific setups.
-   **Automotive Tech**: Deep dives into hybrid systems, turbocharging, and chassis design.

## Features

-   **Semantic Search**: Uses Supabase and OpenAI to find the most relevant technical documents and historical records.
-   **Expert Responses**: powered by `gpt-5-nano` to deliver precise, engineering-grade answers.
-   **Context-Aware**: Retrieves specific chunks of knowledge to ground answers in fact rather than hallucination.

## Prerequisites

-   **Python 3.10+** installed on your system.
-   **Supabase Account** with a configured vector store (function `match_chunks`).
-   **OpenAI API Key** for embeddings and chat generation.

## Installation & Setup

Follow the instructions for your operating system to get started.

### 1. Clone the Repository
```bash
git clone <repository-url>
cd open-api-practice
```

### 2. Create Virtual Environment

**Windows:**
```powershell
python -m venv venv
venv\Scripts\activate
```

**MacOS / Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables
Create a file named `.env` in the root directory and add your keys:
```env
SUPABASE_URL=your_supabase_project_url
SUPABASE_SERVICE_ROLE_KEY=your_supabase_service_role_key
OPENAI_API_KEY=your_openai_api_key
```

## Usage

1.  **Start the Application**:
    ```bash
    python app.py
    ```
2.  **Open in Browser**:
    Navigate to [http://127.0.0.1:3000](http://127.0.0.1:3000)

3.  **Start Chatting**:
    Ask about "Senna's 1988 season", "how to adjust camber for better cornering", or "the principles of ground effect".

## Project Structure

-   `app.py`: The backend Flask application containing the logic for the Motorsport AI.
-   `public/`: Frontend assets (HTML/CSS/JS).
-   `requirements.txt`: Python package dependencies.
