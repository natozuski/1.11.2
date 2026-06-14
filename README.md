# How to play Minecraft

## You need:
- MultiMC
- Java 1.8.0
- Worldedit.jar (mod, for minecraft 1.11.2)
- a minecraft account (you have one alr)

## Steps:
- sign in to minecraft account on multimc
- create a world in minecraft 1.11.2
- install forge in for particular world u created (go to mod settings for particular version, download appropriate forge version for 1.11.2)
- make sure dat worldedit.jar file is in .minecraft/mods

## Tools:
- On a particular world select export instance to export it
- If you select 'Folders -> View Instance folder' you can see the .minecraft files for that instance

## (Git)
- All files gotta be less than 100mb otherwise they gon get rejected

# Working with the repo

### Windows

- download git https://git-scm.com/download/win
- go to cmd and type git --version to see if it worked
- you should see git version 2.xx
- on each computer set up git
- git config --global user.name "Your Name"
- git config --global user.email "you@example.com"
- check it
- git config --global --list
- create the shortcut command for git fresh
- git config --global alias.fresh "!git fetch origin && git reset --hard origin/main && git clean -fd"
- check it with git config --global --list
- always do the cycle of:
- git fresh
- git add
- git push
- clone the repo using https since we'ain got ssh keys set up
- git clone https://github.com/natozuski/multimc-1.9.git (or whatever its called now)

### Mac

- open terminal from finger (command + space)
- just type git and download it if its not there
- type git --version to check
- you should see git version 2.xx
- on each computer set up git
- git config --global user.name "Your Name"
- git config --global user.email "you@example.com"
- check it
- git config --global --list
- create the shortcut command for git fresh
- git config --global alias.fresh '!f(){ git fetch origin && git reset --hard origin/$(git rev-parse --abbrev-ref HEAD) && git clean -fd; }; f'
- ts different from windows btw
- check it with git config --global --list
- always do the cycle of:
- git fresh
- git add
- git push
- clone the repo using https since we'ain got ssh keys set up
- git clone https://github.com/natozuski/multimc-1.9.git (or whatever its called now)
