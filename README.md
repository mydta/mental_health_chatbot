# Mental Health Chatbot Analysis

This project analyzes and models mental health–related conversations to identify emotional themes, sentiment transitions, and topic clusters. It leverages **transformers**, **BERTopic**, and **unsupervised learning** to explore the linguistic and emotional structure of chat data related to mental health and well-being.

## Interactive Dashboard Overview

An interactive **Looker Studio dashboard** accompanies this analysis to visualize insights from the chatbot conversation data.  
It highlights how users express, regulate, and shift emotions throughout their interactions with the chatbot.

### Dashboard Focus
- **Chatbot Conversation Insights:** Summarizes engagement patterns, conversation depth, and emotional consistency across ~500 chatbot sessions.  
- **Emotional Flow Metrics:** Tracks **Emotion** and **Sentiment Transition Rates** to reveal how emotional tone changes during conversations.  
- **Engagement Indicators:** Measures **Drop-off Point** and **Conversation Turns** to evaluate user interaction length and stability.  
- **Sensitive Content & Themes:** Identifies conversations containing emotional intensity, personal disclosures, or sensitive mental health topics.  
- **Text-Level Analysis:** Explores message structure, word usage, and emotional cues within individual texts.

### Purpose
The dashboard translates complex NLP outputs into interpretable visuals—helping researchers, designers, and developers understand user behavior, emotional stability, and engagement quality in mental health chatbot interactions.

For more information, visit the full dashboard and NLP workflow:  
[Chatbot Conversation Insights Dashboard](https://lookerstudio.google.com/) *(replace with actual link once public)*

## Features
- **Emotion & Sentiment Detection** using pre-trained transformer models from Hugging Face.  
- **Topic Modeling** with `BERTopic` and `HDBSCAN` to uncover recurring themes.  
- **Conversation Analysis** to measure emotional transitions, coping themes, and sensitive content.  
- **Data Visualization & Insights** for emotional progression across dialogues.

## Tech Stack
- **Python 3.10+**  
- **Hugging Face Transformers** for emotion and sentiment classification  
- **BERTopic** + **HDBSCAN** for unsupervised topic discovery  
- **scikit-learn** for vectorization  
- **Pandas / NumPy** for data preprocessing  
- **tqdm** for progress tracking  
- **Datasets** (Hugging Face) for loading and managing data  

## Project Structure
```
Mental_Health_Chatbot/
├── Mental_Health_Chatbot.ipynb    # Main notebook for analysis and modeling
├── results/                       # Generated outputs (topics, labels, plots)
├── requirements.txt               # Dependency list
└── README.md                      # Project overview
```

## Installation

1. Clone the repository
   ```bash
   git clone https://github.com/mydta/mental_health_chatbot.git
   cd Mental_Health_Chatbot
   ```

2. Create a virtual environment
   ```bash
   python -m venv venv
   source venv/bin/activate  # (Windows: venv\Scripts\activate)
   ```

3. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```

## Usage
Open the notebook in Jupyter or VSCode:
```bash
jupyter notebook Mental_Health_Chatbot.ipynb
```

Follow the workflow:
1. Load the dataset (e.g., chat transcripts or text logs).  
2. Run emotion/sentiment classification.  
3. Apply topic modeling with BERTopic.  
4. Export and visualize clustered insights.  

## Example Outputs
- Emotion transition trends across conversations  
- Thematic clusters such as *Stress & Overwhelm*, *Coping & Resilience*, *Grief & Loss*  
- Sentiment progression and topic-level emotional intensity  
- Chatbot engagement metrics visualized through the Looker Studio dashboard  

## Dependencies
See [`requirements.txt`](./requirements.txt)

## Author
Developed by **My Ta**  
For research and analysis of emotional language patterns in mental health chatbot dialogues.

## License
MIT License © 2025 My Ta
