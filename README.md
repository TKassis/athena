<p align="center">
  <img src="athena_logo.png" alt="Athena Logo" width="500">
</p>


<p align="center">
  Athena is a basic yet customizable conversational agent with short-term (session-based) memory. It includes two-way dialogue capabilities using OpenAI Whisper for speech-to-text and ElevenLabs for text-to-speech. By default, Athena is powered by GPT-4 and features the Bella voice from ElevenLabs.
</p>

## 🚀 Installation

1. **API Keys Configuration**:
Create a `.env` file in the root directory with your OpenAI and ElevenLabs API keys:
     ```
     OPENAI_API_KEY=1234
     ELEVEN_API_KEY=1234
     ```

2. **Environment Setup**:
Create a conda environment using the `environment.yml` file provided in the repository.
   ```
   conda env create -f environment.yml
   ```
   or (recommended)
    ```
    mamba env create -f environment.yml
    ```
3. **Customize Athena**:
Modify `athena.py` for your specific needs:
- `user_bio`: Add your name, bio, location, etc. This is the information you'd like Athena to be aware of.
- `assistant_bio`: Customize Athena's name, bio, personality, or any other traits you'd like.
- `device_index`: Adjust this value if needed to select the correct microphone on your system.
- `voice`: Select from the available ElevenLabs voices or even create your own on their platform.

4. **Run Athena**: Execute the command:
    ```
    python athena.py
    ```

  ## ✅ To-Do
- [ ] Add long-term memory using a vector database
- [ ] Switch to faster_whisper as transcription seems to be slow
- [ ] Add optional knowledge store
