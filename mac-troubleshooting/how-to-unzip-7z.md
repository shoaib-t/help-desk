# How to Unzip .7z Files on macOS Using 7za

## Step 1: Install Homebrew (if not already installed)

Homebrew is a package manager for macOS. To install it, run this command in your Terminal:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
For more info, visit https://brew.sh

## Step 2: Install p7zip using Homebrew
p7zip provides the 7za command-line tool to unzip .7z files.

Run this in Terminal:
```bash
brew install p7zip
```

## Step 3: Unzip the .7z file
Use the following command syntax:
```bash
7za x /path/to/your/file.7z -o/path/to/destination/folder
```

- Replace /path/to/your/file.7z with the full path to your .7z file.
- Replace /path/to/destination/folder with the folder where you want to extract the files.

### Example:
```bash
7za x ~/Downloads/example.7z -o~/Documents/unzipped-files
```
This extracts the contents of example.7z into the unzipped-files folder inside your Documents directory.

## Notes
- Make sure there is no space between -o and the destination path.
- If the destination folder does not exist, 7za will create it automatically.
