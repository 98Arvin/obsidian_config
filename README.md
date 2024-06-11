# Obsidian Configuration - Zettelkasten template

This repository contains the `.obsidian` folder with my preferred configurations for an Obsidian vault, tailored to utilize the Zettelkasten method for efficient note-taking and knowledge management.

## What is the Zettelkasten Method?

The Zettelkasten method is a powerful system for organizing and linking notes, originally developed by the German sociologist Niklas Luhmann. The term "Zettelkasten" translates to "slip box" or "note box," which captures the essence of the method: a collection of notes (or "slips") that are interconnected to form a web of knowledge.

### Key Features of the Zettelkasten Method:

- **Linking:** Each note is linked to related notes, creating a network of ideas that mirror the way our brains think.
- **Tagging:** Notes are tagged with relevant keywords to facilitate quick retrieval and context-building.
- **Referencing:** Notes reference other notes, sources, or ideas, providing a comprehensive view of a topic.
- **Daily Notes:** Regular note-taking habits are encouraged through daily notes, which help in capturing fleeting thoughts and ideas.
- **Search Functions:** Powerful search capabilities allow for quick access to notes, enhancing the ability to draw connections between ideas.

## Installation Instructions

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
    git clone https://internal-repo.basefarm.com/adoriani/obsidian_config.git .obsidian
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
    git clone https://internal-repo.basefarm.com/adoriani/obsidian_config.git .obsidian
    ```

By utilizing the Zettelkasten method in Obsidian, this configuration aims to create a highly organized and interconnected note-taking system, enhancing your ability to manage and develop complex ideas effectively.


## Obsidian Git setup instructions

### Step 1: Generate an SSH Key (if not already done)
1. Open a terminal.
2. Run the command:
   ```sh
   ssh-keygen -t ed25519 -C "$USER@ldap.basefarm.net"
   ```
3. Press `Enter` to save the key in the default location.
4. Press `Enter` to skip the passphrase.

### Step 2: Add the SSH Key to GitLab (if not already done)
1. Run the command to display your SSH key:
   ```sh
   cat ~/.ssh/id_ed25519.pub
   ```
2. Copy the output.
3. Go to GitLab and log in.
4. Navigate to **User Settings > SSH Keys**.
5. Paste your SSH key into the "Key" field and add a title.
6. Click **Add key**.

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
1. Add your existing GitLab repository as a remote:
   ```sh
   git remote add origin git@gitlab.com:your-username/your-repo.git
   ```

### Step 5: Commit and Push Your Vault to GitLab
1. Stage all files:
   ```sh
   git add .
   ```
2. Commit the changes:
   ```sh
   git commit -m "Add existing Obsidian vault"
   ```
3. Push to GitLab:
   ```sh
   git push -u origin main
   ```

### Step 6: Set Up Obsidian Git Plugin
1. Open Obsidian.
2. Go to **Settings > Community plugins** and ensure **Safe mode** is off.
3. Click **Browse** and search for **Obsidian Git**.
4. Install and enable the plugin.
5. Go to **Settings > Obsidian Git** and configure it as needed (e.g., set up auto-pull, auto-push).

### Summary of Commands:
1. Generate SSH key (if needed):
   ```sh
   ssh-keygen -t ed25519 -C "$USER@ldap.basefarm.net"
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
   git remote add origin git@gitlab.com:your-username/your-repo.git
   ```
5. Commit and push:
   ```sh
   git add .
   git commit -m "Add existing Obsidian vault"
   git push -u origin main
   ```

