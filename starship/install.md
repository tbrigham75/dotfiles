1.  Download a nerd font:  https://www.nerdfonts.com/
    Like: Hack Nerd Font or JetBrainsMono

2. Install:
    Windows:  choco install starship -y
    Linux:  curl -sS https://starship.rs/install.sh | sh

3.  Create this file and folder in home folder for Linux and Windows (Can copy starship.toml from this repo):
    .starship\starship.toml

4.  PowerShell put this in $profile:
    code $profile

    Put this in file:
        $ENV:STARSHIP_CONFIG = "$HOME\.starship\starship.toml"
        Invoke-Expression (&starship init powershell)

5.  Put this in ~/.bashrc
        export STARSHIP_CONFIG=~/.starship/starship.toml
        eval "$(starship init bash)"