# dotfiles

This repository contains configuration for Zsh and related tooling for a powerful terminal environment.

## Getting Started

Follow these steps to set up your terminal with Oh My Zsh, a Nerd Font, [Starship prompt](https://starship.rs/), and essential plugins for productivity and visual enhancements.

### 1. Install [Oh My Zsh](https://ohmyz.sh/)

```sh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### 2. Install a [Nerd Font](https://www.nerdfonts.com/)

Nerd Fonts add extra icons and glyphs for enhanced prompts and plugins.

- Visit [Nerd Fonts Downloads](https://www.nerdfonts.com/font-downloads)
- Download and install a patched font (e.g., FiraCode Nerd Font)
- Set your terminal to use the Nerd Font

### 3. Install [Starship Prompt](https://starship.rs/)

Starship is a fast, customizable, minimal prompt.

```sh
curl -sS https://starship.rs/install.sh | sh
```

Then, add to your `.zshrc` (if not already):

```sh
eval "$(starship init zsh)"
```

### 4. Recommended Zsh Plugins

Install these plugins for enhanced autocompletion, syntax highlighting, command suggestions, and more:

#### a. [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)

```sh
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

#### b. [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

```sh
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

#### c. [you-should-use](https://github.com/MichaelAquilina/zsh-you-should-use)

```sh
git clone https://github.com/MichaelAquilina/zsh-you-should-use.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/you-should-use
```

#### d. [zsh-bat](https://github.com/fdellwing/zsh-bat)

```sh
git clone https://github.com/fdellwing/zsh-bat.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-bat
```

### 5. Enable Plugins in `.zshrc`

Open your `.zshrc` and edit the `plugins=` line, for example:

```sh
plugins=(
  git
  zsh-autosuggestions
  zsh-syntax-highlighting
  you-should-use
  zsh-bat
)
```

### 6. Theme

This setup uses the [`robbyrussell`](https://github.com/ohmyzsh/ohmyzsh/wiki/Themes#robbyrussell) Oh My Zsh theme by default, plus the Starship prompt for modern, informative, and customizable appearances. You can further adjust the prompt and theme via `.zshrc` and [Starship config](https://starship.rs/config/).

---

Enjoy a beautiful, productive shell!
