# pyttsx3 Text-to-Speech Documentation

## Installation
Make sure you have the `pyttsx3` module installed before using the code. If not, install it using the following command:

```bash
pip install pyttsx3
```

## Usage
```python
import pyttsx3 

# Initialize the text-to-speech engine (using SAPI5)
v_engine = pyttsx3.init('sapi5')

# Get the list of available voices
voice_list = v_engine.getProperty('voices')

# Choose the desired voice (you can print voice_list[0].id for voice details)
v_engine.setProperty('voice', voice_list[0].id)

# Provide the text you want to convert to speech
v_engine.say("Hello World")

# Ensure that the program waits for the speech to finish before moving on
v_engine.runAndWait()
```

## Description

This Python script demonstrates how to use the `pyttsx3` module to convert text into speech. The `sapi5` initialization sets up the Microsoft Speech API, and `getProperty('voices')` retrieves the available voices. You can choose a specific voice by setting the voice using `setProperty('voice', voice_list[0].id)`.

The `say()` method is used to input the text you want to convert to speech, in this case, "Hello World." Finally, `runAndWait()` ensures that the program waits for the speech to complete before continuing.

Note: The last line (`v_engine.runAndWait()`) is crucial for the proper functioning of the code. It allows the program to wait and synchronize with the speech engine, ensuring that the speech is fully processed before the program exits.

Feel free to customize the text and voice according to your preferences and project requirements. Enjoy exploring the world of text-to-speech with Python and pyttsx3!

Please Support Jocefyneroot YouTube Channel. #Let's Code The World!