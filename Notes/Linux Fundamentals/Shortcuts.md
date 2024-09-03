---
tags:
  - HTB
  - Notes
  - Linux
  - Reference
---
___
There are many shortcuts that we can use to make working with Linux easier and faster. After we have familiarized ourselves with the most important of them and have made them a habit, we will save ourselves much typing. Some of them will even help us to avoid using our mouse in the terminal.
### Auto-Complete
- [x] `[TAB]` - Initiates auto-complete. This will suggest to us different options based on the `STDIN` we provide. These can be specific suggestions like directories in our current working environment, commands starting with the same number of characters we already typed, or options.
### Cursor Movement
- [x] `[CTRL] + A` - Move the cursor to the `beginning` of the current line.
- [x] `[CTRL] + E` - Move the cursor to the `end` of the current line.
- [x] `[CTRL] + [←]` / `[→]` - Jump at the beginning of the current/previous word.
- [x] `[ALT] + B` / `F` - Jump backward/forward one word.
### Erase The Current Line
- [x] `[CTRL] + U` - Erase everything from the current position of the cursor to the `beginning` of the line.
- [x] `[Ctrl] + K` - Erase everything from the current position of the cursor to the `end` of the line.
- [x] `[Ctrl] + W` - Erase the word preceding the cursor position.
### Paste Erased Contents
- [x] `[Ctrl] + Y` - Pastes the erased text or word.
### Ends Task
- [x] `[CTRL] + C` - Ends the current task/process by sending the `SIGINT` signal. For example, this can be a scan that is running by a tool. If we are watching the scan, we can stop it / kill this process by using this shortcut. While not configured and developed by the tool we are using. The process will be killed without asking us for confirmation.
### End-of-File (EOF)
- [x] `[CTRL] + D` - Close `STDIN` pipe that is also known as End-of-File (EOF) or End-of-Transmission.
### Clear Terminal
- [x] `[CTRL] + L` - Clears the terminal. An alternative to this shortcut is the `clear` command you can type to clear our terminal.
### Background a Process
- [x] `[CTRL] + Z` - Suspend the current process by sending the `SIGTSTP` signal.
### Search Through Command History
- [x] `[CTRL] + R` - Search through command history for commands we typed previously that match our search patterns.
- [x] `[↑]` / `[↓]` - Go to the previous/next command in the command history.
### Switch Between Applications
- [x] `[ALT] + [TAB]` - Switch between opened applications.
### Zoom
- [x] `[CTRL] + [+]` - Zoom in.
- [x] `[CTRL] + [-]` - Zoom out.
___