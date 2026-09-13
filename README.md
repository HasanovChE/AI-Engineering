# AI-Engineering
[AutoML-Web-Platform](https://github.com/HasanovChE/AutoML-Web-Platform)

[Motifs_Clustering_Project](https://github.com/HasanovChE/Motifs_Clustering_Project)

[Fine-Tuning-OpenAI-Whisper-model](https://github.com/HasanovChE/Fine-Tuning-OpenAI-Whisper-model)

## **Workflow Automation and Webhooks**

### **What is n8n?**
- n8n is a workflow automation tool: you connect nodes (trigger, logic, action) on a canvas instead of writing a backend from scratch. Each node receives JSON data from the previous node and passes JSON data to the next one.

### **Triggers vs. actions**

- A trigger node starts a workflow (a new Telegram message, a schedule, a webhook call). An action node does something (send a message, write a row, call an API). Between them, logic nodes (IF, Switch, Merge) decide which path the data takes.

### **Webhooks in one paragraph**

- A webhook is just a URL that, when called, delivers data to your workflow instantly - instead of your workflow having to constantly ask 'anything new?'. Telegram calls your n8n webhook the moment a message arrives.

### **Why this matters before AI**

- Every later week eventually needs to serve a model to a user - through a bot, a form, or an app. Learning to move JSON between systems reliably is the same skill whether the payload is a support ticket or an LLM response.

### **The Telegram Bot API in short**

- You create a bot through @BotFather, get a token, and that token lets any tool (including n8n) send and receive messages on behalf of the bot.


## **n8n Automation & Telegram Bots**
