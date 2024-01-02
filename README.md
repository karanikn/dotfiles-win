***karanik "Windows Dotfiles***

**Starship DotFile - starship.toml**

[Guide](https://starship.rs/guide/#%F0%9F%9A%80-installation)

Prerequisites [https://chrisant996.github.io/clink/clink.html]

Install Starship using winget

Open CMD and run
>winget install --id Starship.Starship

>winget install clink


**CMD**

Create a file at this path %LocalAppData%\clink\starship.lua with the following contents:
>load(io.popen('starship init cmd'):read("*a"))()

Add starship configuration
Or for Cmd (Windows) would be adding this line to your starship.lua:
>os.setenv('STARSHIP_CONFIG', 'C:\\Users\\user\\example\\non\\default\\path\\starship.toml')

**PowerShell**
Add the following to the end of your PowerShell configuration (find it by running $PROFILE):
>Invoke-Expression (&starship init powershell)

Add starship configuration
Equivalently in PowerShell (Windows) would be adding this line to your $PROFILE:
>$ENV:STARSHIP_CONFIG = "$HOME\example\non\default\path\starship.toml"



**CMD result**

![image](https://github.com/karanikn/dotfiles-win/assets/1959460/ca8ab829-95e6-4b56-82d6-0b143ae660f3)
