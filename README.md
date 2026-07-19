🧠 Neuro-Adaptive Multi-Agent System

📌 Project Overview
The Neuro-Adaptive Multi-Agent System is an advanced AI framework inspired by human neuroplasticity. It simulates how humans adapt when one sensory capability is limited by introducing specialized AI agents that compensate for missing modalities.

The system integrates multiple data modalities:

📝 Text
🔊 Audio
🖼️ Image
and dynamically routes reasoning through Normal, Blind, Mute, and LessHearable agents.

Applications
Assistive AI Systems
Inclusive Human–AI Interaction
Cognitive Intelligence Research
Multimodal Reasoning Visualization
Neuro-Adaptive Artificial Intelligence
🧠 Neuroplasticity-Inspired Design
The system is inspired by the way the human brain adapts when one sensory channel becomes unavailable.

Agent Adaptation Model
Condition	Compensation Mechanism
Blindness	Audio + Text
Muteness	Image + Text
Hearing Impairment	Memory Summarization
Normal Perception	All Modalities
Specialized agents collaborate, exchange feedback, and store compact memories to improve future reasoning and decision-making.

🤖 Agents in the System
Agent	Description
NormalPersonAgent	Full multimodal reasoning using image, audio, and text
BlindPersonAgent	Audio and text-based reasoning without visual input
MutePersonAgent	Image and text-based reasoning without audio input
LessHearableAgent	Memory-enhanced reasoning and hearing compensation
Note: LessHearableAgent operates internally and cannot be directly selected by users.

✨ Key Features
Multimodal Processing
Supports:

Text Understanding
Audio Understanding
Image Understanding
Neuro-Adaptive Reasoning
Automatically adapts reasoning when a modality is unavailable.

Multi-Agent Collaboration
Agents communicate and share contextual information to improve output quality.

Memory-Augmented Intelligence
Stores important observations and summaries to improve future reasoning.

3D Visualization
Provides interactive visualizations for:

Input embeddings
Agent reasoning embeddings
Cognitive state transitions
Gemini-Powered Reasoning
Uses Google's Gemini model for advanced cognitive reasoning and analysis.

📂 Project Structure
project-root/
│
├── agents/
│   ├── normal_agent.py
│   ├── blind_agent.py
│   ├── mute_agent.py
│   ├── memory_agent.py
│   └── agent_manager.py
│
├── models/
│   ├── encoders.py
│   ├── image_captioning.py
│   ├── speech_to_text.py
│   ├── img_encoder_15d.pt
│   ├── aud_encoder_15d.pt
│   ├── txt_encoder_15d.pt
│   └── vosk-model-small-en-us-0.15/
│
├── processors/
│   ├── image_processor.py
│   ├── audio_processor.py
│   └── text_processor.py
│
├── reasoning/
│   ├── cognitive_analysis.py
│   ├── gemini_flash_reasoner.py
│   └── extended_vision.py
│
├── memory/
│   ├── memory_manager.py
│   └── retrieval.py
│
├── static/
│   ├── audio/
│   └── plots/
│
├── templates/
│   ├── landing.html
│   ├── index2.html
│   ├── visualize.html
│   └── reasoning_visual.html
│
├── memory_store/
│   └── working_memory.json
│
├── config/
│   └── settings.py
│
├── app.py
├── main8.py
├── .env
├── requirements.txt
└── README.md
⚙️ Environment Setup
Create Virtual Environment
python -m venv venv
Activate Virtual Environment
Windows
venv\Scripts\activate
Linux / macOS
source venv/bin/activate
📦 Install Dependencies
Install from requirements.txt
pip install -r requirements.txt
Manual Installation
pip install torch torchvision torchaudio
pip install sentence-transformers transformers
pip install flask python-dotenv
pip install librosa pydub webrtcvad
pip install vosk deepface
pip install google-generativeai
pip install scikit-learn matplotlib numpy pillow
pip install pyttsx3
🔐 Configuration
Gemini API Key
Create a .env file in the project root directory:

GEMINI_API_KEY=your_google_gemini_api_key
If the API key is not provided:

Gemini reasoning is skipped
Internal fallback reasoning is used
📥 Required Models
Place the following trained models inside the models/ directory:

img_encoder_15d.pt
aud_encoder_15d.pt
txt_encoder_15d.pt
Speech Recognition Model
Download the VOSK model and place it here:

models/vosk-model-small-en-us-0.15/
▶️ Running the Project
Option 1: Terminal Mode
Run the complete neuro-adaptive reasoning pipeline:

python main8.py
This mode:

Loads all AI models
Processes multimodal inputs
Executes reasoning agents
Displays results in the terminal
Option 2: Web Application (Recommended)
Launch the Flask application:

python app.py
Open:

http://127.0.0.1:5000/
🌐 Web Interface Workflow
Step 1
Open the application homepage.

Step 2
Click:

Launch Multi-Agent System
Step 3
Upload any combination of:

Text
Image
Audio
Step 4
Select one of the available agents:

Normal Agent
Blind Agent
Mute Agent
Step 5
View generated reasoning and visualizations.

📊 Visualization Features
3D Input Modality Space
Displays embedding relationships among:

Text Features
Image Features
Audio Features
3D Reasoning Embedding Space
Displays:

Agent reasoning paths
Cognitive transitions
Decision clusters
Memory influence
🧠 Memory Architecture
The system maintains a lightweight working memory that stores:

Important observations
Agent summaries
Contextual knowledge
Reasoning traces
This memory improves future reasoning quality and agent collaboration.

📌 Agent Input Rules
Agent	Required Input
Normal Agent	Any modality
Blind Agent	Audio input
Mute Agent	Image input
🔄 Reset Memory
To clear stored memory:

Delete:
memory_store/working_memory.json
A new memory file will automatically be created during the next execution.

🏗️ System Workflow
User Input
      │
      ▼
Input Processors
(Image / Audio / Text)
      │
      ▼
Feature Encoders
      │
      ▼
Agent Manager
      │
 ┌────┼────┐
 ▼    ▼    ▼
Normal Blind Mute
Agent  Agent Agent
      │
      ▼
Memory Agent
      │
      ▼
Gemini Reasoning
      │
      ▼
Final Response
      │
      ▼
3D Visualization
🚀 Future Enhancements
AI Improvements
Long-Term Memory Systems
Reinforcement Learning Agents
Neuro-Symbolic Reasoning
Self-Adaptive Agent Architectures
Interface Enhancements
Voice-Based Interaction
Real-Time Agent Monitoring
Interactive Knowledge Graphs
Advanced Visualization Dashboards
Research Extensions
Artificial Neuroplasticity Experiments
Cognitive Workload Modeling
Human Perception Simulation
Adaptive Sensory Compensation Systems
🏁 Conclusion
The Neuro-Adaptive Multi-Agent System demonstrates how principles inspired by human neuroplasticity can be incorporated into modern AI systems.

By combining:

Cognitive Science
Artificial Intelligence
Multimodal Learning
Agent-Based Architectures
Memory-Augmented Reasoning
the project creates an adaptive, inclusive, and intelligent framework capable of compensating for missing sensory information through collaborative reasoning.

👨‍💻 Author
Abhishek Srivatsav

Computer Science Engineering Student

📧 Email: abhisheksrivatsav60@gmail.com

🐙 GitHub: https://github.com/abhishek-srivatsav

📜 License
This project is intended for:

Educational Purposes
Academic Research
Experimental AI Development
Feel free to modify and extend the project for learning and research purposes.
