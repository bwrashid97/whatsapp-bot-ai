
# WhatsApp Bots - Multi-Version Automation

This repository contains three versions of WhatsApp chatbots, each designed for different levels of automation and integration. The bots are built using **Node.js**, leveraging **WhatsApp Web API**, **databases**, and **AI technologies** where applicable.

##  Available Versions

### **Basic Bot**
**A simple chatbot for automated keyword-based responses.**  
- **Technology:** Node.js, `whatsapp-web.js`, `express.js`
- **Features:**
  - Keyword-based automated replies
  - Simple response customization
  - No database or authentication required

### **Standard Bot**
**A chatbot with database integration and user authentication.**  
- **Technology:** Node.js, MongoDB/PostgreSQL, `mongoose`
- **Features:**
  - User authentication and data storage
  - Personalized responses based on user history
  - Optional integration with CRM platforms

### **Premium Bot**
**An AI-powered chatbot with multilingual support and automation.**  
- **Technology:** Node.js, OpenAI GPT-4, `langchain`, MongoDB/PostgreSQL
- **Features:**
  - AI-generated responses with contextual understanding
  - Sentiment and intent analysis
  - Task automation (scheduling, transactions, workflows)

## 🛠 Installation & Setup

### **1️ Clone the Repository**
```sh
git clone https://github.com/bwrashid97/whatsapp-bots.git
cd whatsapp-bots
```

### **2️ Install Dependencies**
```sh
npm install
```

### **3️ Configure Environment Variables**
Create a `.env` file in the project root:
```
WHATSAPP_SESSION=your-session-token
DATABASE_URL=mongodb://localhost:27017/whatsapp-bot
OPENAI_API_KEY=your-openai-key
```

### **4️ Run the Bot**
#### Basic Version:
```sh
node basic-bot/server.js
```
#### Standard Version:
```sh
node standard-bot/server.js
```
#### Premium Version:
```sh
node premium-bot/server.js
```

### **5 Run with PM2 for Continuous Execution**
```sh
npx pm2 start basic-bot/server.js --name basic-bot
npx pm2 start standard-bot/server.js --name standard-bot
npx pm2 start premium-bot/server.js --name premium-bot
```

## Deployment
The bots can be deployed on **local servers** or **cloud environments**:
- AWS (Lambda, EC2)
- Heroku
- DigitalOcean
- Docker:
  ```sh
  docker build -t whatsapp-bot .
  docker run -d -p 3000:3000 whatsapp-bot
  ```

## License
This project is licensed under the **MIT License**.

## Contributing
Fork the repository, create a feature branch, and submit a pull request.

---
**Note:** This repository is private. Access is restricted to authorized contributors.
```
