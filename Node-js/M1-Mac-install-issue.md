# M1 Mac Por Install Issue - solution sheet

Command + Shift+ .  (Which can check the hide file)

1. https://brew.idayer.com/guide/m1/

   Homebrew install

2. https://www.youtube.com/watch?v=AEuI0PBvgfM

3. This link will teach you how to install the nodejs.

```shell
local brew_path="/opt/homebrew/bin"
local brew_opt_path="/opt/homebrew/opt"
local nvm_path="$HOME/.nvm"

export PATH="${brew_path}:${PATH}"
export NVM_DIR="${nvm_path}"

[ -s "${brew_opt_path}/nvm/nvm.sh" ] && . "${brew_opt_path}/nvm/nvm.sh"  # This loads nvm
[ -s "${brew_opt_path}/nvm/etc/bash_completion.d/nvm" ] && . "${brew_opt_path}/nvm/etc/bash_completion.d/nvm"  # This loads nvm bash_completion
```



```shell
nvm use 16 # switch node 16 version
```

3. https://github.com/Automattic/node-canvas/issues/1733

   ```bash
   # Ok, I somehow got it to work but I really don't know what I changed... I assume you ran 
   brew install pkg-config cairo pango libpng jpeg giflib librsvg 
   # at some point? The only thing I remember doing was running brew doctor once, then 
   npm uninstall canvas # if canvas has an error.
   # Then 
   npm i canvas --save
   ```

   

