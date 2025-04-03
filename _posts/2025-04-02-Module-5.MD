---
layout: post
title:  "Module 5: Introduction to Text Editors and IDEs"
date:   2025-04-02 8:00:00
categories: Foundations
---

# Module 5: Introduction to Text Editors and IDEs

## Overview
This module introduces you to text editors and Integrated Development Environments (IDEs), the essential tools for writing and managing code. You'll learn about different options available, how to set up Visual Studio Code (VS Code), essential extensions for web development, and productivity-enhancing features and shortcuts that will make your coding more efficient.

## Learning Objectives
By the end of this module, you will be able to:
- Compare popular code editors and understand their strengths and limitations
- Install and configure VS Code for web development
- Install and use essential extensions that enhance your coding experience
- Use keyboard shortcuts and productivity features to code more efficiently

## Section 1: Comparing Popular Code Editors

### Text Editors vs. IDEs
Before diving into specific tools, it's important to understand the distinction:

#### Text Editors
- Lightweight applications focused on editing text files
- Faster startup and lower resource usage
- Usually extensible with plugins/extensions
- Examples: VS Code, Sublime Text, Atom, Notepad++

#### Integrated Development Environments (IDEs)
- Comprehensive development tools with built-in features
- Include compilers, debuggers, and advanced project management
- Higher resource usage but more powerful out-of-the-box
- Examples: WebStorm, Visual Studio, Eclipse, IntelliJ IDEA

### Popular Options for Web Development

#### Visual Studio Code (VS Code)
- **Developer**: Microsoft
- **Platforms**: Windows, macOS, Linux
- **License**: Free, open-source
- **Strengths**:
  - Excellent balance between performance and features
  - Huge extension ecosystem
  - Integrated terminal
  - Great Git integration
  - Regular updates and active development
  - Built-in IntelliSense (code completion)
- **Limitations**:
  - Can become resource-intensive with many extensions

#### Sublime Text
- **Developer**: Sublime HQ
- **Platforms**: Windows, macOS, Linux
- **License**: Paid (with unlimited free evaluation)
- **Strengths**:
  - Extremely fast and lightweight
  - Powerful text manipulation features
  - Distraction-free mode
  - Multiple selection and editing
- **Limitations**:
  - Fewer built-in features compared to VS Code
  - Paid license

#### WebStorm
- **Developer**: JetBrains
- **Platforms**: Windows, macOS, Linux
- **License**: Paid (free for students and open-source projects)
- **Strengths**:
  - Comprehensive built-in features for web development
  - Powerful refactoring tools
  - Advanced debugging capabilities
  - Deep framework integrations (React, Angular, Vue)
- **Limitations**:
  - Resource-intensive
  - Paid subscription

#### Atom
- **Developer**: GitHub (no longer actively developed)
- **Platforms**: Windows, macOS, Linux
- **License**: Free, open-source
- **Strengths**:
  - Highly customizable
  - Good Git integration
  - Hackable with JavaScript/CSS
- **Limitations**:
  - Development discontinued in 2022
  - Performance issues with large files

### Choosing the Right Editor
Consider these factors when selecting a code editor:
- Performance requirements and your computer's specifications
- Specific language or framework support needed
- Preference for built-in features vs. extensibility
- Budget constraints (free vs. paid options)
- Team/workplace standards or requirements

For this curriculum, we'll focus on VS Code as it has become the de facto standard for web development due to its balance of features, performance, and extensibility.

## Section 2: Setting Up VS Code

### Installation

