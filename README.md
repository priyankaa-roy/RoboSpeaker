# 🤖 RoboSpeaker 1.2 🎙️

Welcome to **RoboSpeaker 1.2**, a fun and interactive text-to-speech program created by Priyanka! 🎉 This program uses Python's `os` module and the `win32com.client` library to convert text inputs into spoken words. It's a great way to explore text-to-speech capabilities on both Mac 🍎 and Windows 💻 systems.

---

## ✨ Features

- 🗣️ **Interactive Text-to-Speech**: Type any text, and the program will speak it aloud.
- 🌐 **Multi-platform Support**:
  - 🍎 On **Mac**, it uses the `say` command for speech synthesis.
  - 💻 On **Windows**, it utilizes the `win32com.client` library for text-to-speech.
- ✅ **User-friendly Exit**: Type `q` to gracefully exit the program with a thank-you message.
- ⏱️ **Customizable Speech Delays**: Insert pauses between narrations using Python's `time.sleep()`.

---

## 🔧 Prerequisites

1. 🐍 **Python**: Ensure you have Python installed (version 3.7 or above recommended).  
2. 💾 **win32com.client** (Windows only): Install the `pywin32` library if running on Windows.  
   ```bash
   pip install pywin32
   ```
3. 🍎 For **Mac**, ensure the `say` command is available (default on most macOS versions).

---

## 🚀 How to Run

1. 📥 Clone the repository:  
   ```bash
   git clone [https://github.com/your-username/RoboSpeaker.git](https://github.com/priyankaa-roy/RoboSpeaker)
   ```
2. 📂 Navigate to the project folder:  
   ```bash
   cd RoboSpeaker
   ```
3. ▶️ Run the program:  
   ```bash
   python robospeaker.py
   ```

---

## 🛠️ Usage

1. **Start the program**:
   - ✏️ Enter text you want the program to speak.
   - 🔊 The program will convert your text to speech immediately.
2. **Exit the program**:
   - ❌ Type `q` to quit the program.
   - 🖐️ It will bid you farewell with a spoken "Thanks for interacting."

---

## 🧩 Code Overview

### 🍎 For macOS  
The program uses the `os` module and the `say` command to convert text to speech:  
```python
import os
x = input("Enter what you want me to speak: ")
command = f"say {x}"
os.system(command)
```

### 💻 For Windows  
The program uses the `win32com.client` library to access the Windows Speech API (SAPI):  
```python
import win32com.client as wincom
speak = wincom.Dispatch("SAPI.SpVoice")
speak.Speak("This is a Python text-to-speech test.")
```

---

## 🤝 Contributions

Contributions are welcome! 🌟 If you have ideas to enhance RoboSpeaker or make it more versatile, feel free to fork the repository and submit a pull request. 🛠️

---

## 📜 License

This project is licensed under the [MIT License](LICENSE). 📝

---

## 👩‍💻 Author

Developed with ❤️ by **Priyanka**.  

Enjoy interacting with **RoboSpeaker 1.2**! 🚀✨
