# 🎲 Simple Dice and Flip Bottle Games

> Two classic Android games — Dice and Spin the Bottle — combined in one project.

[![Kotlin](https://img.shields.io/badge/Kotlin-1.7.10-blue.svg?logo=kotlin)](https://kotlinlang.org)
[![API](https://img.shields.io/badge/API-21%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=21)
[![GitHub stars](https://img.shields.io/github/stars/DiyorbekJDK/SimpleDiceAndFlipBottleGames)](https://github.com/DiyorbekJDK/SimpleDiceAndFlipBottleGames/stargazers)
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/DiyorbekJDK/SimpleDiceAndFlipBottleGames/blob/master/LICENSE)

---

## 📱 About the Project

**Simple Dice and Flip Bottle Games** is an Android application that includes two mini-games for two players: dice rolling and spin the bottle (or spinning top).

The app was built with **Kotlin** in **Android Studio** using the **Konfetti** animation library to create a festive confetti effect when a player wins.

This project is ideal for beginner Android developers who want to explore animations, click handling, and simple game logic.

---

## ✨ Features

### 1. 🎲 Dice Game
- **Two players**: Players take turns rolling two six-sided dice.
- **Adjustable target**: Choose the winning score target (100, 200, or 300 points).
- **Confetti effect**: The winner is greeted with a festive confetti explosion.
- **Score tracking**: Keeps a running total for each player.
- **Restart option**: You can restart the game anytime during the match.

### 2. 🍾 Spin the Bottle Game
- **Random spin**: Tap the bottle (or spinner) to trigger a random rotation animation.
- **Simple controls**: Intuitive one-tap gameplay.

### 3. Common Features
- **Splash screen**: Smooth logo animation on launch.
- **Player name input**: Players can enter their names before starting.
- **Game selection menu**: Main menu to navigate between the two games.
- **Animations**: Smooth dice roll and bottle spin animations.
- **Material Design**: Uses modern Material Design components.

---

## 🛠 Technologies and Requirements

- **Min Android version**: API 21 (Android 5.0 Lollipop)
- **Target Android version**: API 32 (Android 12L)
- **Language**: Kotlin
- **Build tool**: Gradle
- **Key libraries**:
  - `androidx.core:core-ktx` — Kotlin extensions for Android.
  - `com.google.android.material:material` — Material Design components.
  - `nl.dionsegijn:konfetti-xml` — Confetti animation library.

---

## 📂 Project Structure

```text
app/
├── src/main/
│   ├── java/com/diyorbek/simplegames/
│   │   ├── models/                 # Data models
│   │   │   └── User.kt             # Player name model
│   │   ├── BoardActivity.kt        # Spin the bottle game logic
│   │   ├── EnterName.kt            # Enter player names screen
│   │   ├── LogosActivity.kt        # Logo screen
│   │   ├── MainActivity.kt         # Dice game main logic
│   │   ├── Menu.kt                 # Main menu for game selection
│   │   └── SplashActivity.kt       # Splash screen
│   └── res/                        # Resources (layouts, animations, images, etc.)
└── build.gradle                    # Project build files

```

## 🧠 How It Works

### Dice Game Logic (`MainActivity.kt`)
1. Players enter their names on the `EnterName` screen.
2. Choose the target winning score (100, 200, or 300).
3. Players take turns tapping a button to roll two dice.
4. Random numbers from 1 to 6 are generated for each die; their sum is added to the player's score.
5. When the score reaches or exceeds the target, the winner is declared and confetti animation starts.

### Spin the Bottle Logic (`BoardActivity.kt`)
1. Tapping the image triggers a rotation animation.
2. The rotation angle is chosen randomly using `Random()`.
3. While the animation is running, additional taps are blocked to avoid glitches.

---

## 🗺 Future Plans

- [ ] Add multi-language support (Russian, Uzbek, English).
- [ ] Implement saving of records and player statistics.
- [ ] Add sound effects for dice rolls and bottle spins.
- [ ] Improve bottle spin animation with a physics engine.
- [ ] Refactor code and extract reusable methods into utilities.

---

## 🤝 Contributing

If you’d like to contribute to the project, please follow these steps:

1. **Fork** the repository.
2. **Create a new branch** for your feature or fix (`git checkout -b feature/AmazingFeature`).
3. **Commit your changes** (`git commit -m 'Add some AmazingFeature'`).
4. **Push to the branch** (`git push origin feature/AmazingFeature`).
5. **Open a Pull Request** to the main repository.
