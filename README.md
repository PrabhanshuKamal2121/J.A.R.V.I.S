# J.A.R.V.I.S - AI-Powered Personal Assistant

![image alt](https://github.com/PrabhanshuKamal2121/J.A.R.V.I.S/blob/d5f807e642cb0ae5f37825f4fbc020fc8d1b882a/Jarvis.png)
> A sophisticated n8n workflow for seamless voice, text, and image task automation.

![n8n](https://img.shields.io/badge/n8n-FF813F?style=for-the-badge&logo=n8n&logoColor=white)
![Telegram](https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)
![OpenRouter](https://img.shields.io/badge/OpenRouter-4B0082?style=for-the-badge&logo=ai&logoColor=white)
![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
---

## 🛠️ Tech Stack

| Layer                | Tools & Services                                       |
|----------------------|-------------------------------------------------------|
| **Core**             | n8n, JavaScript                                       |
| **Messaging**        | Telegram API                                          |
| **AI Models**        | OpenRouter (DeepSeek, MistralAI)                      |
| **Speech**           | Whisper (STT), Custom TTS (J.A.R.V.I.S. voice)        |
| **Image Generation** | Black Forest Labs' FLUX.1                             |
| **Email**            | Gmail API                                             |
| **Web Search**       | Custom HTTP-based search service                       |

---

## ✨ Features

- **Voice Interaction**: Transcribes voice inputs and responds with J.A.R.V.I.S.-style audio.  
- **Image Creation**: Generates hyper-realistic images from detailed prompts.  
- **Text Commands**: Processes text for tasks, queries, or social media posts.  
- **Email Management**: Sends, replies, and organizes Gmail messages.  
- **LinkedIn Integration**: Crafts and posts engaging content with data-driven insights.  
- **Real-Time Search**: Fetches current information via web search.  
- **J.A.R.V.I.S. Persona**: Polished British butler tone with subtle, witty humor.  
- **Context Memory**: Retains conversation history for personalized responses.

---

## 💡 About the Project

J.A.R.V.I.S. (Just A Rather Very Intelligent System) is an advanced AI assistant built on n8n, inspired by Tony Stark’s iconic companion. It integrates Telegram, AI models, and external APIs to handle diverse tasks like voice responses, image generation, and email management. With a refined British butler persona, it delivers professional, engaging interactions.

- **Intuitive Workflow**: Processes text, voice, or image inputs via Telegram with clear routing.  
- **AI-Powered**: Leverages DeepSeek and MistralAI for intelligent responses and task execution.  
- **Visual & Audio Output**: Creates vivid images and J.A.R.V.I.S.-style voice replies.  
- **Custom Styling**: Formal tone with dry wit, ensuring a polished user experience.  
- **Scalable Design**: Modular n8n nodes for easy expansion and maintenance.

---

## 🔍 How It Works

1. **Input Trigger**: Telegram messages (text, voice, or photo) initiate the workflow.  
2. **Input Routing**: Switch nodes categorize inputs for appropriate processing.  
3. **Voice Handling**: Whisper transcribes voice; TTS generates J.A.R.V.I.S.-style audio.  
4. **Image Generation**: Prompts with "image" trigger FLUX.1 for hyper-realistic visuals.  
5. **Text Processing**: AI agents handle queries, LinkedIn posts, or email tasks.  
6. **Output Delivery**: Responses are sent as text, audio, or images via Telegram.  
7. **Task Automation**: Gmail and LinkedIn nodes execute user-requested actions.

---

## 🏗️ Architecture

```bash
J.A.R.V.I.S/
├── J.A.R.V.I.S.json   # n8n workflow configuration
├── jarvis.mp3         # Reference audio for TTS voice cloning
├── README.md          # Project documentation (this file)
```

- **Input Layer**: Telegram Trigger and Switch nodes for input classification.  
- **Processing Layer**: AI agents with OpenRouter models, web search, and Gmail tools.  
- **Transformation**: JavaScript code nodes for data cleaning and formatting.  
- **Output Layer**: Telegram nodes for text/audio/image; TTS for voice responses.  
- **Memory**: Context buffer for conversation continuity.

---

## 📈 Model & Data

- **Models**: DeepSeek R1, MistralAI 7B (OpenRouter); FLUX.1 for images.  
- **Speech**: Whisper for speech-to-text; custom TTS with J.A.R.V.I.S. voice cloning.  
- **Data**: JSON data flow; base64 for images; multipart-form-data for audio.  
- **Memory**: 100-message context window for personalized interactions.

---

## 🚀 Quick Start

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-repo/jarvis.git
   cd jarvis
   ```
2. **Install n8n**:
   - Set up n8n locally or on a hosted instance.  
   - Import `J.A.R.V.I.S.json` into n8n.  
3. **Configure Credentials**:
   - Add Telegram API token.
   - Set up OpenRouter API for AI models.
   - Configure Gmail OAuth2 for email tasks.
   - Add Together AI credentials for image generation. 
4. **Run Services**:
   - Start Whisper (`http://host.docker.internal:8000/whisper`).  
   - Start TTS (`http://host.docker.internal:8004/tts`).  
   - Ensure FLUX.1 API access (`https://api.together.xyz/v1/images/generations`).  
5. **Activate Workflow**:
   - Enable the workflow in n8n.  
   - Test with a Telegram message (text, voice, or image).  

---

## 📬 Contact

Made by **PrabhanshuKamal**  
📧 Email: [prabhanshukamal2121@gmail.com](mailto:prabhanshukamal2121@gmail.com)  
🌐 GitHub: [github.com/PrabhanshuKamal2121](https://github.com/PrabhanshuKamal2121)  

---

> 🚨 **DISCLAIMER**: This project is for educational purposes. Ensure compliance with API terms and data privacy regulations.
