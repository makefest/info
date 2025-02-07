# Setting up Keepass

# Keepass password

- 🔨 get a sheet of paper and a pen
- ✏️ write `KeePass Password` at the top of the sheet
- 🦉 here are some hints on what makes a good password:

> [!IMPORTANT]
> - at least 8 characters long containing at least 1 of each of the following:
> - uppercase letters
> - lowercase letters
> - numbers
> - special characters like !%+;,- 

- ✏️ write down a **good** password on your password paper
- 🔨 copy the password on another piece of paper, identify a person you trust, for example a parent, give the piece of paper to that person and ask him or her to keep it in a safe place

## Hiding the password paper

- 🦉 we need a place to hide the password paper - here are some hints:

> [!IMPORTANT]
> - it's not openly visible to everyone
> - the dog can't get to it
> - water can't get to it
> - it can't be mistaken for garbage

- 🔨 identify a good place for hiding the password paper **securely** 
- 🔨 when done using the paper, put it back into its hiding place

## Install KeePassXC

- 🔨 install [KeePassXC](https://keepassxc.org/)
- 🔨 try starting keepass
- 🔨 if keepass starts, close it again
- 🔨 if keepassxc does not start, install Microsoft Visual C++ Redistributable, see [here](https://keepassxc.org/blog/2022-03-21-2.7.0-released/) and try again

## Create KeePassXC shortcut for screen capturing

- 🦉 In the interest of privacy and security, if you start `KeePassXC`, the program won't be visible when screen sharing and you can't make screenshots of it. See [docs](https://keepassxc.org/docs/KeePassXC_UserGuide.html#_screenshot_security) for details.
- 🦉 Below we will create an extra program shortcut to have the option to start KeePassXC with screen capturing enabled
- 🔨 press `Start` and type `keepass` but don't press Enter
- 🔨 right-click on the keepass app and select `Open file location`
- 🦉 that opens File Explorer and shows you the folder where the Windows shortcut to the KeePass program is located
- 🔨 select the keepass shortcut and press `Ctrl` + `C` to copy and then `Ctrl` + `V` to paste a copy of the shortcut
- 🔨 rename the copy to:

```markdown
KeePassXC - ScreenCapture
```

- 🔨 right-click `KeePassXC - ScreenCapture` and select Properties
- 🔨 on the tab `Shortcut`, in the field `Target`, at the very end after the quotation marks, add a single space and then the following:
```markdown
--allow-screencapture
```

- 🔨 click on Ok to close the window
- 🔨 press `Start` again and type keepass
- 👁️ besides the previous `KeePassXC` you should now also have `KeePassXC - ScreenCapture` as a second hit, perhaps under Apps
- 🔨 start `KeePassXC - ScreenCapture`
- 👁️ you will now be able to screen share the program and make screenshots of it

## Create keepass database

- 🔨 make sure you have a folder called `Credentials` in your `Documents` folder
- 🔨 open `KeePassXC - ScreenCapture`
- 🔨 if you don't have a database yet, create one in your `Credentials` folder, using the password you've noted before and accepting the default settings KeePass is proposing
