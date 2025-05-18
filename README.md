# Gloation: A Custom Notion Theme

## Overview
Gloation is a professional dark-mode theme for Notion, built upon the framework developed by [u/CarbonGhost0](https://www.reddit.com/user/CarbonGhost0/). This documentation provides installation instructions and customisation options for implementing the theme in your Notion workspace.

**Note:** This theme requires Notion's dark mode to be enabled for proper functionality.

## Preview
![Interface Example 1](https://i.imgur.com/eTOyja0.png)
![Interface Example 2](https://i.imgur.com/VZHWF4J.png)
![Interface Example 3](https://i.imgur.com/oxy8oX6.png)

## Important Considerations
Before installation, please be aware of the following limitations:

- Manual update process (no automatic updates)
- Potential brief performance delays when opening or closing the application
- Theme initialisation may take a few seconds upon launch
- Occasional theme loading inconsistencies (approximately 2% of launches)
- Additional configuration required for Windows search integration

## Installation Guide

### Prerequisites
- Windows operating system
- Administrator privileges

### Step-by-Step Installation

1. **Install Node.js**
   - Download [Node.js](https://nodejs.org/en/) (select "Current" version if unsure)
   - Complete the installation and restart your computer

2. **Set Up Development Environment**
   - Navigate to your desktop in File Explorer
   - Click in the address bar, type "cmd" and press Enter to open Command Prompt
   - Install Nativefier by running: `npm install nativefier -g`

3. **Create Notion Application**
   - In the Command Prompt, run:
     ```
     nativefier --name "Notion" "https://notion.so" --inject "./inject.css" --inject "./inject.js"
     ```

4. **Install Theme Files**
   - Navigate to: `desktop\notion\Notion-win32-x64\resources\app\inject`
   - Download the repository using one of these methods:
     - Git command: `git clone https://github.com/iJynx/gloation.git`
     - Manual download: Extract the ZIP file into this directory
   - Verify that the following files exist in the directory:
     - inject.js (default file)
     - inject.css (from Gloation)
     - README.md (from Gloation)

5. **Create Application Shortcuts**
   - Return to `desktop/notion`
   - Pin `Notion.exe` to your taskbar, Start menu, or desktop for easy access

## Customisation Options

### Custom Background Image
1. Open `inject.css` with a text editor
2. Locate the line: `background-image: url('IMAGE-URL-HERE') !important;`
3. Replace 'IMAGE-URL-HERE' with the URL of your preferred image
4. Ensure the URL points directly to an image file (typically ending in .jpg, .png, etc.)
5. Maintain the quotation marks around the URL

### Advanced Customisation
- For JavaScript customisations: Modify `inject.js` and reload Notion
- For CSS customisations: Modify `inject.css` and restart the application

## Troubleshooting
If you encounter issues during installation or use:

1. Review the [original documentation](https://www.reddit.com/r/Notion/comments/ho2hu5/custom_electron_wrapper_cssjs_injection_details/fxf1e86?utm_source=share&utm_medium=web2x&context=3) for potential solutions
2. Submit an issue on the GitHub repository
3. Contact support at: iJynx@protonmail.com

## Acknowledgements
This theme was inspired by previous customisation work and built upon the foundation created by the Notion community.
