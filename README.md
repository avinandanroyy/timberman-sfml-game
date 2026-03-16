# 🌲 Timber - SFML Lumberjack Game

![C++](https://img.shields.io/badge/language-C++-blue)
![SFML](https://img.shields.io/badge/library-SFML-green)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20macOS-lightgrey)
![License](https://img.shields.io/badge/license-MIT-orange)

A fast-paced **2D lumberjack arcade game** built using **C++** and the **Simple and Fast Multimedia Library (SFML)**.

The objective is simple: **chop the tree as fast as possible while avoiding branches and managing time**.

---

# 🎮 Gameplay

* Chop the tree from **left or right**
* Avoid falling branches
* Each successful chop adds a small amount of time
* Survive as long as possible and beat your score

*(You can place a gameplay screenshot or GIF here later)*

```
docs/gameplay.gif
```

---

# 📂 Project Structure

```
Timber-SFML-Game/
│
├── main.cpp
│
├── textures/
│   ├── background.png
│   ├── bee.png
│   ├── cloud.png
│   ├── tree.png
│   ├── branch.png
│   ├── rip.png
│   ├── player.png
│   ├── axe.png
│   └── log.png
│
├── sound/
│   ├── chop.wav
│   ├── death.wav
│   └── out_of_time.wav
│
├── font/
│   └── KOMIKAP_.ttf
│
└── README.md
```

⚠️ The game **requires these folders** to exist in the same directory as the executable.

---

# 🚀 Build and Run

## 🍎 macOS

### Install Dependencies

```bash
brew install sfml@2
```

### Compile

```bash
g++ main.cpp \
-I/opt/homebrew/Cellar/sfml@2/2.6.2_1/include \
-L/opt/homebrew/Cellar/sfml@2/2.6.2_1/lib \
-lsfml-graphics -lsfml-window -lsfml-system -lsfml-audio \
-o main
```

### Run

```bash
./main
```

---

## 🐧 Linux (Ubuntu / Debian)

### Install Dependencies

```bash
sudo apt update
sudo apt install libsfml-dev
```

### Compile

```bash
g++ main.cpp -o main -lsfml-graphics -lsfml-window -lsfml-system -lsfml-audio
```

### Run

```bash
./main
```

---

## 🪟 Windows (MinGW / GCC)

### Setup

1. Download the **MinGW version of SFML**
2. Extract to:

```
C:\SFML
```

### Compile

```bash
g++ main.cpp -I"C:\SFML\include" -L"C:\SFML\lib" -lsfml-graphics -lsfml-window -lsfml-system -lsfml-audio -o main.exe
```

### Copy DLL Files

Copy all `.dll` files from:

```
C:\SFML\bin
```

Paste them into the folder containing `main.exe`.

### Run

```
.\main.exe
```

---

# 🎮 Controls

| Key         | Action     |
| ----------- | ---------- |
| Enter       | Start Game |
| Left Arrow  | Chop Left  |
| Right Arrow | Chop Right |
| Escape      | Quit Game  |

---

# 🛠 Built With

* **C++**
* **SFML 2.6**
* **GCC / g++**

---

# 📌 Future Improvements

* Add scoring leaderboard
* Add game menu
* Add sound settings
* Improve animations

---