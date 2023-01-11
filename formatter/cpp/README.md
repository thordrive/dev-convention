# ClangFormat

Creating separate `.clang-format` files for each project is not recommended. Instead, we recommend that you keep your `.clang-format` up-to-date in a parent directory common to all your workspaces. For example, let's say you have two projects at `/ws/project-a` and `/ws/project-b`. It is recommended to place `.clang-format` at `/ws/.clang-format`.

# Integration

## VSCode

Extension [C/C++ [ms-vscode.cpptools]](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools) published by Microsoft provides built-in **clang-format**.

### Install on the Web Page

1. Open [C/C++ [ms-vscode.cpptools]](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools) page on VSCode Marcketplace.
2. Click *install* button on the page.

### Install on the VSCode

1. Bring up the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of VS Code or the View: Extensions command (`Ctrl`+`Shift`+`X`).
2. Search `ms-vscode.cpptools`.
3. Click the search result titled `C/C++`.
4. Click *install* button on the page.

### Format Code

Default shortcut:
- Windows: `Alt`+`Shift`+`F`
- Mac: `Option`+`Shift`+`F`
- Linux: `Ctrl`+`Shift`+`I`

Alternatively, you can run the command on the **Command Palette**
1. Open **Command Pallette** (`Ctrl`+`Shift`+`P`).
2. Enter *Format Document*.

You can format the code whenever you save the file.

1. Open `settings.json` (`ctrl`+`,`).
2. Click **User** tab.
2. Search *edit.formatOnSave*.
3. Check the box on the left of *Editor: Format On Save*.