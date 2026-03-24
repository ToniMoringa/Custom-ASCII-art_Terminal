### **Is this safe?**
Yes. These steps do not install any software, change system registries, or affect your computer's performance. We are simply editing a "profile" script—a text file that the terminal reads to know how you want it to look. You can undo these changes at any time by deleting the lines we add.

Setup Instructions

Follow these steps to customize your default Windows terminal.

Open PowerShell.

Check for a profile:
Type test-path $profile. If it says False, create one by typing:
New-Item -path $profile -type file -force

Open the editor: Type notepad $profile.

Add your art: Copy your ASCII art and greeting message into the Notepad window.

Note: Wrap your text in a "Here-String" so PowerShell handles it correctly:

PowerShell
Write-Host @"
[Paste your ASCII art here]
Welcome back, YourName!(You can change this statement as you want you can add emojis too!🌸)
"@ -ForegroundColor Cyan
Save and Exit: Save the Notepad file and restart PowerShell.

2. WSL (Ubuntu)
3. This works for your Linux terminal within Windows.
4. Open Ubuntu/WSL.

Open the editor: We will use Nano, a simple terminal-based editor. Type:
nano ~/.bashrc

Navigate: Scroll to the very bottom of the file using your arrow keys.

Add your art: Type echo " then paste your art, and close it with another ".
Bash
echo "
[Paste your ASCII art here]
Domain Expansion: Welcome YourName!. (You can change this statement as you want you can add emojis too!🌸)
"
Save and Exit: * Press Ctrl + O (to Write Out/Save).

Press Enter to confirm.

Press Ctrl + X to exit the editor.

Tips for Custom ASCII Art

Scaling
ASCII art can "break" or wrap around if it is wider than your terminal window. (Replace with any custom one you make or find online )
Use Notepad first: Paste your art into Notepad and resize the window to see where the lines break.
Shrink it: If the art looks messy, try a smaller version or reduce the font size in your Terminal Settings.

Edit Menu (Nano)
In Ubuntu Terminal using Nano, At the bottom of the screen is a menu as so;
Command                     Action
^G Get Help               View instructions
^O Write Out              Save your changes
^W Where Is               Search for text
^X Exit                   Close the editor


The ^ symbol represents the Ctrl key on your keyboard.

Going back to Default?

To return terminal as it was:
Re-open the files (notepad $profile for Windows or nano ~/.bashrc for Ubuntu).

Delete the lines you added.

Save and exit.

![Terminal Preview](assets/HigurumaTerminal.png)<img src="terminal-preview.png" alt="Terminal Preview" width="500">
![Terminal Preview](assets/GojoVscodewithBeSunflowerTheme.png)