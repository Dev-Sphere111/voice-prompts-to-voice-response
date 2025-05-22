# voice-prompts-to-voice-response

I developed a Node.js application where you can pose questions to ChatGPT using vocal inputs, observe the ChatGPT-style word-by-word answer, and then hear the replies spoken aloud.

**Audio to Text Conversion:** I transform audio into text utilizing [Whisper](https://openai.com/research/whisper), which is an OpenAI Speech Recognition Model that converts audio into text with an accuracy of up to 99%. Whisper is a speech transcription framework from the creators of ChatGPT. It is available for anyone to use and is entirely free. The system has been trained on 680,000 hours of speech data from the internet and recognizes 99 different languages.

**Generating Replies:** To produce word-by-word replies and show them, we leverage the [LangChain](https://js.langchain.com/) streaming API. This API enables us to obtain words in real-time as they are formed. Furthermore, we employ Node.js Socket.IO, which facilitates bidirectional and event-driven communication between the client-side and server-side.

**Text to Audio Conversion:** I utilize [gTTS.js](https://www.npmjs.com/package/gtts), which is a Google Text to Speech JavaScript library originally developed in Python.

To begin:

```
        Clone the repository

        git clone https://github.com/Dev-Sphere111/voice-prompts-to-voice-response/
        cd voice-prompts-to-voice-response

        Add your API key to the .env file

        # installs package dependencies
          npm install

        # to execute locally
          npm start

```
