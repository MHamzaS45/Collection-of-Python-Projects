# 🏛️ Messages from the Four Emperors

**Messages from the Four Emperors** is a small text-based adventure and cryptography game written in Python, inspired by the *Year of the Four Emperors* of Ancient Rome.
The player travels between palaces, passes guarded entrances using secret passphrases, and uncovers encrypted messages left behind by each emperor.

This project blends **historical flavor**, **file-based game state**, and **classical cryptography** into a simple but intriguing console experience.

---

## 📜 Story Overview

You begin your journey at home and are tasked with visiting the palaces of four Roman emperors:

1. Galba
2. Otho
3. Vitellius
4. Vespasian

   <img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/eb028690-58f7-4173-9db5-8b067a3ad86b" />

Each palace holds a hidden message. To retrieve it, you must:

* Present the correct **passphrase** to the guards
* Locate an encrypted message file
* Decipher it using a **ROT13 Caesar cipher**
* Preserve your progress as you move on to the next emperor

Once all emperors have been visited, your journey is complete.

---

## 🧠 Core Concepts

This project demonstrates several programming ideas:

* **ROT13 encryption/decryption**
  A simple Caesar cipher used for both passphrases and emperor messages.

* **File-based persistence**
  Player progress is stored in `player_progress.txt`, allowing the game to resume where it left off.

* **State-driven gameplay**
  Locations, progress, and messages are determined dynamically based on saved data.

* **Light puzzle mechanics**
  Encrypted filenames and messages encourage curiosity and exploration.

---

## 📁 Project Structure

* `player_progress.txt`
  Stores the player’s current location, next destination, and encrypted passphrase.

* `*.gkg` files
  Encrypted message files for each emperor.
  Format:

  ```
  <location_id>_<encrypted_passphrase>.gkg
  ```

* `*.txt` files
  Deciphered, human-readable messages generated after each visit.

---

## ▶️ How to Run

1. Make sure you have **Python 3** installed.
2. Place the game script and message files in the same directory.
3. Run the script:

   ```bash
   python main.py
   ```
4. Follow the console narration as your journey unfolds.

Progress is autosaved after each successful palace visit.

---

## 🏁 End Condition

The game ends automatically after all four emperors have been visited and their messages decrypted.

---

## ✨ Notes

* The project intentionally uses simple file handling and encryption for educational clarity.
* The ROT13 cipher is symmetric—encrypting and decrypting use the same function.
* The missing trailing comma in the `LOCATIONS` dictionary is… deliberate. Seasoned programmers know why 😉

---

## 📌 Purpose

This is a **personal learning project**, created to practice and apply knowledge on:

* Python fundamentals
* File I/O and Handling
* String manipulation with Cryptography 
* Low level Game development with Python with a narrative
* Clean, readable code that is understood. 

---

Enjoy uncovering the secrets of the emperors as you traverse through the 4 Lands.! 📃
