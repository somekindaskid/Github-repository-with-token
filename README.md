# 🌌 Starry GitHub Repository File Viewer

A simple **HTML + CSS + JavaScript** webpage that uses the **GitHub REST API** to display the contents of a GitHub repository directly in the browser.

It lists all files and folders in the repo, and if the item is a file, it downloads and displays the file content on the page.  
It also includes a **space-themed animated star background**.

---

## ✅ Features

- 📂 Lists repository contents (files + folders)
- 📄 Automatically fetches and displays file contents
- 🌌 Animated star background effect
- 🔑 Supports GitHub API authentication using a token
- 🖥️ Runs fully in the browser (no backend required)

---

## 🛠️ Built With

- **HTML** (structure)
- **CSS** (styling + animations)
- **JavaScript** (GitHub API fetching)

---

## ⚙️ How It Works

The project uses this GitHub API endpoint:

`https://api.github.com/repos/<USER>/<REPO>/contents/`

It loops through each item returned from the API:

- If the item is a **folder**, it gets displayed as a folder entry
- If the item is a **file**, the code fetches `download_url` and prints the file text inside a `<pre>` block

---

## 🚀 How To Run

1. Save the code as:

`index.html`

2. Open the file in your browser.

---

## ⚠️ IMPORTANT: Token Warning

**Do NOT upload your GitHub token into a public repository.**

If your token is leaked, anyone can use it depending on the permissions it has.

✅ Safer options:
- Use public repos and remove the token
- Use a backend server to hide the token securely
- Limit permissions when generating the token in GitHub

---

## 📌 Notes

This project is mainly for learning/testing how the GitHub API works using a front-end only HTML project.
