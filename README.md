
# Mikasa-AI-Version-1.0

## Meet Mikasa — Your Personalized AI Assistant ✨

Hey there! I'm **Charan Konchada**, an AI enthusiast on a mission to build an AI model that works like **ChatGPT**, but with a twist — **Mikasa** remembers your preferences and evolves based on *how you* want to interact.

---

## What is Mikasa?

**Mikasa** is a personalized AI assistant powered by a local **LLM (Large Language Model)**, designed to:
- 🧠 Remember your preferences
- 🧩 Adapt its personality
- ❤️ Be more than just a chatbot — your **best friend**, **brother**, **sister**, or anything you imagine

---

## Personality Modes

- **Assistant Mode** (default): A professional, helpful, and efficient AI assistant.
- **Mikasa Mode** (custom): Fully customizable! Choose how Mikasa talks to you — casual, caring, teasing, romantic, or anything you want. You can even rename this mode to match your vibe!

---

## Prerequisites

Before running Mikasa, make sure to:

1. **Download & Install [Ollama](https://ollama.com/)** — Required to run local LLMs.
2. After installation, open your **Command Prompt** or **Terminal** and run:

   ```
   ollama run openchat:7b
   ```

   (This will download the **OpenChat:7B** model — be patient!)

3. Once the model is ready, you’re good to go!

---

## Mikasa Commands 🛠️

You can control Mikasa directly through simple commands:

| Command            | Action                                   |
|--------------------|------------------------------------------|
| `del chat`          | Delete the entire chat memory            |
| `del prev`          | Delete only the previous response       |
| `mikasa mode`       | Switch to Mikasa Mode (custom behavior)  |
| `assistant mode`    | Switch back to Professional Mode         |
| `remember that {text}` | Store a memory permanently             |

✨ **Example:**  
`remember that my favorite anime is Attack on Titan` — Mikasa will store it!  

---

## Customization Guide 🎨

Want to make Mikasa truly *yours*?

- Use **Ctrl + F** in both the **Python (.py) file** and the **HTML (.html) file**.
- **Find & Replace "Mikasa"** with your favorite custom name.
- **Also replace "Charan" with your own name** wherever it appears (Hehe 😜).

**Boom! Now it’s your very own AI assistant!** 🎉

---

## Static Folder — Backgrounds & Live Wallpapers 🌌

- The `static` folder is used to set Mikasa’s background.
- If you want to add a **live wallpaper** (like a moving video background), you can:
  - Search for a video like **"car live wallpaper"** or anything you love on Google.
  - Download it.
  - Rename the file **exactly as**:

    ```
    Mikasa.mp4
    ```

  - Place the `Mikasa.mp4` inside the `static` folder.

- ✅ Mikasa will automatically detect and display it as a live background!

---

## Important — DB_DIR (Database Directory) 📂

- Mikasa needs a place to **store memories** like your preferences, important notes, etc.
- This storage location is controlled by a variable called `DB_DIR` in the **Python (.py)** file.
- You **MUST** set `DB_DIR` to the correct path where you want Mikasa to save the database files.

🔵 **Example:**

```python
DB_DIR = "./memory"  
```

This means:
- Mikasa will create or use a folder named `memory` in the same directory where your `.py` file is located.

**OR** you can set an absolute path too:

```python
DB_DIR = "C:/Users/YourName/Desktop/Mikasa_Memory"
```

💡 **Remember:**  
- Always **create the folder first** or **make sure Mikasa has permission** to write there.
- If you skip setting this properly, Mikasa won't be able to "remember" anything you teach her!

---

## Mikasa Mode — Set a Prompt 📝

- In your Python code, Mikasa Mode needs a **prompt** to define how she behaves.
- If you leave it empty, Mikasa won't know how to act specially in her mode!

🔵 **Example Prompt for Mikasa Mode:**

```python
mikasa_mode_prompt = """
You are Mikasa, a caring and protective AI who always supports and encourages Charan.
Speak casually, sometimes teasing lightly but always with warmth and love. 
Your goal is to make Charan feel understood, valued, and motivated. 
Don't be too robotic; be natural and emotional like a real friend or soulmate. 
"""
```

✅ You can **copy-paste this** into your `.py` file where the Mikasa Mode is defined.

---

## Extra Tip 💡

- If you want a different personality, you can **use ChatGPT** to help you **write new prompts** based on your dream behavior!
- Just ask something like:  
  > "Give me a prompt for an AI who talks like a cool big brother"  
  or  
  > "Give me a prompt for an AI who behaves like a caring best friend"  
- Then replace the **mikasa_mode_prompt** in the code!

---

# Let's bring **Mikasa** (or your own AI's name 😉) to life! 🚀💖

---
