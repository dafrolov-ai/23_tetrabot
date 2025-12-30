# Voice Command Recognition for Robot Control

## 📌 Project Description

This project focuses on the development of a voice command recognition system based on neural networks and the conversion of recognized commands into two-byte control codes for a robot.
Control is performed via an Android application that captures user speech, recognizes commands, and transmits them to the robot control unit.

---

## 🎯 Project Goal

To build a software–hardware pipeline **“voice → command → code → robot”** with high recognition accuracy (above 95%) and support for extending the command vocabulary.

---

## 🧩 Project Tasks

* Voice command recognition using pre-trained and experimental Speech-to-Text (STT) models
* Command vocabulary creation and matching against reference commands
* Encoding commands into predefined two-byte values
* Development of Android applications for transmitting commands to the robot
* Testing command transmission using Arduino / ESP modules

---

## 📥 Input Data

* User voice commands (Russian language)
* Audio stream from an Android device microphone
* Pre-trained speech recognition models (Vosk, Google Speech Recognition)
* Dictionary of supported commands and their corresponding codes

---

## 📤 Output Data

* Recognized command text
* Normalized command (using Levenshtein distance)
* Decimal / two-byte command code
* Command transmission to the robot control unit

---

## 🧠 Technologies Used

* **Speech-to-Text:** Vosk (offline ASR based on Kaldi), Google Speech Recognition, SpeechRecognition, experiments with DeepSpeech2
* **NLP processing:** Levenshtein distance, Pymorphy2, command dictionary normalization, command parameter parsing
* **Android:** Kotlin, Java, Flutter, Kivy, App Inventor 2, Android Studio, KivyMD
* **Backend / Prototyping:** Python, Google Colab, Jupyter Notebook, TCP sockets, HTTP / POST requests
* **Hardware & Communication:** Arduino, ESP-01, ESP8266, Wi-Fi, Serial / Hardware UART

---

## 📂 Repository Structure

'''

### `001_Concept_and_analysis`

Project documentation including task description, goals, requirements, and analysis of voice command recognition approaches and robot control system design options.

### `002_notebooks`

Jupyter / Google Colab notebooks containing experiments with speech recognition, command processing, evaluation of Vosk model accuracy, and command matching logic.

### `003_android_vosk_demo_kotlin`

Demonstration Android application written in Kotlin using Vosk for voice command recognition and conversion into predefined robot control codes.

'''

---

## ✅ Project Results

* Multiple Android application variants were implemented
* Voice command recognition accuracy exceeds 95%
* Support for complex command parsing, including:

  * single commands
  * command sequences
  * commands with parameters
* The system is scalable and can be extended with new commands and devices

---

## 🧪 Project Status

The project is completed and its objectives have been achieved.
The solution is ready for demonstration and further engineering development.
