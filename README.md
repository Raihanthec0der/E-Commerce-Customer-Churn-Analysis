# 🗣️ Text-to-Speech Program

A modern and beginner-friendly **Text-to-Speech (TTS) application built with Python**.

The application converts written text into speech and provides controls for **Play, Pause, Resume, Stop, Voice Selection, Speech Speed, and Volume**.

> 🎯 Built as a practical Python project for learning GUI development, text-to-speech, threading, and error handling.

---

## ✨ Features

- 🔊 **Text-to-Speech** — Convert written text into spoken audio
- ▶️ **Play** — Start speaking the entered text
- ⏸️ **Pause** — Pause the speech
- ▶️ **Resume** — Continue speaking after pause
- ⏹️ **Stop** — Stop the current speech
- 🗑️ **Clear** — Clear the text box
- 🗣️ **Voice Selection** — Select from available system voices
- 🎚️ **Speech Speed** — Adjust speaking speed
- 🔊 **Volume Control** — Adjust speech volume
- 🛡️ **Error Handling** — Handles invalid input and common errors
- 🧵 **Multithreading** — Keeps the GUI responsive while speaking
- 🖥️ **GUI Application** — Built with Python Tkinter

---

## 🖼️ Screenshot

Add your application screenshot to the `assets` folder:

```text
assets/
└── screenshot.png
```

Then GitHub will display it here:

![Text-to-Speech Program](assets/screenshot.png)

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| 🐍 Python | Main programming language |
| 🗣️ pyttsx3 | Text-to-speech engine |
| 🖥️ Tkinter | Graphical user interface |
| 🧵 threading | Keeps the application responsive |
| 🔤 re | Splits text into sentences |
| 🌐 GitHub | Project hosting |

---

## 📂 Project Structure

```text
text-to-speech-program/
│
├── text_to_speech.py
├── requirements.txt
├── README.md
│
└── assets/
    └── screenshot.png
```

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/Raihanthec0der/text-to-speech-program.git
```

### 2. Enter the project directory

```bash
cd text-to-speech-program
```

### 3. Install the dependencies

```bash
pip install -r requirements.txt
```

Or install `pyttsx3` directly:

```bash
pip install pyttsx3
```

### 4. Run the application

```bash
python text_to_speech.py
```

---

## 📦 Requirements

The project currently requires:

```text
pyttsx3
```

Your `requirements.txt` should contain:

```text
pyttsx3
```

Tkinter is included with most standard Python installations on Windows.

---

## 🎮 How to Use

### 1. Enter Text

Type or paste text into the text box.

Example:

```text
Hello! Welcome to my Text-to-Speech application.
This project was created using Python.
```

### 2. Select a Voice

Choose an available system voice from the **Voice** dropdown.

### 3. Adjust Speed

Use the **Speed** slider to make the speech slower or faster.

### 4. Adjust Volume

Use the **Volume** slider to control the speech volume.

### 5. Play

Click:

```text
▶ Play
```

The application starts reading your text.

### 6. Pause

Click:

```text
⏸ Pause
```

The speech pauses.

### 7. Resume

Click:

```text
▶ Resume
```

The application continues from the next sentence.

### 8. Stop

Click:

```text
⏹ Stop
```

The current speech is completely stopped.

---

## 🧠 How Pause & Resume Works

The application separates the entered text into individual sentences.

For example:

```text
Hello everyone. Welcome to my project. Thank you for visiting.
```

The program processes it as:

```text
Sentence 1 → Sentence 2 → Sentence 3
```

When **Pause** is pressed, the speech engine stops and the application remembers the current sentence position.

When **Resume** is pressed, the application continues from the next sentence.

### ⚠️ Important Note

`pyttsx3` does not provide a reliable cross-platform native pause/resume API.

Therefore, this project uses **sentence-based pause and resume** rather than attempting to pause the audio at the exact word.

---

## 🧩 What I Learned

This project helped me practice:

### Python

- Variables
- Functions
- Classes
- Loops
- Conditional statements
- Exception handling
- Object-Oriented Programming

### GUI Development

- Tkinter
- Frames
- Labels
- Buttons
- Text widgets
- Comboboxes
- Sliders
- Event handling

### Other Concepts

- Text-to-speech technology
- Multithreading
- Regular expressions
- Error handling
- Project organization
- Git and GitHub

---

## 🔮 Future Improvements

Planned features for future versions:

- 🌍 Multiple language support
- 🎙️ More voice options
- 💾 Save speech as MP3/WAV
- 📄 Read `.txt` files
- 📕 Read PDF documents
- 📊 Word and character counter
- ⏱️ Speech progress indicator
- 🌙 Dark mode
- 🎨 More modern UI
- 🔄 Improved pause/resume behavior
- 🖥️ Windows `.exe` version
- 📋 Copy/paste shortcuts
- 🔊 Audio file playback controls

---

## 🐛 Known Limitation

The current pause/resume system works **between sentences**, not at the exact audio position.

For example:

```text
Sentence 1 → Sentence 2 → Sentence 3
```

If you pause while Sentence 2 is being spoken, the application may resume from Sentence 3 instead of the exact word where the pause occurred.

This behavior is related to the capabilities of the `pyttsx3` engine.

---

## 🤝 Contributing

Contributions are welcome!

### Fork the repository

Create your own fork on GitHub.

### Create a feature branch

```bash
git checkout -b feature/new-feature
```

### Make your changes

Improve the project or add a new feature.

### Commit your changes

```bash
git add .
git commit -m "Add new feature"
```

### Push your branch

```bash
git push origin feature/new-feature
```

Then open a **Pull Request** on GitHub.

---

## ⭐ Support

If you find this project useful for learning Python or text-to-speech development, please consider giving the repository a ⭐.

It helps support the project and motivates me to continue improving it.

---

## 👨‍💻 Author

**MD. Abdullah Al Raihan**

🐍 Python Learner | 📊 Aspiring Data Scientist | 💻 Developer

### GitHub

[Raihanthec0der](https://github.com/Raihanthec0der)

### Repository

[Text-to-Speech Program](https://github.com/Raihanthec0der/text-to-speech-program)

---

## 📜 License

This project is open-source and available for educational and personal use.

You are welcome to modify, improve, and learn from the code.

---

## 🚀 Project Status

**Version:** `v2.0`

**Status:** 🟢 Active Development

More features and improvements are planned for future releases.

---

### ⭐ If this project helped you, don't forget to star the repository!
