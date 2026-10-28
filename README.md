# AI-Engineering

[Fine-Tuning-OpenAI-Whisper-model](https://github.com/HasanovChE/Fine-Tuning-OpenAI-Whisper-model)

[Motifs_Clustering_Project](https://github.com/HasanovChE/Motifs_Clustering_Project)

[Satellite-Vision-Platform](https://github.com/HasanovChE/Satellite-Vision-Platform)

[AutoML-Web-Platform](https://github.com/HasanovChE/AutoML-Web-Platform)

[myAIPlatform](https://github.com/HasanovChE/myAIPlatform)

[nlp](https://github.com/HasanovChE/nlp)


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
[FAQ-Bot-Backed-by-a-Knowledge-Base-Spreadsheet---n8n](https://github.com/HasanovChE/FAQ-Bot-Backed-by-a-Knowledge-Base-Spreadsheet---n8n)

[Customer-Support-Ticket-Bot-with-n8n-and-Telegram](https://github.com/HasanovChE/Customer-Support-Ticket-Bot-with-n8n-and-Telegram)

[Daily-Personal-Digest-Bot---n8n](https://github.com/HasanovChE/Daily-Personal-Digest-Bot---n8n)


## **Convolutional Neural Networks**

### **Why not just use an MLP on pixels?**
- A plain fully-connected layer treats every pixel as unrelated to its neighbors and has no notion of 'this shape appears somewhere in the image.' A convolution slides a small filter across the image, so the same detector (an edge, a curve) can fire anywhere in the picture.

### **Convolution and pooling in one paragraph each**
- A convolution layer learns small filters that respond to local patterns. Pooling (usually max-pooling) shrinks the feature map, keeping the strongest signal in each region and making the network less sensitive to small shifts.

### **Reading loss curves**
- If training loss keeps dropping while validation loss rises, the model is overfitting. If both stay high, the model is underfitting or the learning rate is off. A healthy curve shows both decreasing and then flattening together.

### **Overfitting and regularization**
- Dropout randomly disables neurons during training so the network can't over-rely on any single path. Data augmentation increases effective dataset diversity, which reduces overfitting too - but too much can slow learning or blur the class signal.

[Handwritten-Digit-Classifier-with-a-CNN-MNIST](https://github.com/HasanovChE/Handwritten-Digit-Classifier-with-a-CNN-MNIST)

[Digit-Classifier-Web](https://github.com/HasanovChE/Digit-Classifier-Web)

[Data-Augmentantion](https://github.com/HasanovChE/Data-Augmentantion)


## **Object Detection and OCR Pipelines**

### **Detection vs. classification**
- Classification answers 'what is in this image?'. Detection answers 'what is in this image, and where?' by predicting bounding boxes plus classes.

### **Intersection over Union (IoU)**
- IoU measures how much a predicted box overlaps a ground-truth box: area of overlap divided by area of union. An IoU near 1.0 means a near-perfect box; a common threshold for 'counts as a correct detection' is IoU >= 0.5.

### **Why anchor-free detectors got popular**
- Older detectors predicted boxes relative to predefined anchor shapes. Modern anchor-free detectors (like YOLOv8) predict box coordinates directly, simplifying training and often improving speed.

### **OCR basics**
- Optical Character Recognition converts pixels of text into a string. It works best on clean, high-contrast, upright text - which is exactly what a good plate-cropping step should produce for the recognizer.

### **Why pipelines break at the seams**
- A detector that works perfectly and an OCR engine that works perfectly can still produce a broken pipeline if the crop between them is off by a few pixels, has no padding, or isn't deskewed. Test the seam, not just each half.

[License-Plate-Detection-and-Recognition-Pipeline](https://github.com/HasanovChE/License-Plate-Detection-and-Recognition-Pipeline)

[Multi-Country-Plate-Classifier](https://github.com/HasanovChE/Multi-Country-Plate-Classifier)

[Detector-Speed-Benchmark-Accuracy-vs.-Latency](https://github.com/HasanovChE/Detector-Speed-Benchmark-Accuracy-vs.-Latency)
