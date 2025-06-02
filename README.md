# Smart-ClaimMate
A RAG-powered virtual assistant built with IBM watsonx.ai for insurance claim support.
# 💡 Smart ClaimMate – IBM watsonx.ai Hackathon Submission

**Theme:** Advance the Future of Customer Experience  
**Team:** Solo Submission  
**Built With:** IBM watsonx.ai Prompt Lab, RAG (Retrieval-Augmented Generation), UI Mockups (Canva), Python (Optional), GitHub  


## 🧠 Overview

**Smart ClaimMate** is a Retrieval-Augmented Generation (RAG)-powered virtual assistant designed to simplify insurance claims — starting with healthcare and scalable to auto and banking use cases.  
It uses IBM watsonx.ai to provide clear, document-aware answers, personalized suggestions, and a supportive user experience for people struggling with claim denials, policy confusion, and appeal processes.


## 🔨 Development Journey

### 📌 Step 1: Problem Definition  
We identified a common customer pain point:  
Insurance claim processes are confusing, emotionally draining, and often inaccessible to the average user.

We asked:  
> *“What if we could turn complex denial letters into plain-language support with next steps, and even generate email drafts — all through a friendly chatbot?”*



### 📌 Step 2: UI Design and Structure  
We created a clean UI mockup with three main areas:
- **Left Panel**: Customer Profile, Policy Details, Claim Timeline
- **Main Panel**: AI Chat interface with user + assistant bubbles, charts, denial reason insights, and "Did You Know?" tips
- **Bottom Panel**: Dispute Suggestion Mode – including a draft email generator

Mockups were designed using **Canva**, and are located in `ui-mockups/`.



### 📌 Step 3: Prompt Development (watsonx.ai Prompt Lab)  
We used IBM **watsonx.ai Prompt Lab** to:
- Create a custom **System Prompt** that guided the assistant to behave like an empathetic, document-based insurance advisor
- Upload relevant documents (policy PDFs, denial letter samples, hospital listings)
- Test multiple **user questions** to confirm grounded, helpful responses

We grounded all answers using **RAG**, ensuring they come from uploaded documents only.

🧾 Sample user questions:
- "Why was my claim denied?"
- "What hospital near me is wheelchair accessible?"
- "What plan suits my current diagnosis?"

📄 All prompt files are saved under: `prompts/`

### 📌 Step 4: RAG Integration & Logic  
We simulated a **RAG pipeline** by using:
- **Document Uploads** in Prompt Lab
- Prompt instructions to pull only from relevant sources
- Custom instructions to summarize, reason, or generate structured replies like mail drafts

📊 Additional features added:
- Trust score / approval prediction logic
- Document suggestions based on denial type
- Email appeal draft generation
- ZIP code–based hospital recommendations (plan compatibility, doctor, rating)

See full write-up in `docs/RAG_Usage.md`



### 📌 Step 5: Video Demo  
A 90-second demo video was created to:
- Show the user journey  
- Explain the tech and prompt logic  
- Walk through the UI with visual highlights  

📽 Watch it here: [👉 Demo Video]https://drive.google.com/file/d/1hvtPqyOepJUbc5OPW-C29UWYNgZpq5di/view?usp=sharing
(Replace with your actual YouTube or Vimeo link)



### 📌 Step 6: Submission  
We submitted:
- 📝 Problem + Solution write-up (see `docs/Problem_Statement.md`)
- 🧠 RAG & watsonx.ai usage explanation (see `docs/RAG_Usage.md`)
- 🎥 Video demo (see `demo/video_link.txt`)
- 💻 Code & assets (this repo)

No public deployment was required — everything is shown through Prompt Lab and UI mockups.



## 💡 Features Recap

- Chatbot built with watsonx.ai + RAG
- Policy explanation in simple terms
- Email draft generator for appeals
- ZIP code–based hospital finder
- Trust score / approval prediction
- "Did You Know?" education tips
- Easy prompt customization for other domains



## 🔄 Reusability

Smart ClaimMate can be adapted to other insurance sectors:
- 🚗 **Auto Insurance**
- 🏦 **Banking Claims**
- 🏥 **Healthcare Plans**

Just upload different policy files and adjust the system prompt — the same assistant logic applies.



## 📁 Repository Structure

