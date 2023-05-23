# Version

```shell
NVIM v0.9.0
Build type: Release
LuaJIT 2.1.0-beta3
```
# Icon and Fonts

I use iterm as my terminal, you can use a nerd font for your termimal.In this title, i recommand [JetBrain Mono Nerd font](https://www.nerdfonts.com/#downloads).Take mine iterm as a example, open **settings > profiles >text > Fonts**.Check Anti-aliased block to make you characters look more smooth. 

# Theme
Since for lazyvim use a amazing theme names [tokyonight](https://github.com/enkia/tokyo-night-vscode-theme), so i want to sync all my themes to tokyonight.As for iterm you can go to the [ iterm color scheme ](https://iterm2colorschemes.com/) to install it.When you dowload the code of color scheme.You should name the file like this: **tokyonight-storm.itermcolors**
+ iterm: settings > profiles > default > colors > color preset
+ idea: plugins store
+ vscode: plugins

# Keymaps

You can type tree to see the file structure, my tree is below:
```shell
.
├── README.md
├── init.lua
├── lazy-lock.json
├── lua
│   ├── config
│   │   ├── autocmds.lua
│   │   ├── keymaps.lua
│   │   ├── lazy.lua
│   │   └── options.lua
│   └── plugins
│       └── example.lua
└── stylua.toml

4 directories, 9 files
```

All the changes of my personal config is below: **~/.config/lua/keymaps.lua**

|Key             |Description                              |Model |
|----------------|-----------------------------------------|----- |
|jj              |quit insert model                        |i     |
|J               |move lines down                          |v     |
|K               |move lines up                            |v     |
|L               |move cursor to line start                |v,n   |
|H               |move cursor to line end                  |v,n   |
|\<Shift-tab\>   |jump to previous buffer                  |n     |
|tab             |jump to next buffer                      |n     |

And some keymaps not be metioned in [lazyvim.org](https://www.lazyvim.org/keymaps)
|Key             |Description                              |Model |
|----------------|-----------------------------------------|----- |
|\<Ctrl-d\>      |close the hover terminal                 |n     |

# Trouble shooting

If you open lazyvim and find treesitter download parsers error,pls download the parsers manually with TSInstall /<language/>.You can **cd ~/.config/nvim/plugins/nvim-treesitter.lua** to see the propertity **ensure_installed** that you specify to install.
