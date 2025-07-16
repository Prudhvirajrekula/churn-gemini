
# Muffin: Gemini-Powered Customer Churn Prediction Assistant

This project is a modern, interactive customer churn prediction and explanation assistant, powered by Google Gemini LLM and Streamlit. Muffin provides actionable insights into customer churn using both machine learning models and natural language explanations.


## View Live : https://churn-gemini.streamlit.app/

## Features
- **Conversational Chatbot UI** (Streamlit)
- **Gemini 2.0 Flash LLM** for natural language answers
- **Database and CSV Integration**: Uses your data in `/data` for context
- **Customer Profile Sidebar**: Select a customer and get tailored explanations

## Setup
1. **Clone the repo**
   ```sh
   git clone https://github.com/Prudhvirajrekula/churn-gemini.git
   cd churn-gemini
   ```
2. **Install dependencies**
   ```sh
   pip install -r requirements.txt
   ```
3. **Add your Gemini API key**
   - Create a file at `.streamlit/secrets.toml`:
     ```toml
     GEMINI_API_KEY = "your-gemini-api-key"
     ```
   - _This file is in `.gitignore` and will not be tracked._
4. **Run the app**
   ```sh
   streamlit run explain_app.py
   ```
5. **Open in your browser**
   - Go to `http://localhost:8501` (or the port shown in your terminal)

## Usage
- Use the sidebar to select a customer profile.
- Ask questions in the chat (e.g., "Why is this customer predicted to churn?").
- Muffin will use the selected customer's data and your database/CSV context to answer.
- Special Muffin persona responses for questions about the assistant's name or identity.

## Data
- Place your data files (CSV, SQLite DB) in the `/data` folder.
- The app will use these for context and explanations.

## Customization
- To change the LLM or add more features, edit `muffin_llm.py` and `explain_app.py`.
- The app is modular and easy to extend.

---

Built with ❤️ by Prudhvi Raj. Muffin is your friendly, explainable AI for customer retention!
