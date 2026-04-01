1. we need the JetBrains Mono Nerd Fonts before we jump on customization
2. Go to https://github.com/SleepyCatHey/Ultimate-Win11-Setup -> Terminal -> setting.json -> copy all the code
3. at the terminal windows, click on the drop down button and navigate to settings
4. Open JSON file at bottom left
5. Once we in the config JSON file, we now select all the config and replace it with the config we get from the setting.json that we did copy earlier
6. Then save it Ctrl + S then we Save the settings.

*if we get the error message "Can't find JetBrains Mono Nerd font. Please install it or change it." we can issue it like this:
i. At Desktop, right click -> Personalize -> Fonts
ii. At "Available fonts" we search for JetBrains then it will show up the font name
iii. Go back to the JSON file config, Ctrl + H to find then we type JetBrain to navigate to the Font-family
iv. We now change the whole name to match the name that we already found at step ii*

7. Then when you open the new Terminal, you will see different from the first Terminal that we use to know
8. Type in "$PROFILE" it will show us a path file like this: D:\%USER_NAME\Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1
9. Open File Explorer and navigate to that path, at first we won't see the folder WindowsPowerShell because we haven't created a profile manually yet
10. Go back to Terminal and issue the command: New-Item -Path $profile.CurrentUserAllHosts -Type File -Force Then Boommm! now we got the profile created, go back to the file path, we now should see the .ps1 file
11. Now we will work on fastfetch (is a lightweight command-line tool that shows your system info in a clean, fast way.), open this link: https://github.com/fastfetch-cli/fastfetch
12. Scroll down to the Installation section and find winget install fastfetch (located at window section), copy that command line and paste it in your Terminal, this step you will install fastfetch in your computer
13. Once it download successfully, go back to https://github.com/SleepyCatHey/Ultimate-Win11-Setup -> FastFetch folder -> download all the file in it (ascii.txt and config.json)
14. Now open File Explorer -> This PC -> Users -> $YOUR_USER_NAME -> create a folder name ".config" -> right click to that folder -> properties -> at General pane, Check the "Hidden" Box -> apply -> OK

*To see the hidden file, at File Explorer action bar on the top, click View -> Show -> Hidden Items*

15. Inside .config folder, create another folder name fastfetch
16. Now we move all the file that we've downloaded at step 13 and put it in fastfetch folder
17. Open config.jsonc File, at source change the default path to the path that you create the fastfetch folder at step 15 and save it
18. Now go back to the website https://github.com/SleepyCatHey/Ultimate-Win11-Setup -> PowerShell -> open the file and copy all
19. Open your .ps1 file (D:\%USER_NAME\Documents\WindowsPowerShell\Microsoft.PowerShell_profile.ps1) and paste all the codes that we copied in step 18, remember replacing the %USERPROFILE% to your username -> save