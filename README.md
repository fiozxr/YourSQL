# YourSQL ⚡

![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
![Platform](https://img.shields.io/badge/Platform-Web%20%7C%20Mobile-blue)
![Stack](https://img.shields.io/badge/Stack-HTML%20%7C%20JS%20%7C%20SQLite-yellow)

**YourSQL** is a lightning-fast, zero-dependency, fully local SQL IDE that runs entirely in your browser. 

# WEB
https://fiozxr.github.io/YourSQL

No backend. No server installations. No heavy desktop clients. Just a single `.html` file that spins up a persistent SQLite environment instantly, whether you're on a desktop or an Android phone.

## 🎯 Why YourSQL?
I built YourSQL and released it under the **MIT License** because nobody should have to waste time building another practice environment or downloading bloated 500MB+ database engines just to test a few queries. 

Whether you are studying database management, testing out cybersecurity payloads, or just need a scratchpad for relational data, YourSQL gives you a fully functional IDE in milliseconds and if there any issues, don't hesitate to fix by yourself or pull a request.

## ✨ Features

* 🚫 **Zero Setup & Serverless:** Powered by `sql-asm.js`. It runs entirely client-side, bypassing local file restrictions on Android and desktop browsers.
* 💾 **Persistent Memory:** Closes the tab? Your data is safe. The app serializes your database and auto-saves it directly to your browser's LocalStorage after every successful execution.
* 🌑 **Aesthetic Dark Mode:** Built with a minimalist `#121212` "True Dark" UI. High contrast, zero clutter, and easy on the eyes for long coding sessions.
* 🌳 **Database Explorer (Tree View):** A built-in visual file manager. Instantly map out your schema, inspect tables, view columns, data types, and primary keys.
* 🔄 **Import & Export .sql:** Easily dump your entire database structure and data into a standard `.sql` text file, or import existing `.sql` files to rebuild your tables instantly.
* 📱 **Fully Responsive:** Flexbox-driven UI that scales perfectly from ultra-wide desktop monitors to mobile phone screens.

## 🚀 How to Use

1. **Download** the `index.html` file (or clone this repository).
2. **Open** it in any modern web browser (Chrome, Firefox, Brave, etc.).
3. **Write** your queries.

### Basic Workflow Example:
```sql
-- 1. Create a table
CREATE TABLE users (
    id INT PRIMARY KEY,
    username VARCHAR NOT NULL,
    role VARCHAR DEFAULT 'user'
);

-- 2. Insert data (App auto-saves to LocalStorage here)
INSERT INTO users (id, username, role) VALUES (1, 'admin_fiozxr', 'superadmin');

-- 3. View the data in the dynamic CSS grid
SELECT * FROM users;
```
#🛠️ Tech Stack & Architecture

 * Frontend: Pure HTML5 and Vanilla JavaScript. No React, no Vue, zero build steps.
 * Styling: Custom CSS3 with CSS Variables for dynamic theme management.
 * Database Engine: sql.js (SQLite compiled to JavaScript).
 * Storage Mechanism: Base64 serialization paired with Web Storage API (localStorage).

#📜 License

What Licensing, what was that ?
No rights reserved. contribute 
