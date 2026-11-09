# My_StudyAssistant
# 🤖 AI-Powered Study Assistant

An interactive, AI-powered Study Assistant built using **Python, Google Gemini API, and Gradio**. It helps students understand complex concepts through personalized explanations using two different AI personalities: **Friendly** and **Academic**.

The application uses Google's Gemini model to generate intelligent, context-aware responses based on the user's questions and selected learning style.

## 🚀 Live Demo

**Try the application here:** [Study Assistant – Live Demo](https://my-study-assistant-yajd.onrender.com/)

## ✨ Features

- **AI-Powered Responses:** Uses Google Gemini API to generate intelligent and context-aware explanations.
- **Two AI Personalities:** Choose between Friendly and Academic learning styles.
- **Friendly Mode:** Explains complex concepts in simple, beginner-friendly language using real-world examples and analogies.
- **Academic Mode:** Provides detailed, structured, and professional explanations using formal terminology.
- **Interactive Interface:** Simple and user-friendly web interface built with Gradio.
- **Dynamic Responses:** Generates answers based on user questions and selected personality.
- **Cloud Deployment:** Deployed on Render for online accessibility.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Google Gemini API | AI-powered response generation |
| Gemini 3.5 Flash Lite | Language model |
| Gradio | Interactive web interface |
| Google GenAI SDK | Gemini API integration |
| Render | Cloud deployment |
| Git & GitHub | Version control and project hosting |

## 🧠 How It Works

The application allows users to enter a question and select their preferred AI personality.

1. The user enters a question in the Gradio interface.
2. The user selects either Friendly or Academic personality.
3. The application retrieves the corresponding system instruction from the personalities dictionary.
4. The selected instruction is passed to the Gemini API through `GenerateContentConfig`.
5. Gemini generates a response based on the question and selected personality.
6. The generated response is displayed in the Gradio interface.

## 🎭 Available AI Personalities

### 1. Friendly Personality

- Uses simple and understandable language.
- Explains complex concepts through everyday examples.
- Provides beginner-friendly explanations.
- Encourages interactive learning with follow-up questions.

### 2. Academic Personality

- Uses formal and professional language.
- Provides structured and detailed explanations.
- Uses technical terminology and relevant examples.
- Focuses on conceptual understanding.

## 📂 Project Structure

```text
Study-Assistant/
│
├── app.py              # Main application
├── requirements.txt   # Python dependencies
├── .env               # API key (not committed)
├── .gitignore         # Ignored files
└── README.md          # Project documentation
```

## ⚙️ Installation and Setup

### Prerequisites

- Python 3.9 or higher
- Google Gemini API key
- Git installed on your system

### Step 1: Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Navigate into the project directory:

```bash
cd Study-Assistant
```

### Step 2: Create a Virtual Environment

```bash
python -m venv venv
```

Activate it:

**macOS/Linux:**
```bash
source venv/bin/activate
```

**Windows:**
```bash
venv\Scripts\activate
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Configure the Gemini API Key

Create a `.env` file in the project directory:

```env
GEMINI_API_KEY=your_actual_gemini_api_key
```

For local development, load the environment variable using `python-dotenv`, or export it directly in your terminal.

**Important:** Never commit your API key or `.env` file to GitHub.

### Step 5: Run the Application

```bash
python app.py
```

Open the local Gradio URL displayed in your terminal.

## 📦 Requirements

Add the following dependencies to `requirements.txt`:

```text
gradio
google-genai
python-dotenv
```

## ☁️ Deployment on Render

This project is deployed using Render.

To deploy your own instance:

1. Push the project to a GitHub repository.
2. Sign in to [Render](https://render.com/).
3. Create a new Web Service.
4. Connect your GitHub repository.
5. Configure the deployment settings:

| Setting | Value |
|---|---|
| Environment | Python |
| Build Command | `pip install -r requirements.txt` |
| Start Command | `python app.py` |

6. Add the following environment variable in Render:

```text
GEMINI_API_KEY = your_actual_gemini_api_key
```

7. Deploy the application and access your live URL.

## 🔐 Environment Variables

| Variable | Description |
|---|---|
| `GEMINI_API_KEY` | Google Gemini API authentication key |
| `PORT` | Port provided by Render |

## 🎯 Project Objectives

- Explore practical applications of Generative AI.
- Understand how Large Language Models respond to system instructions.
- Implement persona-based AI interactions.
- Integrate Google Gemini API with Python applications.
- Build interactive AI applications using Gradio.
- Deploy AI applications to cloud platforms.

## 🔮 Future Enhancements

- Add more AI personalities, such as Mentor, Interviewer, and Exam Tutor.
- Integrate voice-based question and answer functionality.
- Add conversation history and chat memory.
- Include subject-specific learning modes.
- Add quiz generation and personalized study plans.
- Support multiple languages.

## 👨‍💻 Author

**Afsar Basha**

Aspiring Software Developer | AI Enthusiast | Python Developer

- **GitHub:** https://github.com/Apsar-0089
- **Portfolio:** https://ai-portfolio-chatbot-backend.vercel.app/

## ⭐ Support

If you find this project useful, consider giving this repository a ⭐ on GitHub.

Your feedback and suggestions are always welcome!

---

*Built with Python, Google Gemini API, and Gradio.*
