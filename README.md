# 🐻 Bear Type Scorer

## 📝 Overview

**Bear Type Scorer** is a sleek, feature-rich typing test application designed for developers and anyone looking to boost their Words Per Minute (WPM) speed and accuracy. Built entirely with **HTML, CSS, and vanilla JavaScript**, it runs directly in the browser with no server dependencies.

The application features real-time performance tracking, a history of past scores, configurable test durations, and modern quality-of-life features like automatic text scrolling and a fun exit animation.

***

## ✨ Key Features

* **Real-time WPM & Accuracy:** Track your performance instantly as you type.
* **Speed Meter:** A dynamic speed bar and message system provide instant feedback on your current pace (e.g., "BLAZING FAST!").
* **Configurable Timer:** Adjust the test duration using a slider from 15s up to 120s.
* **Local History Tracking:** Saves your past test results (WPM, Accuracy, and a progress chart) to local storage.
* **WPM Progression Chart:** A detailed line chart in the results modal shows your WPM progression over the course of the test using **Chart.js**.
* **Seamless Autoscroll 🚀 (Bug Fix Implemented):** The typing area automatically scrolls up to reveal the next line of text once the cursor reaches the third visible line, ensuring your focus remains centered.
* **Fun Exit Animation:** Clicking the "Close" button on the results modal triggers a "fly away" animation of the entire application before attempting to close the browser tab.

***

## 🚀 Getting Started

This project is a single-file application and is incredibly easy to set up.

### Prerequisites

You only need a modern web browser (Chrome, Firefox, Edge, Safari).

### Installation & Usage

1.  **Clone the repository** (or download the file):
    ```bash
    git clone [https://github.com/your-username/bear-type-scorer.git](https://github.com/your-username/bear-type-scorer.git)
    ```
2.  **Open the file:** Navigate to the cloned directory and open the `index.html` (or similar) file directly in your web browser.

    ```bash
    # Assuming the main file is named index.html
    open index.html 
    ```
3.  **Start Typing!** The application is ready to use immediately.

***

## 🕹️ How to Play

1.  **Set Username:** Upon first launch, enter a username to personalize the experience and save your scores.
2.  **Select Duration:** Use the **Test Duration** slider to choose a time limit (default is 60s).
3.  **Start Typing:** Click the **"Start Test"** button or simply begin typing the first word.
4.  **Error Correction:** The application does *not* allow you to use the `Backspace` key. Correct letters turn **white**, incorrect letters flash **red**. You must type the correct character to advance the cursor.
5.  **Finish:** The test automatically ends when the timer runs out.
6.  **Review Results:** The **Results Modal** pops up with your final WPM, Accuracy, and a detailed progression chart.

***

## 💻 Project Structure

The entire application is contained within a single HTML file, leveraging the simplicity of a standalone tool.

***

## 🛠️ Technology Stack

| Component | Technology | Description |
| :--- | :--- | :--- |
| **Markup** | HTML5 | Structure of the application. |
| **Styling** | CSS3 | Custom dark theme styling and keyframe animations. |
| **Logic** | JavaScript (Vanilla) | All game logic, state management, scoring, and local storage persistence. |
| **Charting** | Chart.js | Used for rendering the WPM Progression line graph in the results modal. |

***

## 💡 Future Enhancements

* **Custom Text/Quote Mode:** Allow users to paste their own text for typing practice.
* **Punctuation and Numbers Mode:** Option to include more complex characters.
* **Multiplayer/Challenge Mode:** Implement a simple real-time challenge feature using a database/backend.
* **User Settings:** Add persistent settings for theme colors or preferred font size.

***

## ⚠️ Note on `window.close()`

For security purposes, modern web browsers restrict JavaScript from closing a window or tab unless that window/tab was opened by the same script (e.g., using `window.open()`).

The **Close** button in this application attempts to close the tab after the animation using `window.close()`. If the tab was opened manually, this may fail, and the user will have to close the tab manually after the animation completes.
