# Modi AstroGuru - Open WebUI AI Astrologer

## Open WebUI Link: [Modi AstroGuru - An AI Astrologer](https://openwebui.com/m/rithikaanand/modiastroguruv1)

![image](https://github.com/user-attachments/assets/c45be3a4-60ae-4ba9-a26a-125bb72a1be7)

## Objective
Modi AstroGuru is an AI-powered astrologer that predicts the future with the wisdom, confidence, and humor of PM Narendra Modi. This model provides engaging, insightful, and motivational zodiac readings infused with Modi-style slogans, desi jugaad, and leadership vision.

## Technology Stack Used
Modi AstroGuru is built using cutting-edge AI and cloud computing technologies to ensure high performance, scalability, and accuracy.

### 1. Large Language Model (LLM) – Llama 3.2: Latest
We leverage Llama 3.2: Latest, an advanced open-source LLM that excels in:
- Zodiac sign predictions with humor and motivation
- Storytelling with a leadership-driven approach
- Personalized and engaging astrology insights
- Conversational AI for cosmic guidance

Llama 3.2 provides fast and accurate responses, making it ideal for an AI-powered astrology mentor.

### 2. Web OpenAI via Docker
To test and deploy Modi AstroGuru, we pulled Web OpenAI from Docker, ensuring an isolated and optimized execution environment.
We first installed Ollama, an AI model serving framework, to efficiently run Llama 3.2.

## Installation & Deployment Process

### Step 1: Install Ollama
Ollama is used to run Llama 3.2 efficiently.
```sh
curl -fsSL https://ollama.ai/install.sh | sh
```
Once installed, we pull the latest Llama 3.2 model:
```sh
ollama pull llama3.2:latest
```
The Llama 3.2 model (~2GB) is downloaded and ready to use.

### Step 2: Deploy Web OpenAI on Docker
We used Docker to create an isolated container for Open WebUI, ensuring seamless communication with the model.
```sh
docker run -d -p 3000:8080 --add-host=host.docker.internal:host-gateway -v open-webui:/app/backend/data --name open-webui --restart always ghcr.io/open-webui/open-webui:main
```
This command spins up a Docker container, mapping port 3000 (local) to 8080 (container). The Open WebUI runs inside Docker and is ready to interact with Modi AstroGuru.

## Images

![image](https://github.com/user-attachments/assets/0dddabbe-8680-4ef6-918b-32882d4049d1)

## Video

https://github.com/user-attachments/assets/ad8468f6-742e-4b78-8064-cb45a5804be0

## Results: AI Astrology in Action

### Example 1: Basic Conversation
**User input:**
```
Hello
```
**🪔 Modi AstroGuru's response:**
```
Bhaiyo aur Behno! Namaste! 🙏 Kya aapka rashifal ho? Aapke zindagi ke saath mein kaise hoga? Chalo, hum is tarah se pechana shuru karte hain... 👀
Aap Aries (Mesh) ka hain? Taurus (Vrishabh)? Gemini (Mithun)? Cancer (Kark)? Leo (Singh)? Virgo (Kanya)? Libra (Tula)? Scorpio (Vrishchik)? Sagittarius (Dhanu)? Capricorn (Makar)? Aquarius (Kumbh)? Ya Pisces (Meen)?
Chalo, main aapke liye kuch tips aur suggestions deta hoon! 😊
```

### Example 2: Zodiac Insights
**User input:**
```
Gemini
```
**🪔 Modi AstroGuru's response:**
```
Bhaiyo aur Behno, Gemini (Mithun) ka! 🤔 Aapke zindagi mein change zaroori hai! Aap do-mukh wale nahi, bas bahut flexible ho! 👀
Aap naye naye ideas adopt karte hain, lekin thoda sochne ka samay bhi zaroori hai!
Apne decisions ko thoda think karein. Naye naye ideas adopt karte rahe! Apni flexibility ka istemaal karein! Yeh sab aapke zindagi mein change laane mein madad kar sakte hain! Chalo, aur kuch tips shuru karte hain... 🤔
```

### Example 3: Life Advice
**User input:**
```
Mere achhe din kab aayenge?
```
**🪔 Modi AstroGuru's response:**
```
Aapke achhe din tabhi aayenge jab aap khud taiyaar hon! Positivity rakhna aur naye opportunities ko embrace karna zaroori hai! Kyunki sahi samay ka intezaar mat karo, khud apna samay banao! 🚀
```

## Key Learnings from the Project

### 1. AI-Powered Astrology is the Future
Modi AstroGuru proves that AI can make astrology fun, engaging, and motivational while maintaining a leadership-driven approach.

### 2. Efficient AI Model Deployment Matters
Using Ollama + Docker for Llama 3.2 deployment ensures seamless performance and low-latency responses.

### 3. User-Centric AI Development
- AI astrologers need real-time adaptability and must align with user expectations.
- Docker allows scalability and smooth execution for AI-driven applications.
- AI-powered astrology assistants can boost engagement and provide insightful guidance in a unique way.

🚀 **Try Modi AstroGuru today and let Guru ji guide your destiny!** 🔮
