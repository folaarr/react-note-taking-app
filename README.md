# 📝 React Note-Taking App

A note-taking application built with **React** and **Material UI**.  
👉 [Live Demo](https://folaarr.github.io/react-note-taking-app/)

---

## 🚀 Features

- ➕ Create new notes with a title and content  
- 🗑️ Delete notes instantly  
- 🎨 Responsive and clean UI styled with CSS + Material UI  
- 📱 Mobile-friendly layout  
- ⚡ Interactive animations with Material UI’s Zoom & Fab  

---

## 📂 Project Structure

    react-note-taking-app/
    ├── public/
    │ ├── index.html # Base HTML structure
    │ ├── styles.css # Global styles
    │ └── favicon.ico # App icon
    │
    ├── src/
    │ ├── components/
    │ │ ├── App.jsx # Main app logic (state + rendering notes)
    │ │ ├── Header.jsx # Top navigation with app title
    │ │ ├── Footer.jsx # Footer with copyright
    │ │ ├── Note.jsx # Individual note component
    │ │ └── CreateArea.jsx # Input form for adding notes
    │ │
    │ └── index.js # Entry point, renders <App />
    │
    ├── package.json # Dependencies and scripts
    └── README.md # Project documentation


---

## 📘 Code Overview

### `App.jsx`
- Manages **state** for all notes  
- `addNote()` → Adds a new note  
- `deleteNote()` → Removes a note by ID  

### `CreateArea.jsx`
- Handles note creation  
- Expands input area on click  
- Uses **Material UI** components:
  - `Fab` (Floating Action Button)  
  - `Zoom` animation  
  - `AddIcon`  

### `Note.jsx`
- Displays individual notes  
- Includes delete button with **DeleteIcon** from **Material UI** 

### `Header.jsx`
- Styled header with **EditNoteIcon** from **Material UI** 

### `Footer.jsx`
- Dynamic footer with the current year  

---

## 🛠️ Installation & Setup

Clone the repo and install dependencies:
```bash
git clone https://github.com/folaarr/react-note-taking-app.git
cd react-note-taking-app
npm install
```

Run locally:
```bash
npm start
```

Open in your browser:
```
http://localhost:3000
```

## 🌐 Deployment (GitHub Pages)

This project is hosted on **GitHub Pages** at:  
➡️ [https://folaarr.github.io/react-note-taking-app/](https://folaarr.github.io/react-note-taking-app/)

### Deployment steps:

**1. Build for production:**
```bash
npm run build
```

**2. Add the following to your `package.json`:**
```json
"homepage": "https://<your-github-username>.github.io/<your-repo-name>"
```

**3. Install the GitHub Pages package:**
```
npm install --save gh-pages
```

**4. Add deploy scripts in `package.json`:**
```
"scripts": {
  "predeploy": "npm run build",
  "deploy": "gh-pages -d build"
}
```

**5. Run deployment:**
```
npm run deploy
```
This will publish the production build to the gh-pages branch, which GitHub Pages serves automatically.


## 📦 Dependencies

- **React** (UI framework)  
- **Material UI** (`@mui/material`, `@mui/icons-material`)  
- **Create React App** (project setup)  