#### Windows
1. Download the installer from the [VS Code website](https://code.visualstudio.com/)
2. Run the installer and follow the prompts
3. Ensure you select "Add to PATH" during installation

#### macOS
1. Download the .zip file from the [VS Code website](https://code.visualstudio.com/)
2. Extract and move the application to your Applications folder
3. Optionally, install the `code` command in PATH through the Command Palette (Cmd+Shift+P) by selecting "Shell Command: Install 'code' command in PATH"

#### Linux
1. Follow distribution-specific instructions on the [VS Code website](https://code.visualstudio.com/)
2. For Ubuntu/Debian: Use the package manager or download the .deb file
3. For Red Hat/Fedora: Download the .rpm file

### Initial Configuration

#### Interface Customization
1. **Theme**: File → Preferences → Color Theme (or Ctrl+K Ctrl+T)
2. **Icon Theme**: File → Preferences → File Icon Theme
3. **Font**: Customize in settings.json:
   ```json
   "editor.fontSize": 14,
   "editor.fontFamily": "Fira Code, Consolas, 'Courier New', monospace",
   "editor.fontLigatures": true  // If using a font with ligatures
   ```

#### Essential Settings
Open settings.json (File → Preferences → Settings → Edit in settings.json) and consider these settings:

```json
{
  "editor.formatOnSave": true,
  "editor.tabSize": 2,
  "editor.wordWrap": "on",
  "files.autoSave": "afterDelay",
  "files.autoSaveDelay": 1000,
  "workbench.startupEditor": "newUntitledFile",
  "explorer.confirmDelete": false,
  "editor.minimap.enabled": false,
  "workbench.editor.enablePreview": false
}
```

#### Integrated Terminal Setup
1. Configure your preferred terminal:
   - Windows: PowerShell, Git Bash, WSL
   - macOS/Linux: bash, zsh, fish
   
   Configure in settings.json:
   ```json
   "terminal.integrated.defaultProfile.windows": "Git Bash",
   "terminal.integrated.defaultProfile.osx": "zsh",
   "terminal.integrated.defaultProfile.linux": "bash"
   ```

2. Open the terminal: View → Terminal or Ctrl+`

### Working with Projects
- Open a folder: File → Open Folder
- Multi-root workspaces: File → Add Folder to Workspace
- Open recent projects: File → Open Recent

## Section 3: Essential Extensions for Web Development

### How to Install Extensions
1. Click the Extensions icon in the Activity Bar (or press Ctrl+Shift+X)
2. Search for extensions by name
3. Click "Install" on desired extensions

### Core Extensions for Web Development

#### HTML & CSS
- **HTML CSS Support**: Provides CSS class name completion
- **Auto Rename Tag**: Automatically renames paired HTML tags
- **CSS Peek**: Allows peeking at CSS definitions from HTML
- **HTML Snippets**: Provides snippets for HTML

#### JavaScript
- **ESLint**: JavaScript linting for code quality
- **Prettier**: Code formatter for consistent styling
- **JavaScript (ES6) Code Snippets**: Snippets for modern JavaScript
- **Quokka.js**: Live JavaScript playground in your editor

#### Frameworks and Libraries
- **ES7 React/Redux/GraphQL/React-Native snippets**: React snippets
- **Vetur/Volar**: Vue.js support
- **Angular Language Service**: Angular support
- **Svelte for VS Code**: Svelte support

#### General Development
- **Live Server**: Launch a development server with live reload
- **GitLens**: Enhanced Git capabilities
- **Path Intellisense**: Autocompletes filenames
- **IntelliSense for CSS class names**: CSS class name completion
- **Debugger for Chrome/Edge/Firefox**: Browser debugging

#### Themes and Appearance
- **Material Icon Theme**: File icons based on Material Design
- **One Dark Pro**: Popular dark theme
- **GitHub Theme**: Official GitHub themes

### Extension Management Best Practices
- Disable extensions you don't use regularly to improve performance
- Use workspace-specific extensions when appropriate
- Regularly update extensions
- Review extension permissions before installing

## Section 4: Basic Shortcuts and Productivity Features

### Essential Keyboard Shortcuts
Learning keyboard shortcuts can dramatically improve your coding speed and efficiency.

#### General
- **Ctrl+S** (Win/Linux) / **Cmd+S** (Mac): Save file
- **Ctrl+N** / **Cmd+N**: New file
- **Ctrl+P** / **Cmd+P**: Quick open file
- **Ctrl+Shift+P** / **Cmd+Shift+P**: Command Palette
- **Ctrl+,** / **Cmd+,**: Open Settings
- **Ctrl+`** / **Ctrl+`**: Toggle terminal
- **Ctrl+B** / **Cmd+B**: Toggle sidebar

#### Editing
- **Ctrl+X/C/V** / **Cmd+X/C/V**: Cut/Copy/Paste
- **Ctrl+Z** / **Cmd+Z**: Undo
- **Ctrl+Shift+Z** / **Cmd+Shift+Z**: Redo
- **Ctrl+F** / **Cmd+F**: Find
- **Ctrl+H** / **Cmd+H**: Replace
- **Alt+Up/Down** / **Option+Up/Down**: Move line up/down
- **Shift+Alt+Up/Down** / **Shift+Option+Up/Down**: Copy line up/down
- **Ctrl+/** / **Cmd+/**: Toggle line comment
- **Ctrl+D** / **Cmd+D**: Select next occurrence of selected text
- **Ctrl+Shift+K** / **Cmd+Shift+K**: Delete line

#### Navigation
- **Ctrl+G** / **Cmd+G**: Go to line
- **Ctrl+Home/End** / **Cmd+Home/End**: Go to beginning/end of file
- **Ctrl+F2** / **Cmd+F2**: Select all occurrences of current word
- **F12**: Go to definition
- **Alt+F12** / **Option+F12**: Peek definition
- **Ctrl+Tab** / **Cmd+Tab**: Navigate editor tabs

### Advanced Editing Features

#### Multi-Cursor Editing
- **Alt+Click** / **Option+Click**: Add cursor at clicked position
- **Ctrl+Alt+Up/Down** / **Cmd+Option+Up/Down**: Add cursor above/below
- **Ctrl+Shift+L** / **Cmd+Shift+L**: Select all occurrences of current selection

#### Code Folding
- **Ctrl+Shift+[** / **Cmd+Option+[**: Fold code block
- **Ctrl+Shift+]** / **Cmd+Option+]**: Unfold code block
- **Ctrl+K Ctrl+0** / **Cmd+K Cmd+0**: Fold all
- **Ctrl+K Ctrl+J** / **Cmd+K Cmd+J**: Unfold all

#### Split Editor
- **Ctrl+\\** / **Cmd+\\**: Split editor
- **Ctrl+1/2/3** / **Cmd+1/2/3**: Focus on editor group 1/2/3

### Workspace and Project Navigation

#### File Explorer
- Use breadcrumbs at the top of the editor for navigation
- Drag and drop to reorganize files
- Right-click for context menu with file operations

#### Search and Replace Across Files
- **Ctrl+Shift+F** / **Cmd+Shift+F**: Search across files
- **Ctrl+Shift+H** / **Cmd+Shift+H**: Replace across files

#### Integrated Terminal
- Multiple terminals can be created and managed
- Terminal can be split horizontally/vertically
- Use the dropdown to switch between different terminal types

### Personalization and Customization

#### Custom Keybindings
1. File → Preferences → Keyboard Shortcuts (or Ctrl+K Ctrl+S)
2. Search for commands and assign your preferred shortcuts
3. Use keybindings.json for advanced customizations

#### Snippets
1. File → Preferences → User Snippets
2. Create snippets for frequently used code patterns:
   ```json
   "HTML5 Boilerplate": {
     "prefix": "html5",
     "body": [
       "<!DOCTYPE html>",
       "<html lang=\"en\">",
       "<head>",
       "\t<meta charset=\"UTF-8\">",
       "\t<meta name=\"viewport\" content=\"width=device-width, initial-scale=1.0\">",
       "\t<title>${1:Document}</title>",
       "</head>",
       "<body>",
       "\t${2}",
       "</body>",
       "</html>"
     ],
     "description": "HTML5 boilerplate"
   }
   ```

#### Settings Sync
Use Settings Sync to keep your VS Code configuration consistent across different machines:
1. Click the Settings Sync icon in the Activity Bar
2. Sign in with GitHub or Microsoft account
3. Choose what to sync (settings, extensions, keybindings, etc.)

## Practical Exercises

1. **Editor Installation**: Install VS Code and configure basic settings like theme, font, and auto-save.

2. **Extension Exploration**: Install at least five extensions from the recommended list and explore their features.

3. **Keyboard Shortcut Practice**: Create a text file and practice using at least 10 different keyboard shortcuts for editing and navigation.

4. **Custom Snippet Creation**: Create a custom snippet for a code pattern you expect to use frequently in HTML, CSS, or JavaScript.

## Additional Resources

### Documentation
- [VS Code Documentation](https://code.visualstudio.com/docs)
- [VS Code Keyboard Shortcuts Reference](https://code.visualstudio.com/docs/getstarted/keybindings#_keyboard-shortcuts-reference)

### Videos and Tutorials
- [VS Code Introductory Videos](https://code.visualstudio.com/docs/getstarted/introvideos)
- [VS Code Can Do That?](https://www.vscodecandothat.com/) - Showcases lesser-known features

### Cheat Sheets
- [VS Code Keyboard Shortcuts Cheat Sheet](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-windows.pdf) (Windows)
- [VS Code Keyboard Shortcuts Cheat Sheet](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-macos.pdf) (macOS)

## Next Steps
After completing this module, you'll have a solid understanding of text editors and IDEs, particularly VS Code, which will be your primary tool for code development. The next module will introduce you to version control concepts, focusing on Git and GitHub.

## Assignment
Create a document that:
1. Shows screenshots of your customized VS Code setup, including theme and layout
2. Lists the extensions you installed with a brief explanation of why each is useful
3. Documents at least 15 keyboard shortcuts you've learned with descriptions
4. Includes a custom snippet you created for a common code pattern you expect to use