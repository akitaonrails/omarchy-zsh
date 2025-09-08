## Omarchy ZSH configs

[Omarchy 2.0](https://omarchy.org/) comes default with Bash. But I prefer ZSH (personal preference, Bash is perfectly fine). So I decided to make my own overrides for ZSH.

### Install

```Bash
yay -S zsh zoxide
chsh -s $(which zsh)
git clone https://github.com/akitaonrails/omarchy-zsh.git ~/.config/zsh
ln -s ~/.config/zsh/.zshrc ~/.zshrc 
```

### New Features

* support for [Atuin](https://atuin.sh/) for history cloud syncing (you can keep all your history across installations).

* replaced the old PS1 prompt for [Starship Presets](https://starship.rs/presets/pure-preset), in particular defaults to Pure Prompt, but you can change it later. Check the link for other presets.

* source from `~/.config/zsh/secrets` where you can keep your OpenAI Keys and other secrets Envs. Make sure to `chmod 600 secrets` to make it extra safe.
