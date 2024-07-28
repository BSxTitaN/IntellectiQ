# IntellectiQ - Interactive Microlearning Platform 🏆

IntellectiQ is an innovative microlearning platform focused on technology-based subjects. This project was the **1st Rank Winner** for the CREST Data System Track during the Hackathon organized by the Computer Society of India in collaboration with TechHolding and IQM. IntellectiQ aims to enhance the educational experience by integrating advanced technology and innovative learning methods.

[LinkedIn Post](https://www.linkedin.com/posts/harsh-parekh-233689221_bringiton-hackathon-edtech-activity-7188217855161622528-bQQv?utm_source=share&utm_medium=member_desktop) - on the event of hackathon.

## Key Features ✨

1. **Video Content**: Users can upload educational videos to the platform.
2. **Video-to-Speech Extraction**: Extracts audio from videos to generate transcripts and summaries.
3. **Large Language Model (LLM) Integration**: Utilizes LLMs to identify grammatical errors in transcripts and create corresponding multiple-choice questions (MCQs).
4. **Innovative Feedback**: Provides playback points in the video for further learning when a user answers a question incorrectly.
5. **Leaderboard System**: Implements a ranking system based on MCQ completion to encourage user engagement and competition.

## Project Workflow 🚀

The backend logic of IntellectiQ is designed to seamlessly process and integrate various components. The figure below illustrates the workflow:

![Backend Logic](https://media.canva.com/v2/image-resize/format:JPG/height:500/quality:92/uri:s3%3A%2F%2Fmedia-private.canva.com%2FVVfrc%2FMAGDCRVVfrc%2F1%2Fp.jpg/watermark:F/width:800?csig=AAAAAAAAAAAAAAAAAAAAAIUbUQ0FcYHbAwAGs4hPqvO6-L3HRfCqhtY_Ms_lZh9C&exp=1722201813&osig=AAAAAAAAAAAAAAAAAAAAANs7Qx-ugAAfHPT-V6Z2cEM0caavY8R8W3Rbpr7X4jxh&signer=media-rpc&x-canva-quality=screen)

### Detailed Workflow Description

1. **User Input**: Users input video tags and upload videos to Google Cloud Storage.
2. **Extract Audio**: Audio is extracted from the uploaded videos.
3. **Generate Transcript with Timestamp**: The audio is fed to Assembly AI, which generates a transcript with timestamps.
4. **LLM Integration**: The generated transcript is processed by OpenAI GPT-3.5 Turbo to identify grammatical errors and create MCQs.
5. **Push Data**: The summarized paragraphs, QA pairs, MCQs, and video playback durations are pushed to Firebase Firestore.
6. **Frontend Client**: Interacts with the Firebase Firestore database to retrieve and display data.
7. **Innovative Feedback**: Users receive playback points for further learning based on their MCQ performance.

## Technologies Used 💡

Here is the list of technologies that power IntellectiQ:

- 🌐 **Web Development**
- 🤖 **LLMs**
- 🧠 **Model Fine-Tuning**
- ⚛️ **Next.js**
- 🌶️ **Flask**
- 🐍 **Python**
- 🔷 **TypeScript**
- 🎙️ **AssemblyAI**
- 🗣️ **Text-to-Speech**

## Project Demonstrations 📸

Below are some images demonstrating the various features and user interface of IntellectiQ:

- Image 1: Auth System with Signup/Login/Forget-Password
  ![VUI](https://media.canva.com/v2/image-resize/format:JPG/height:931/quality:92/uri:s3%3A%2F%2Fmedia-private.canva.com%2FATCaw%2FMAGDCBATCaw%2F1%2Fp.jpg/watermark:F/width:1280?csig=AAAAAAAAAAAAAAAAAAAAAGi7VjKXIBwW0raDkbGN5l-2YWj7AKILOFjRAWq8UcnC&exp=1722200843&osig=AAAAAAAAAAAAAAAAAAAAAHt50RPddC0x9lGJPxKAWAucvmKykDLFTDkBVe6zFi67&signer=media-rpc&x-canva-quality=screen_2x)
- Image 2: Transcription and Summarization Interface
  ![TSI](https://media.canva.com/v2/image-resize/format:JPG/height:588/quality:92/uri:s3%3A%2F%2Fmedia-private.canva.com%2FTO4dM%2FMAGDCOTO4dM%2F1%2Fp.jpg/watermark:F/width:800?csig=AAAAAAAAAAAAAAAAAAAAAGvP6t8c3V5kW_VceimxekI90IfAmUhFi2Bf6M3L2UvX&exp=1722200621&osig=AAAAAAAAAAAAAAAAAAAAAP3aXg9-WJk4hZqvqfUAozcL8qalgxOPQTEE22D6hhZE&signer=media-rpc&x-canva-quality=screen)
  ![TSI](https://media.canva.com/v2/image-resize/format:PNG/height:586/quality:100/uri:s3%3A%2F%2Fmedia-private.canva.com%2FNcjmM%2FMAGDDeNcjmM%2F1%2Fp.png/watermark:F/width:800?csig=AAAAAAAAAAAAAAAAAAAAAKqLdpkeebUnRKlZNovbqeK3ewj3kPfQYprjq6oberIs&exp=1722202267&osig=AAAAAAAAAAAAAAAAAAAAAISqwD1s2JikSqbGYZh2Wj-BUSCNqhng5BbtBa-Q0_bT&signer=media-rpc&x-canva-quality=screen)
- Image 3: MCQ Generation Interface & Feedback Playback Points
  ![MCQ1](https://media.canva.com/v2/image-resize/format:JPG/height:370/quality:92/uri:s3%3A%2F%2Fmedia-private.canva.com%2FP90O0%2FMAGDCqP90O0%2F1%2Fp.jpg/watermark:F/width:800?csig=AAAAAAAAAAAAAAAAAAAAABA8q3bQnsCzMc3ZUzRShnZdYD0WN4aEhKz20dybw5Bs&exp=1722200551&osig=AAAAAAAAAAAAAAAAAAAAAOQLK_Ga1hcgKvNX_jREbdOUa_1llfwOtP5OS160pCea&signer=media-rpc&x-canva-quality=screen)
  ![MCQ2](https://media.canva.com/v2/image-resize/format:JPG/height:651/quality:92/uri:s3%3A%2F%2Fmedia-private.canva.com%2FUuR5s%2FMAGDCMUuR5s%2F1%2Fp.jpg/watermark:F/width:800?csig=AAAAAAAAAAAAAAAAAAAAAN6gHIphdReHNPKv5HGU4TV8OvJRKLD0eXMX6SRHYJUw&exp=1722201642&osig=AAAAAAAAAAAAAAAAAAAAAGGho_TFnXAjrhX2xJ7tNC8xm39Zln8HPJYwFgx-Kgu6&signer=media-rpc&x-canva-quality=screen)
- Image 4: Home Screen
  ![HS2](https://media.canva.com/v2/image-resize/format:PNG/height:583/quality:100/uri:s3%3A%2F%2Fmedia-private.canva.com%2FthPqI%2FMAGDDbthPqI%2F1%2Fp.png/watermark:F/width:800?csig=AAAAAAAAAAAAAAAAAAAAAKXvfQAQIS9-eUedi1iQW2e9kaDchzvbKuEA-DOwovby&exp=1722201840&osig=AAAAAAAAAAAAAAAAAAAAABkKzCPsveDVUCIo8ltILVvYiw6_PyF64GSBuWrCTsY7&signer=media-rpc&x-canva-quality=screen)
- Image 5: Leaderboard System
  ![LS](https://media.canva.com/v2/image-resize/format:PNG/height:565/quality:100/uri:s3%3A%2F%2Fmedia-private.canva.com%2FLpeE8%2FMAGDDTLpeE8%2F1%2Fp.png/watermark:F/width:800?csig=AAAAAAAAAAAAAAAAAAAAAAN_bvcWnWBEfK4wVRNnBr1gL2fdpM8DG9j1kkZ8UH-L&exp=1722200595&osig=AAAAAAAAAAAAAAAAAAAAAHa12PdmWDRcIGougQIAN6zsc9utu5DpTAngpC_cPMi2&signer=media-rpc&x-canva-quality=screen)

## Team Develomers 👥

- **Harsh Parekh (Leader)**
- **Preet Dudhia**
- **Lakshit Pathak**
- **Khushi Shah**

## Conclusion 🎓

IntellectiQ leverages cutting-edge technology to transform the learning experience, making it interactive, engaging, and efficient. The platform's ability to generate accurate transcripts, create relevant MCQs, and provide targeted feedback ensures that users can learn effectively and stay motivated through gamification elements like leaderboards. 

We hope IntellectiQ will pave the way for more interactive and personalized learning experiences in the field of technology education.
