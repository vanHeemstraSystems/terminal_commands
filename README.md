terminal_commands
# Terminal Commands

## Make the "cls" command in a Windows terminal act when using the "clear" command of Linux

- [Tired of typing ‘cls’ into a *nix terminal or ‘clear’ in CMD?](https://community.spiceworks.com/t/tired-of-typing-cls-into-a-nix-terminal-or-clear-in-cmd/1006566)

Add ```cls``` and ```clear``` custom commands to both Windows and Linux so you don’t punch a hole in the monitor when you keep typing the wrong one.

### Step 1: Windows

![9ac91cc888102808c41bc50cf5c1a2c7032965e2](https://github.com/user-attachments/assets/31b0bda3-af9d-4fd8-ac19-5b25c903ebb8)

This is the simpler one of the two.

Text editor: (notepad)<br/>
Just open notepad, type in ```cls``` and save it as “C:\Windows\Clear.bat”. Now every time you’re in CMD and type ```clear```, you will clear your screen just like ```cls```.

Command Prompt:<br/>
Elevate yourself as admin and run ```echo cls > C:\Windows\Clear.bat```.

### Step 2: Linux

![2896815acc52642c91b15e780a3aed955db649c0](https://github.com/user-attachments/assets/0ec6c837-3e94-49ee-b5cc-2b67f70300a1)

A little more time consuming, but simple none the less. After this, typing ```cls``` will clear your prompt.

Terminal:<br/>
Elevate yourself to root and run ```echo clear > /usr/bin/cls; chmod 777 /usr/bin/cls```

Just something small that keeps your from pulling out your hair.
