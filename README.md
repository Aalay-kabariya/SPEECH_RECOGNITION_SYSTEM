# Speech_RECOGNITION_SYSTEM 
A Python-based web app that transcribes `.wav` audio files into text using **Facebook's Wav2Vec2 model**. Built with **Streamlit** for seamless deployment.

## Project Details  
- **Company:** CODETECH IT SOLUTIONS  
- **Intern Name:** Aalay Kabariya  
- **Intern ID:** C0DF49  
- **Domain:** Artificial Intelligence  
- **Duration:** 4 Weeks  
- **Mentor:** Neela Santosh  

## Features  
✅ **Upload .wav audio files** via an intuitive UI  
🔄 **Automatic audio preprocessing** (mono conversion, resampling to 16kHz)  
🔊 **Accurate speech-to-text transcription** powered by Wav2Vec2  
⚡ **Fast inference** with cached model loading  
❌ **Error handling** for invalid inputs  

## Technologies Used  
- **Python** – Core programming language  
- **Streamlit** – Web UI framework  
- **PyTorch & TorchAudio** – Audio processing  
- **Hugging Face Transformers** – Wav2Vec2 model integration  
- **Wav2Vec2** – (`facebook/wav2vec2-base-960h`)  

## How It Works  
### Model Loading  
- Loads pre-trained **Wav2Vec2 model** and processor, cached for efficiency.  

### Audio Processing  
- Converts **stereo → mono** for consistency.  
- Resamples audio to **16kHz** if required.  

### Transcription  
- Audio input → **Wav2Vec2 Model** → **Text output**  

### UI  
- Users upload `.wav` files and receive transcriptions **instantly**.  

## Installation  
```bash
git clone https://github.com/yourusername/speech-to-text-app.git
cd speech-to-text-app
pip install torch torchaudio transformers streamlit 
streamlit run text-to-speech.py  # Launch the app
