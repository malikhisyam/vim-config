# VSCode + Vim Keybindings Cheatsheet

<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/9/9f/Vimlogo.svg" alt="Vim Logo" width="100" height="100">
</p>

This cheatsheet covers essential Vim navigation, editing, and custom keybindings in VSCode to help streamline your development workflow.

## Setup Instructions

### Step 1: Install Vim Extension in VSCode
1. Open VSCode.
2. Go to the Extensions sidebar (`Ctrl+Shift+X`).
3. Search for **Vim** and install the extension by **VSCodeVim**.

### Step 2: Configure Settings in settings.json and keybindings.json
1. Open the VSCode settings by pressing `Ctrl + ,`.
2. In the top-right corner, select **Open Settings (JSON)** to edit the `settings.json` file directly.
3. Copy and paste the settings.json into your `settings.json`
4. In the bottom-right corner press gear icon and click **Keyboard Shortcut**
5. Then look at the top-right corner, again click **Open Keyboard Settings (JSON)** to edit the `keybindings.json`
6. Copy and paste the keybindings.json to your keybindings.json`

## Table of Contents
1. [Basic Navigation](#basic-navigation)
2. [Word Navigation](#word-navigation)
3. [Line Navigation](#line-navigation)
4. [Searching](#searching)
5. [Editing](#editing)
6. [Visual Mode](#visual-mode)
7. [Command-line Mode](#command-line-mode)
8. [Split Windows and Tabs](#split-windows-and-tabs)
9. [Leader Key Configurations](#leader-key-configurations)
10. [VSCode Keybindings](#vscode-keybindings)

---

### Basic Navigation
| Key       | Command                   | Description                 |
|-----------|---------------------------|-----------------------------|
| `h`       | Move cursor left          | Basic left movement         |
| `j`       | Move cursor down          | Basic down movement         |
| `k`       | Move cursor up            | Basic up movement           |
| `l`       | Move cursor right         | Basic right movement        |
| `i`       | Insert mode               | Enter insert mode           |
| `<ESC>`   | Normal mode               | Exit insert mode            |

### Word Navigation
| Key       | Command                   | Description                   |
|-----------|---------------------------|-------------------------------|
| `w`       | Move to start of next word| Jump to next word             |
| `b`       | Move to start of prev word| Jump to previous word         |
| `e`       | Move to end of next word  | Move to next word end         |
| `ge`      | Move to end of prev word  | Move to previous word end     |

### Line Navigation
| Key       | Command                   | Description                     |
|-----------|---------------------------|---------------------------------|
| `0`       | Start of line             | Jump to beginning of line       |
| `^`       | Start of non-blank line   | Jump to first non-blank character|
| `$`       | End of line               | Jump to end of line             |

### Searching
| Key       | Command                       | Description                     |
|-----------|-------------------------------|---------------------------------|
| `/`       | Search forwards               | Search for a pattern forwards   |
| `?`       | Search backwards              | Search for a pattern backwards  |
| `n`       | Next search match             | Go to the next match            |
| `N`       | Previous search match         | Go to the previous match        |

### Editing
| Key             | Command                     | Description                         |
|-----------------|-----------------------------|-------------------------------------|
| `d{motion}`     | Delete                      | Delete text covered by motion       |
| `y{motion}`     | Yank                        | Copy text covered by motion         |
| `p`             | Paste                       | Paste text after the cursor         |
| `u`             | Undo                        | Undo last change                    |
| `<C-R>`         | Redo                        | Redo last undo                      |

### Visual Mode
| Key             | Command                     | Description                         |
|-----------------|-----------------------------|-------------------------------------|
| `v`             | Character-wise visual mode  | Enter character-wise visual mode    |
| `V`             | Line-wise visual mode       | Enter line-wise visual mode         |
| `<C-V>`         | Block-wise visual mode      | Enter block-wise visual mode        |

### Command-line Mode
| Command                     | Description                             |
|-----------------------------|-----------------------------------------|
| `:w`                        | Save file                               |
| `:q`                        | Quit file                               |
| `:wq`                       | Save and quit file                      |
| `:sp {file}`                | Open horizontal split with file         |
| `:vsp {file}`               | Open vertical split with file           |

### Split Windows and Tabs
| Key                | Command                                   | Description                  |
|--------------------|-------------------------------------------|------------------------------|
| `:sp {file}`       | Open horizontal split                     |                              |
| `:vsp {file}`      | Open vertical split                       |                              |
| `<C-W> h`          | Move to split to the left                 |                              |
| `<C-W> j`          | Move to split below                       |                              |
| `<C-W> k`          | Move to split above                       |                              |
| `<C-W> l`          | Move to split to the right                |                              |
| `:tabnew {file}`   | Open file in new tab                      |                              |

### Vim Leader Key Configurations

| Key Combination        | Command                                      | Description                       |
|------------------------|----------------------------------------------|-----------------------------------|
| `<leader> + v`         | `:vsplit`                                    | Open vertical split               |
| `<leader> + s`         | `:split`                                     | Open horizontal split             |
| `<leader> + h`         | `workbench.action.focusLeftGroup`            | Focus pane to the left            |
| `<leader> + j`         | `workbench.action.focusBelowGroup`           | Focus pane below                  |
| `<leader> + k`         | `workbench.action.focusAboveGroup`           | Focus pane above                  |
| `<leader> + l`         | `workbench.action.focusRightGroup`           | Focus pane to the right           |
| `<leader> + w`         | `:w!`                                        | Save file                         |
| `<leader> + q`         | `:q!`                                        | Close file without saving         |
| `<leader> + x`         | `:x!`                                        | Save and close                    |
| `[ + d`                | `editor.action.marker.prev`                  | Jump to previous marker           |
| `] + d`                | `editor.action.marker.next`                  | Jump to next marker               |
| `<leader> + c + a`     | `editor.action.quickFix`                     | Open quick fix for current line   |
| `<leader> + f`         | `workbench.action.quickOpen`                 | Open file quick-open menu         |
| `<leader> + p`         | `editor.action.formatDocument`               | Format the current document       |
| `g + h`                | `editor.action.showDefinitionPreviewHover`   | Preview definition under cursor   |

### VSCode Keybindings
| Key Combination    | Command                                    | Description                           |
|--------------------|--------------------------------------------|---------------------------------------|
| `ctrl+shift+a`     | `workbench.action.terminal.focusNext`      | Focus next terminal                   |
| `ctrl+shift+b`     | `workbench.action.terminal.focusPrevious`  | Focus previous terminal               |
| `ctrl+shift+j`     | `workbench.action.togglePanel`             | Toggle panel visibility               |
| `ctrl+shift+n`     | `workbench.action.terminal.new`            | Open new terminal                     |
| `ctrl+shift+w`     | `workbench.action.terminal.kill`           | Kill current terminal                 |
| `ctrl+e`           | `workbench.action.toggleSidebarVisibility` | Toggle sidebar visibility             |
| `ctrl+e` (in editor) | `workbench.files.action.focusFilesExplorer` | Focus file explorer                 |
| `n`                | `explorer.newFile`                         | Create new file in file explorer      |
| `r`                | `renameFile`                               | Rename selected file                  |
| `shift+n`          | `explorer.newFolder`                       | Create new folder in file explorer    |
| `d`                | `deleteFile`                               | Delete selected file                  |

---

This cheat sheet consolidates the most useful Vim commands, VSCode keybindings, and custom configurations to optimize your development experience!
