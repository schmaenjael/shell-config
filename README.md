# LinuxConfiguration

## Installation

To use these configurations you are required to have the Friendly-Interactive Shell (FISH) and Starship (Cross-Shell Prompt)installed.

Install Fish using:

```sh
sudo apt-get install fish
```

And install starship using 

```sh
curl -fsSL https://starship.rs/install.sh | bash
```

If not existing, create directory ~./config/fish
```sh
mkdir ~./config/fish
```

Navigate to ~./config/fish and create the file config.fish using:

```sh
cd ~./config/fish && touch config.fish
```

Copy paste the content of my configuration into the newly created file.
You may have to change the Path to the Starship installation.
e.g. it could be "/usr/local/bin/starship" instead of "/usr/bin/starship".

Check your starship installation directory with the ``which`` command and replace the path to the starship prompt in your configuration (~./config/fish/config.fish - Section "Starship prompt")

```sh
which starship
```

Now create the file starship.toml in ~/.config/ and copy-paste the content of my starship.toml into it.

------------

OPTIONAL:

If you want to use ``neofetch`` as well, install it using:

```sh
sudo apt-get install neofetch
`````

------------

Save it and now enter ``fish`` to start the shell.

To set the fish shell to default, enter the first command, copy paste the fish directory and execute the second command with your fish location.

`````sh
which fish

chsh -s [YOUR_FISH_LOCATION] 
`````

Please mind that:
Inspiration was taken from Garuda Linux's Fish Configuration. (I added some functions and Aliases and removed some stuff I deemed unnecessary).
