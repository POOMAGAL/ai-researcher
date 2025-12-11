# ai-researcher
🚀 Complete Setup Guide - GROQ LLM API (FREE)
✅ What You'll Build
A multi-agent AI research system that:

Uses GROQ (completely FREE)
Uses Tavily Search (FREE tier - 1000 queries/month)
Has 5 specialized AI agents working together
Produces comprehensive research reports

Total Cost: $0.00 🎉

📋 Prerequisites

Python 3.9 or higher
Internet connection
10 minutes


🔑 Step 1: Get API Keys (Both FREE!)
GROQ API Key (FREE Forever)

Go to: (https://console.groq.com/keys)
Sign in with your Google account
Click "Create API Key"
Click "Create API key in new project"
Copy the key (starts with gsk_...)

Free Tier:
Completely FREE forever! 🎉

Tavily API Key (FREE Tier)

Go to: https://tavily.com/
Sign up with email
Verify your email
Copy your API key from dashboard (starts with tvly-...)

Free Tier:

1,000 searches per month
Perfect for hackathons!


💻 Step 2: Setup Project
Create Project Directory
bash# Create and navigate to project folder
mkdir ai-researcher
cd ai-researcher
Create Virtual Environment
bash# Create virtual environment
python -m venv venv

# Activate it
# On Mac/Linux:
source venv/bin/activate

# On Windows:
venv\Scripts\activate

# You should see (venv) in your terminal now

📦 Step 3: Install Dependencies
Create requirements.txt
Create a file named requirements.txt with this content:
txtstreamlit==1.31.0
langchain==0.1.20
langchain-google-genai==1.0.1
langchain-core==0.1.52
langgraph==0.0.40
google-generativeai==0.3.2
tavily-python==0.3.3
python-dotenv==1.0.0
Install Packages
bashpip install -r requirements.txt
This will take 2-3 minutes. You'll see packages being installed.

🔐 Step 4: Configure API Keys
Create .env File
Create a file named .env in your project folder:
bash# On Mac/Linux:
cat > .env << 'EOF'
GOOGLE_API_KEY=your_gemini_key_here
TAVILY_API_KEY=your_tavily_key_here
EOF

# On Windows (or manually create the file):
# Create a file named .env and add the lines above
Add Your Real Keys
Edit the .env file and replace with your actual keys:
GOOGLE_API_KEY=AIzaSyDxxxxxxxxxxxxxxxxxxxxxxxxxxx
TAVILY_API_KEY=tvly-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
Important:

Don't share these keys
Don't commit .env to git
Keep them secret!


📝 Step 5: Create app.py
Copy the complete app.py code from the artifact above into a file named app.py.
Your project structure should now look like:
ai-researcher/
├── venv/              # Virtual environment (created)
├── .env               # API keys (created)
├── requirements.txt   # Dependencies (created)
└── app.py            # Main app (create this)

🚀 Step 6: Run the App!
bashstreamlit run app.py
You should see:
  You can now view your Streamlit app in your browser.

  Local URL: http://localhost:8501
  Network URL: http://192.168.x.x:8501
Your browser will automatically open to the app! 🎉

🧪 Step 7: Test It
Test Query 1: Simple
Latest developments in quantum computing
Test Query 2: Complex
Analyze the impact of artificial intelligence on healthcare diagnostics, including recent breakthroughs, ethical considerations, and future implications
Test Query 3: Technical
Current state of renewable energy storage technology and its role in achieving net-zero emissions by 2050

🎯 How It Works
The Agent Pipeline
User Query
    ↓
Agent 1: Research Planner
    ├─ Creates search strategy
    ├─ Identifies key topics
    └─ Plans 5-7 search queries
    ↓
Agent 2: Web Search (Tavily)
    ├─ Executes searches
    ├─ Retrieves 15+ sources
    └─ Ranks by relevance
    ↓
Agent 3: Critical Analysis
    ├─ Validates findings
    ├─ Identifies contradictions
    └─ Assesses data quality
    ↓
Agent 4: Insight Generator
    ├─ Synthesizes patterns
    ├─ Identifies trends
    └─ Creates recommendations
    ↓
Agent 5: Report Builder
    ├─ Compiles executive summary
    ├─ Organizes findings
    └─ Formats final report
    ↓
Final Research Report
Technologies Used

GROQ: Fast, free LLM for agent reasoning
Tavily Search: AI-optimized web search
LangGraph: Agent orchestration framework
Streamlit: Web UI framework
LangChain: LLM integration toolkit
