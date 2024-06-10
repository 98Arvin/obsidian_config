# Obsidian Configuration Repository

This repository contains the `.obsidian` folder with my preferred configurations for an Obsidian vault.

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
2. Removobsidian` folder:
    ```bash
    rm -r .obsidian
    ```
3. Clone this repe the current `.ository to set up the new `.obsidian` folder:
    ```bash
    git clone https://internal-repo.basefarm.com/adoriani/obsidian_config.git .obsidian
    ```
