# 🎨 Customize Your Oh My Posh Prompt (Windows)

This repository explains how to install and customize **Oh My Posh** on a **Windows** system. It includes a personal styling file that you can use or modify to your own taste.

## 🧰 What is Oh My Posh?

[Oh My Posh](https://ohmyposh.dev/) is a prompt theme engine for your terminal. It lets you transform your terminal with beautiful and informative prompts.

## 🔽 How to Install Oh My Posh (Windows)

1. Open PowerShell as Administrator.
2. Install via the official instructions or directly with the following command:

```powershell
winget install JanDeDobbeleer.OhMyPosh -s winget
```
3. You can also visit the official site for more options and documentation:
   👉 https://ohmyposh.dev


# 🛠 How to Apply a Custom Theme (Using $PROFILE)

To load your custom styling on startup, you need to edit your PowerShell profile file.

##Step-by-step:

1. Check if your $PROFILE file exists:

```powershell
Test-Path $PROFILE
```

2. If it doesn't exist, create it:

```powershell
New-Item -Path $PROFILE -ItemType File -Force
```

3. If it doesn't exist, create it:

```powershell
notepad $PROFILE
```

4. Add the following line to load your custom theme (adjust the path to where you cloned this repo):

```powershell
oh-my-posh init pwsh --config "C:\path\to\your\theme.omp.json" | Invoke-Expression
```

5. Save the file and restart your terminal.


# 🧪 Example Theme

Inside this repo, you'll find a custom .json theme file you can try out right away or tweak to your liking.

Feel free to fork this project or suggest improvements. Enjoy your personalized terminal!
