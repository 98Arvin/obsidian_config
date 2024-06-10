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
