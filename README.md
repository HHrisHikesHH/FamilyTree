## FamilyTree – Interactive Family Tree Web App

This repository contains a single-page web app for visualizing and editing your family tree using `index.html` and `family.json`.

### How to open the app

- **Option 1 – Open from file system**
  - Clone or download this repo to your computer.
  - Open `index.html` directly in a modern browser (Chrome, Edge, Firefox, Safari) by double‑clicking it or using `File → Open`.

- **Option 2 – Use GitHub Pages (recommended)**
  - In GitHub, go to **Settings → Pages** for this repo.
  - Under **Source**, choose the branch (e.g. `main`) and root folder `/` and save.
  - After a minute or two, GitHub will give you a link like `https://<your-username>.github.io/<repo-name>/index.html`.
  - **Share that link** with your family; they can open it on any device.

### How to use it

- **Unlock / view-only**
  - When the page loads, you will see a lock screen.
  - Enter the edit password to **add / edit people**, or click “Just browse (view only)” to look around without changing data.
  - The default password is `family2024` (you can change it in the code or via the settings screen in the app).

- **Editing your tree**
  - Click the **+** button (in the header) to add a new person, with name, nickname, parents, spouses, years, place and notes.
  - Click on any person card or timeline entry to see full details and (in edit mode) an **Edit** button.
  - Use the **Tree / Timeline** tabs in the header to switch between views.

- **Saving your data**
  - The app automatically saves to your browser’s **local storage**, so your changes stay on that device.
  - You can click **⬇️ Export JSON** in Settings to download your current `family.json`.

- **Optional: Auto‑save to GitHub**
  - Open **Settings (⚙️)** and fill in your:
    - GitHub username
    - Repository name (this repo)
    - Branch (e.g. `main`)
    - A personal access token
  - Each time you click **💾 Save**, the app will commit the latest `family.json` back to this repo using the GitHub API.

### GitHub token scope (for this app)

For a token that will **only update `family.json` in this repo**, give it **minimal repo contents access**:

- If you are using **fine‑grained tokens (recommended)**:
  - Limit it to **this repository only**.
  - In **Repository permissions → Contents**, select **Read and write**.

- If you are using **classic tokens** and the only option is broad scopes:
  - You must select **`repo`** (full control of private repositories) for the GitHub Contents API to allow file updates.
  - Do **not** enable any of the extra org / admin scopes unless you truly need them.

