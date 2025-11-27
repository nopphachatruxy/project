# 📚 Vocabulary Quiz Generator

A simple web-based quiz application to test your English vocabulary knowledge.

![Quiz Screenshot](./screenshots/preview.png)

---

## 📋 Table of Contents

- [Features](#-features)
- [Demo](#-demo)
- [Installation](#-installation)
- [How to Run](#-how-to-run)
- [Project Structure](#-project-structure)
- [Technologies Used](#-technologies-used)
- [How It Works](#-how-it-works)

---

## ✨ Features

- ✅ **60+ English vocabulary words** with definitions
- ✅ **Randomized questions** - different order every time
- ✅ **Multiple choice format** - 4 options per question
- ✅ **Instant feedback** - see if you're correct immediately
- ✅ **Score tracking** - track your progress in real-time
- ✅ **Responsive design** - works on desktop and mobile
- ✅ **No installation required** - runs in any modern browser

---

## 🌐 Demo

**Live Demo:** [https://[your-username].github.io/VocabularyQuizGenerator](https://[your-username].github.io/VocabularyQuizGenerator)

*(Replace `[your-username]` with your GitHub username after deployment)*

---

## 💻 Installation

### Option 1: Clone from GitHub

```bash
# Clone the repository
git clone https://github.com/[your-username]/VocabularyQuizGenerator.git

# Navigate to the project folder
cd VocabularyQuizGenerator/04_Implementation/src
```

### Option 2: Download ZIP

1. Click the green **"Code"** button on GitHub
2. Select **"Download ZIP"**
3. Extract the ZIP file
4. Navigate to `04_Implementation/src` folder

---

## 🚀 How to Run

### Method 1: Direct Open (Simplest)

1. Navigate to `04_Implementation/src` folder
2. Double-click `index.html`
3. The app will open in your default browser

### Method 2: Using Live Server (VS Code)

1. Install **Live Server** extension in VS Code
2. Open the `src` folder in VS Code
3. Right-click on `index.html`
4. Select **"Open with Live Server"**

### Method 3: Using Python (if installed)

```bash
# Navigate to src folder
cd 04_Implementation/src

# Python 3
python -m http.server 8000

# Then open http://localhost:8000 in your browser
```

### Method 4: Using Node.js (if installed)

```bash
# Install serve globally
npm install -g serve

# Navigate to src folder
cd 04_Implementation/src

# Run server
serve

# Open the URL shown in terminal
```

---

## 📁 Project Structure

```
VocabularyQuizGenerator/
├── 01_Requirements/
│   ├── Scope_Document.md
│   └── User_Stories.md
├── 02_UX_UI_Design/
│   ├── Prototype/
│   │   └── prototype.html
│   └── Design_Rationale.md
├── 03_System_Design/
│   ├── Architecture_Diagram.html
│   ├── Data_Model_Diagram.html
│   └── Technology_Stack_Justification.md
├── 04_Implementation/
│   └── src/
│       ├── index.html          # Main HTML file
│       ├── css/
│       │   └── style.css       # Stylesheet
│       └── js/
│           ├── data.js         # Vocabulary database (60 words)
│           └── app.js          # Application logic
├── 05_Testing/
│   ├── Test_Case_Report.md
│   └── Test_Evidence/
├── 06_Deployment_Review/
│   ├── User_Manual.md
│   └── Presentation_Slides.pdf
├── README.md                    # This file
└── .gitignore
```

---

## 🛠 Technologies Used

| Technology | Purpose |
|------------|---------|
| **HTML5** | Structure and content |
| **CSS3** | Styling and animations |
| **JavaScript (ES6+)** | Application logic |
| **GitHub Pages** | Hosting (free) |

### No External Dependencies!

This project uses **vanilla JavaScript** with no frameworks or libraries required.

---

## ⚙️ How It Works

### Quiz Flow

1. **Start Screen** - User clicks "Start Quiz"
2. **Question Screen** - Shows vocabulary word and 4 definition options
3. **Answer Feedback** - Immediately shows if answer was correct/wrong
4. **Next Question** - User proceeds to next question
5. **Result Screen** - Shows final score and statistics
6. **Try Again** - Option to restart with new randomized questions

### Key Functions

| Function | Description |
|----------|-------------|
| `startQuiz()` | Initializes a new quiz with randomized questions |
| `generateQuestions()` | Creates 10 random questions from word database |
| `selectOption(index)` | Handles user's answer selection |
| `nextQuestion()` | Moves to the next question |
| `showResults()` | Displays final score and statistics |

### Data Structure

```javascript
// Each vocabulary word is stored as:
{
    word: "ABUNDANT",
    definition: "Existing in large quantities; plentiful"
}

// Each question is generated as:
{
    word: "ABUNDANT",
    correctAnswer: "Existing in large quantities; plentiful",
    options: ["definition1", "definition2", "definition3", "definition4"],
    correctIndex: 2  // Index of correct answer in options array
}
```

---

## 📝 License

This project is created for educational purposes as part of a Software Engineering course.

---

## 👤 Author

- **Name:** [ใส่ชื่อนักศึกษา]
- **Student ID:** [ใส่รหัสนักศึกษา]
- **Course:** Software Engineering Final Project

---

## 🙏 Acknowledgments

- Course instructor for project guidance
- English vocabulary sourced from common academic word lists
