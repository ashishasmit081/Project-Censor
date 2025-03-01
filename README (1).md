# Profanity Censorship and Speech Processing Tool

This project provides a powerful profanity censorship and speech processing tool that can detect and censor profane words from text and speech. It also provides additional functionalities like speech-to-text transcription and generating censored audio using artificial voice generation.

## Features

- **Profanity Detection**: Uses an extensive dataset to detect profane words in text and speech.
- **Censorship in Audio**: Profane words in speech are replaced with a beep sound.
- **Speech-to-Text Transcription**: Converts audio input into readable text.
- **Text Censorship**: Profane words in text are masked with asterisks (e.g., "f**k").
- **Artificial Voice Regeneration**: Uses text-to-speech to generate a clean version of the input speech.
- **Portable**: No need for an external dataset; all required data is embedded within the code.

## Applications and Use Cases

- **Content Moderation**: Helps in filtering offensive language from audio and text platforms.
- **Educational Use**: Can be used in schools to censor inappropriate language in recorded lectures.
- **Speech-to-Text Services**: Acts as a transcription tool for audio files.
- **Podcast and Media Editing**: Useful for editors who need to clean up recorded content.
- **Safe AI Assistants**: Enhances AI assistants by removing offensive speech.

## Technologies and APIs Used

- **SpeechRecognition**: For converting speech to text.
- **pydub**: To process and modify audio files.
- **gTTS (Google Text-to-Speech)**: For regenerating censored audio.
- **NumPy**: Used to generate beep sounds when necessary.
- **Pandas**: Used for handling and managing the profanity dataset.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
