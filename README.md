Firepad Collaborative Editor
A simple, powerful, and self-hostable real-time collaborative code editor built with Firepad, CodeMirror, and Firebase. This project provides a clean, modern, and mobile-friendly interface for seamless collaborative coding.

Features
Real-Time Collaboration: Powered by Firepad and Firebase Realtime Database for true, low-latency, character-by-character synchronization.

Syntax Highlighting: Supports multiple languages out of the box, including JavaScript, Python, HTML, and CSS.

Customizable Themes: Easily switch between light and dark editor themes.

Mobile Friendly: A responsive design that works on both desktop and mobile devices, with an auto-hiding header on mobile to maximize screen space.

Easy Document Sharing: Automatically generates short, shareable URLs for each new document.

Essential Editor Tools: Includes one-tap buttons for creating a new document, copying the share link, clearing the document, and selecting/copying all content.

Zero Backend Code: The entire application is a single index.html file that runs client-side, making it incredibly easy to deploy.

How to Use
The user interface is designed to be simple and intuitive:

New: Instantly creates a new document with a fresh, unique URL.

Copy Link: Copies the URL of the current document to your clipboard so you can share it with others.

Select & Copy: A mobile-friendly utility that reliably selects all text in the editor and copies it to your clipboard in one tap.

Clear: Deletes all content in the current document for all collaborators.

Lang: A dropdown menu to change the syntax highlighting for the current document.

Theme: A dropdown menu to switch between the editor's visual themes.

Setup & Deployment
Getting your own instance of this editor running is simple.

Step 1: Create a Firebase Project
Go to the Firebase Console and create a new project.

In the "Build" menu on the left, click Realtime Database.

Click Create Database, select a server location, and start in Test mode. (You can secure your database later with security rules if needed).

Step 2: Get Your Firebase Configuration
In your Firebase project, go to Project settings (click the gear icon at the top of the left menu).

Scroll down to the "Your apps" card.

Click the Web icon (</>) to create a new web app.

Give it a nickname (e.g., "Firepad Editor") and click Register app.

Firebase will display a firebaseConfig object. Copy this entire object.

Step 3: Configure and Deploy
Open the index.html file.

Find the firebaseConfig object in the <script> section.

Paste your own configuration object over the placeholder.

Save the file.

Deploy the single index.html file to any static hosting provider (Firebase Hosting, Netlify, Vercel, GitHub Pages, etc.).

Your collaborative editor is now live!