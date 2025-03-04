# 🌪️ Weather Disaster Management AI Agent  

## 📌 Overview  

This project introduces an **AI-driven Weather Emergency Response System** that automates **weather monitoring, disaster analysis, and emergency response planning**. Built using **LangGraph**, it enables **real-time decision-making** based on live weather data and simulated severe weather conditions.  

The system consists of **two agent graphs**:  

1. **Real-Data Agent Graph** – Monitors **real-time** weather conditions to generate automated disaster insights.  
2. **Hybrid Agent Graph** – Simulates extreme weather scenarios with dummy social monitoring data for **testing and validation**.  

---

## 🎯 Features  

- ☁️ **Real-time Weather Monitoring** – Retrieves live weather data via APIs.  
- 🔍 **Disaster Analysis** – Identifies extreme weather patterns using **AI-driven insights**.  
- 🆘 **Emergency Response Generation** – Provides recommended actions for disaster management.  
- 🚨 **Severity Assessment** – Classifies disaster intensity (mild, moderate, severe).  
- 📢 **Email Alert System** – Sends notifications to relevant authorities.  
- 🏛 **Social Media Monitoring (Hybrid Mode)** – Simulates external reports for corroboration.  
- ⚡ **Automated Workflow** – Implements state-based AI decision-making using **LangGraph**.  

---

## 🏗 Architecture  

The AI agent follows a structured workflow:

1. **Weather Data Retrieval** – Gathers weather conditions via APIs.  
2. **Social Media Monitoring (Hybrid Mode)** – Analyzes reports for corroboration.  
3. **Disaster Analysis** – Identifies potential risks using AI.  
4. **Severity Assessment** – Evaluates disaster intensity.  
5. **Response Generation** – Provides actionable emergency response plans.  
6. **Human Verification** – Ensures accuracy before sending alerts.  
7. **Email Notifications** – Sends real-time alerts to stakeholders.  
8. **Data Logging** – Stores disaster data for future analysis.  

![Weather Disaster Management AI Workflow](images/weather_disaster_workflow.png)  

---

## 🛠 Tech Stack  

- **LangGraph & LangChain** – AI workflow orchestration  
- **OpenAI GPT (LLM)** – AI-based disaster analysis  
- **Requests & APIs** – Weather data retrieval  
- **Playwright & lxml** – Web scraping for additional weather insights  
- **Gradio** – Web UI for manual interaction (optional)  
- **Email Integration** – Automatic notification dispatch  

---

## 📦 Installation  

### 1️⃣ Clone the Repository  

```bash
git clone git@github.com:devashishskumar/weather-disaster-ai-agent.git
cd weather-disaster-ai-agent

2️⃣ Set Up a Virtual Environment

python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

3️⃣ Install Dependencies

pip install -r requirements.txt

	If running in a Jupyter Notebook, install Jupyter:

4️⃣ Configure Environment Variables

Create a .env file in the project root and add necessary API keys:

OPENAI_API_KEY=your_openai_api_key
WEATHER_API_KEY=your_weather_api_key
EMAIL_SMTP_SERVER=your_email_smtp_server
EMAIL_USERNAME=your_email_username
EMAIL_PASSWORD=your_email_password

5️⃣ Run the Notebook

Launch Jupyter Notebook and open Weather_Disaster_Management_AI_AGENT.ipynb:

jupyter notebook

Run all cells to activate real-time monitoring and emergency alert generation.

	Note: This system runs best on a local machine rather than Google Colab due to API and scraping dependencies.

🖥 Running in Hybrid Mode

For testing extreme weather scenarios:
	1.	Open the notebook.
	2.	Switch to Hybrid Mode in the settings.
	3.	Run all cells to observe simulated weather emergency responses.

🛠 Dependencies

The project requires the following Python packages:

pip install langgraph langchain langchain-openai langchain-community requests
pip install python-dotenv patchright lxml schedule nest_asyncio playwright
pip install gradio smtplib

🔑 Key Learnings
	•	AI-powered decision-making enhances disaster management efficiency.
	•	Automated emergency response reduces reaction times and improves accuracy.
	•	LangGraph’s structured workflows enable real-time, scalable AI implementations.

🚀 Future Enhancements
	•	🔄 Multi-platform integration – Expand beyond weather to include earthquakes, floods, and wildfires.
	•	📊 AI-driven trend analysis – Predict disaster severity based on historical data.
	•	🌎 Global disaster response – Expand coverage to more regions and integrate with government APIs.

