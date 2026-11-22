Learn To Live Academy — Website Package
=========================================

FOLDER STRUCTURE
-----------------
learn-to-live-academy/
├── index.html                  ← Main website file
├── data/
│   ├── settings.json           ← Academy + teacher + contact info
│   ├── banners.json            ← Hero slider banners
│   └── courses.json            ← Course list
└── assets/
    └── images/
        ├── logo.png            ← Academy logo
        ├── teacher.png         ← Teacher photo
        ├── banners/
        │   ├── banner1.jpg
        │   ├── banner2.jpg
        │   └── banner3.jpg
        └── courses/
            ├── math.jpg
            ├── science.jpg
            └── english.jpg


HOW TO USE
----------

1. EDIT CONTENT
   - Open the files in data/ folder with any text editor
   - Change names, phone number, address, course info, etc.
   - The _en fields are for English version (optional)

2. REPLACE IMAGES
   - Replace the placeholder images in assets/images/ with your real photos
   - Keep the same file names, or update the paths in the JSON files
   - Suggested sizes:
     * logo.png       → 128 x 128 px (square)
     * teacher.png    → 800 x 1000 px (portrait, 4:5)
     * banner*.jpg    → 1920 x 1080 px (landscape)
     * course *.jpg   → 800 x 500 px (landscape, 16:10)

3. TEST LOCALLY
   The website uses fetch() to load JSON files, which does NOT work
   when opening index.html directly with file:// protocol.

   Use ONE of these methods:

   a) VS Code Live Server (easiest):
      - Install "Live Server" extension in VS Code
      - Right-click index.html → "Open with Live Server"

   b) Python HTTP server:
      - Open terminal in this folder
      - Run:  python3 -m http.server 8000
      - Open browser: http://localhost:8000

4. DEPLOY TO GITHUB PAGES
   - Create a new repository on GitHub
   - Upload all files (keep the folder structure)
   - Go to: Settings → Pages
   - Source: Deploy from branch
   - Branch: main / (root)
   - Save. Your site will be live in ~1 minute.

   All paths are relative, so it works under repository subpaths too.


FEATURES
--------
- Dark / Light theme toggle (saved in browser)
- Bengali / English language switch (saved in browser)
- Hero slider with autoplay
- Dynamic courses from JSON
- WhatsApp integration with auto-encoded messages
- Fully responsive (mobile, tablet, desktop)
- No backend, no database — pure static site


NEED HELP?
----------
Edit the JSON files to change any content. The website automatically
reads from them on every page load.
