# Profanity Censorship and Speech Processing Tool

## Overview
This project provides an advanced profanity censorship and speech processing tool that detects and censors profane words from both text and speech. It integrates modern machine learning techniques to accurately filter offensive language while maintaining the natural flow of speech.

## Features
- **Profanity Detection:** Utilizes a trained Random Forest model with an extensive dataset to identify profane words in text and speech.
- **Censorship in Audio:** Profane words detected in speech are replaced with a beep sound for censorship.
- **Speech-to-Text Transcription:** Converts spoken language from audio files into readable text.
- **Text Censorship:** Profane words in text are masked with asterisks (e.g., "f**k").
- **Artificial Voice Regeneration:** Uses text-to-speech (TTS) to generate a cleaned-up version of the input speech without offensive words.
- **Portable:** The required profanity dataset is embedded within the code, eliminating external dependencies.

 ## Dataset and Labeling
-A profanity dataset was used to identify offensive words.
-The NLTK words dataset was used to extract a large vocabulary of non-profane words.
-Words found in the profanity dataset were labeled as 1 (profane), while all other words were labeled as 0 (non-profane).
-This labeled dataset was used to train the profanity detection model.

## Performance and Accuracy
The model was tested on a labeled profanity dataset and achieved the following results:

- **Model Accuracy:** 92%
- **Classification Report:**

```
              Precision    Recall  F1-score   Support

           0       1.00      0.92      0.96    235730
           1       0.08      0.98      0.15      1659

    Accuracy                           0.92    237389
   Macro Avg       0.54      0.95      0.56    237389
Weighted Avg       0.99      0.92      0.95    237389
```

- **Confusion Matrix Visualization:** A heatmap is generated to analyze the model's misclassification patterns.

## Applications and Use Cases
- **Content Moderation:** Automatically filters offensive language on social media, forums, and chat applications.
- **Educational Use:** Helps in censoring inappropriate language in recorded lectures and educational materials.
- **Speech-to-Text Services:** Functions as a transcription tool while ensuring clean text output.
- **Podcast and Media Editing:** Useful for media producers and editors who need to censor offensive language in recorded content.
- **AI Assistants & Chatbots:** Enhances AI models by preventing offensive speech in generated responses.

## Technologies and Dependencies
- **Machine Learning:** Scikit-learn (Random Forest Classifier)
- **Speech Processing:** SpeechRecognition (Google API)
- **Audio Processing:** pydub (for audio file handling and modification)
- **Text-to-Speech:** gTTS (Google Text-to-Speech API)
- **Beep Sound Generation:** NumPy
- **Data Handling:** Pandas, NLTK



## License
This project is licensed under the MIT License.
