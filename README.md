# group_work_ai_final
The Proposal
1. Problem: Most students watch YouTube videos while studying complex mathematical or technical subjects (such as programming or statistics) on their own. In such cases, the problem of passive viewing often occurs: students often lose focus on the studied topic, they cannot quickly discuss the topic with the author of the video through questions and cannot get really high-quality practical experience.
User: University students who take advanced technical courses, especially in IT and math majors.
2. AI feature: The system will include 4 specialized agents:
●	Curriculum Agent: Generates a personal roadmap for the student and selects high-quality videos from YouTube.
●	Context Agent: Extracts and analyzes the video transcript (using the youtube transcript api) and uses it to form key concepts and problem areas in the form of complex moments and hidden meanings.
●	Tutor Agent: Generates interactive contextual question prompts based on the received material and answers them, thereby helping with question-answers and summaries.
●	Assessment Agent: Creates adaptive tasks based on the video material, checks the answers received, and awards rewards for progress.
How we will measure whether it works: We will compare the relevance of the generated questions by tutor compared to the usual ChatGPT promts. Also we will check the examiner's error rate, that is, how well he creates tests and solves mathematical problems.
3. Agentic tools: Gemini API, Claude Code and GitHub Copilot
Both paid and free.
4. MVP: A working pipeline: The user enters a topic - The Context Agent downloads and analyzes the video transcript - The Tutor Agent outputs 3 interactive questions - The Assessment Agent generates a task for checking
Stretch goals: 
●	Gamification: experience system (XP), study streaks and collectibles for achievements on completed topics
●	Multilingual support: Transcripts and explanations in Russian and English.
5. Data and External APIs:
●	YouTube Data API v3 (available, free quotable key).
●	youtube-transcript api (available, an open Python library for parsing subtitles).
●	Gemini 1.5 Pro / Claude 3.5 Sonnet API (available API keys).
6. Who does what: 
Rabina (Frontend & User Experience): Interface (Streamlit / Next.js /FastHTML), video display, question chips, test widget and reward system.
Zhansulu (Evaluation & Math Engine): Creating an assessment dataset, writing evaluation scripts (Evaluation test suite), integrating task verification (Assessment Agent).
Karina (Backend & Agent Architecture): Multi-Agent Graph development (LangGraph/Python), integration with YouTube API and transcriptors.
