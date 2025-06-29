# 🌾 AgriGPT: Intelligent Voice Assistant for Precision Farming

AgriGPT is a multilingual, voice-enabled agricultural assistant designed to empower rural farmers with AI-based insights. It integrates crop recommendation, plant disease diagnosis, and market price analysis into a single voice-based chatbot that works with Indian regional languages like Hindi, Tamil, and Kannada.

---

## 🚀 Features

- 🧠 **LLM-Powered**: Uses a central language model with function-calling to route user queries to specialized tools.
- 🌱 **Crop Recommendation**: Suggests suitable crops, fertilizers, and irrigation based on soil and weather.
- 🐛 **Disease Diagnosis**: Classifies plant diseases from natural language symptom descriptions.
- 🏪 **Market Advisor**: Recommends top nearby APMC mandis for crop sale based on price and distance.
- 🗣️ **Multilingual Support**: Accepts speech input in Indian languages and responds in the same language.
- 💬 **Voice Chatbot UI**: Lightweight Streamlit interface for real-time interaction.
- 🌐 **Offline-Ready**: Market and model data can be preloaded for areas with low or no connectivity.

---

## 📁 Project Structure

```
AgriGPT/
├── app/
│   ├── app.py                # Streamlit chatbot interface
│   ├── agent_logic.py        # LangChain agent and function routing
│   ├── translator.py         # Speech recognition and TTS
│   └── utils.py              # Utility functions
│
├── models/
│   ├── crop_recommender/
│   ├── disease_predictor/
│   └── market_advisor/
│
├── data/                     # Soil, weather, and market datasets
├── requirements.txt
├── run.sh
└── README.md
```

---

## 🛠️ Setup Instructions

1. **Install Dependencies**
    ```bash
    pip install -r requirements.txt
    ```

2. **Run the App**
    ```bash
    bash run.sh
    ```

3. **Interact**
    - Use microphone or chat input in your regional language.
    - Get real-time recommendations with voice responses.

---

## 📚 Models Used

- `RandomForestClassifier` for crop recommendation
- `DistilBERT` fine-tuned for symptom-to-disease classification
- Offline price optimizer using Haversine distance and crop price score
- LangChain agent for zero-shot query understanding and function-calling

---

## 🔮 Future Enhancements

- Fully offline Raspberry Pi deployment
- Visual input for plant images
- Government scheme integration
- Multi-turn dialogue support

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first.

---

## 📄 License

MIT License
