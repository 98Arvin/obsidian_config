# Obsidian Setup - Zettelkasten template

This repo has my`.obsidian` folder, set up specifically for the Zettelkasten method. If you're looking to streamline your note-taking and knowledge management in Obsidian, you're in the right place.

### What’s the Zettelkasten Method?

The Zettelkasten method is a powerful system for organizing and linking notes, originally developed by the German sociologist Niklas Luhmann. The term **Zettelkasten** translates to **slip box** or **note box**, which captures the essence of the method: a collection of notes _or slips_ that are interconnected to form a web of knowledge.

### Why Use the Zettelkasten Method?

- **No More Folders:** Forget about rigid folder structures. Each note is linked to others, creating a network of ideas.
- **Tagging:** Add relevant tags for easy retrieval and context.
- **Referencing:** Notes can reference other notes, ideas, or sources, building a connected knowledge base.
- **Daily Notes:** Capture thoughts and ideas regularly with daily notes.
- **Powerful Search:** Use Obsidian’s search to quickly find and connect related ideas—again, no need for folders.

## Hotkeys Overview

Here’s a list of the custom hotkeys for this Obsidian setup:

- **Delete File:** `Ctrl` + `Shift` + `Delete`
- **Insert Template:** `Alt` + `T`
- **Go Back:** `Alt` + `ArrowLeft`
- **Go Forward:** `Alt` + `ArrowRight`
- **Add Internal Link:** `Ctrl` + `L`
- **Toggle Left Sidebar:** `Alt` + `Z`
- **Toggle Right Sidebar:** `Alt` + `X`
- **Toggle Checklist Status:** `Ctrl` + `Shift` + `L`
- **Open Daily Notes:** `Alt` + `D`
- **Insert Code Block:** `Alt` + `C`
- **Omnisearch Vault Search:** `Alt` + `O`
- **Fold All:** `Alt` + `Shift` + `ArrowUp`
- **Unfold All:** `Alt` + `Shift` + `ArrowDown`
- **Add Metadata Property:** `Ctrl` + `\`

## Fonts

For the best experience with this Obsidian setup, you'll need to install the following fonts:

- **Interface Font:** [Cabin](https://fonts.google.com/specimen/Cabin)
- **Text Font:** [Crimson Pro](https://fonts.google.com/specimen/Crimson+Pro)
- **Monospace Font:** [Caskaydia Nerd Font](https://www.nerdfonts.com/font-downloads)

Once you’ve got these fonts installed, the Obsidian config will automatically use them, giving your setup a clean and polished vibe.

# Installation Instructions

### Preserving a Backup of Your Existing `.obsidian` Folder

To ensure you have a backup of your current `.obsidian` folder, follow these steps:

1. Navigate to your vault directory:
    ```bash
    cd /path/to/your/obsidian/vault
    ```
2. Create a backup of your current `.obsidian` folder:
    ```bash
    cp -r .obsidian previous_obsidian_configs
    ```
3. Clone this repository to replace your existing `.obsidian` folder:
    ```bash
    git clone https://github.com/98Arvin/obsidian_config.git .obsidian
    ```

### Replacing the Existing `.obsidian` Folder Without Backup

If you prefer to replace your existing `.obsidian` folder without keeping a backup, use the following commands:

1. Navigate to your vault directory:
    ```bash
    cd /path/to/your/obsidian/vault
    ```
2. Remove the current `.obsidian` folder:
    ```bash
    rm -r .obsidian
    ```
3. Clone this repository to set up the new `.obsidian` folder:
    ```bash
    git clone https://github.com/98Arvin/obsidian_config.git .obsidian
    ```

## Obsidian Git setup instructions

### Step 1: Generate an SSH Key (if not already done)
1. Open a terminal.
2. Run the command:
   ```sh
   ssh-keygen -t ed25519 -C "Obsidian"
   ```
3. Press `Enter` to save the key in the default location.
4. Press `Enter` to skip the passphrase.

### Step 2: Add the SSH Key to GitHub (if not already done)
1. Run the command to display your SSH key:
   ```sh
   cat ~/.ssh/id_ed25519.pub
   ```
2. Copy the output.
3. Go to GitHub and log in.
4. Navigate to **SSH and GPG keys > New SSH key**.
5. Paste your SSH key into the "Key" field and add a title.
6. Click **Add SSH key**.

### Step 3: Initialize Git in Your Existing Vault
1. Open a terminal.
2. Navigate to your existing Obsidian vault directory:
   ```sh
   cd /path/to/your/vault
   ```
3. Initialize Git:
   ```sh
   git init
   ```

### Step 4: Add the Remote Repository
1. Add your existing GitHub repository as a remote:
   ```sh
   git remote add origin git@github.com:your-username/your-repo.git
   ```

### Step 5: Commit and Push Your Vault to GitHub
1. Stage all files:
   ```sh
   git add .
   ```
2. Commit the changes:
   ```sh
   git commit -m "Add existing Obsidian vault"
   ```
3. Push to GitHub:
   ```sh
   git push -u origin main
   ```

### Step 6: Set Up Obsidian Git Plugin
1. Open Obsidian.
2. Go to **Settings > Community plugins** and ensure **Safe mode** is off.
3. Click **Browse** and search for **Obsidian Git**.
4. Install and enable the plugin.
5. Go to **Settings > Obsidian Git** and configure it as needed (e.g., set up auto-push).

### Summary of Commands:
1. Generate SSH key (if needed):
   ```sh
   ssh-keygen -t ed25519 -C "Obsidian"
   cat ~/.ssh/id_ed25519.pub
   ```
2. Navigate to your vault directory:
   ```sh
   cd /path/to/your/vault
   ```
3. Initialize Git:
   ```sh
   git init
   ```
4. Add remote repository:
   ```sh
   git remote add origin git@github.com:your-username/your-repo.git
   ```
5. Commit and push:
   ```sh
   git add .
   git commit -m "Add existing Obsidian vault"
   git push -u origin main
   ```
