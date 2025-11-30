# 🧳 Real-time Travel Planner

A simple **Streamlit app** powered by **Google ADK + Gemini** that helps travelers decide what to pack based on the weather at their destination.  
This demo uses a **mock weather API** (instead of MCP) to simulate realistic conditions and generate packing recommendations.

---

##  Features
- 🌍 Enter any city and get **personalized packing suggestions**
- ⛅ Mock weather tool simulates realistic conditions (snowy, rainy, sunny, clear)
- 🎒 Packing list tailored to the weather (e.g., raincoat for rainy London, sunscreen for sunny Miami)
- ⚡ Built with **Google ADK**, **Gemini LLM**, and **Streamlit**
- 🔄 Retry logic for robust API calls

---

## Project Structure
travel_planner/ 


│── app.py              # Main Streamlit app 


│── .env                # Environment variables (GOOGLE_API_KEY) 


│── requirements.txt    # Python dependencies 


│── README.md           # Project documentation

---

##  Installation

### 1. Clone the repository
```bash
git clone https://github.com/Karthik-1221/-Real-time-Travel-Planner.git
cd travel-planner
```
2. Create a virtual environment

python -m venv venv


source venv/bin/activate   # Mac/Linux


venv\Scripts\activate      # Windows



3. Install dependencies


pip install -r requirements.txt


5. Set up environment variables

Create a .env file in the project root

GOOGLE_API_KEY=your_google_api_key_here


 Usage
Run the Streamlit app:

streamlit run app.py

Open the app in your browser at:
http://localhost:8501

Example
- Input: Helsinki
- Output:
Weather: snowy (-5°C)
Packing List:
- Heavy coat
- Gloves
- Hat
- Thermal layers

Dependencies
- Streamlit – UI framework
- python-dotenv – Environment variable management
- google-adk – Google Agent Development Kit
- Gemini – LLM model

 Notes
- This demo uses mock weather data for simplicity.
- Replace get_current_weather with a real weather API (e.g., OpenWeatherMap) for production use.
- The agent strictly follows the process:
- Get weather for the city
- Generate packing list based on condition
- Return concise response

 License
MIT License – feel free to use and modify.

 Acknowledgements
- Google ADK + Gemini for LLM integration
- Streamlit for interactive UI

---









