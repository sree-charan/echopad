# Echopad Collaborative Text Editor

A simple, powerful, and self-hostable real-time collaborative code editor built with **Firepad**, **CodeMirror**, and **Firebase**. This project provides a clean, modern, and mobile-friendly interface for seamless collaborative coding.

## 🚀 Features

- **Real-Time Collaboration:** Powered by Firepad and Firebase Realtime Database for true, low-latency, character-by-character synchronization.
- **Syntax Highlighting:** Supports multiple languages out of the box, including JavaScript, Python, HTML, and CSS.
- **Customizable Themes:** Easily switch between light and dark editor themes.
- **Mobile Friendly:** Responsive design works on both desktop and mobile devices, with an auto-hiding header on mobile to maximize screen space.
- **Easy Document Sharing:** Automatically generates short, shareable URLs for each new document.
- **Essential Editor Tools:** Includes one-tap buttons for creating a new document, copying the share link, clearing the document, and selecting/copying all content.
- **Zero Backend Code:** The entire application is a single `index.html` file that runs client-side, making it incredibly easy to deploy.

## ✨ How to Use

The user interface is designed to be simple and intuitive:

- **New:** Instantly creates a new document with a fresh, unique URL.
- **Copy Link:** Copies the URL of the current document to your clipboard so you can share it with others.
- **Select & Copy:** A mobile-friendly utility that reliably selects all text in the editor and copies it to your clipboard in one tap.
- **Clear:** Deletes all content in the current document for all collaborators.
- **Lang:** Dropdown to change the syntax highlighting for the current document.
- **Theme:** Dropdown to switch between light and dark themes.

## 🛠️ Setup & Deployment

Getting your own instance of this editor running is simple:

### Step 1: Create a Firebase Project

1. Go to the [Firebase Console](https://console.firebase.google.com/) and create a new project.
2. In the **Build** menu on the left, click **Realtime Database**.
3. Click **Create Database**, select a server location, and start in **Test mode** (you can secure your database later with security rules if needed).

### Step 2: Get Your Firebase Configuration

1. In your Firebase project, go to **Project settings** (gear icon at the top of the left menu).
2. Scroll down to the **Your apps** section.
3. Click the **Web** icon (</>) to create a new web app.
4. Give it a nickname (e.g., `Firepad Editor`) and click **Register app**.
5. Firebase will display a `firebaseConfig` object — copy this entire object.

### Step 3: Configure and Deploy

1. Open the `index.html` file.
2. Find the `firebaseConfig` object in the `<script>` section.
3. Paste your own configuration object over the placeholder.
4. Save the file.
5. Deploy the single `index.html` file to any static hosting provider, e.g.:
   - [Firebase Hosting](https://firebase.google.com/docs/hosting)
   - [Netlify](https://www.netlify.com/)
   - [Vercel](https://vercel.com/)
   - [GitHub Pages](https://pages.github.com/)

Your collaborative editor is now live!

---

Enjoy seamless collaborative coding with your own hosted Firepad editor.
