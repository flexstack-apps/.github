<img src="https://flexstack.com/favicon.svg" width=64/>

## FlexStack 1-Click Apps

Build and deploy serverless apps on AWS with unrivaled ease.<br/>
FlexStack is a cloud native alternative to platforms like Render, Vercel, and Heroku.

### Philosophy

- Use high quality tooling, not too much, mostly Rust-based
- Obey the [12-factor methodology](https://12factor.net/)
- If it runs on my computer, it runs on your computer
- If you understand one developer environment, you understand all environments

### Prerequisites

Our curated apps use [mise](https://mise.jdx.dev/about.html) to run tasks, manage tool versions, 
and manage environment variables.

1. [Install mise](https://mise.jdx.dev/getting-started.html)

```sh
curl https://mise.run | sh
```

2. Add mise to your shell profile. This activates mise in your shell, ensuring the correct tool versions are used for your environment.

```sh
# Zsh
echo 'eval "$(~/.local/bin/mise activate zsh)"' >> ~/.zshrc
echo 'eval "$(~/.local/bin/mise activate zsh --shims)"' >> ~/.zprofile
source ~/.zshrc

# Bash 
echo 'eval "$(~/.local/bin/mise activate bash)"' >> ~/.bashrc
echo 'eval "$(~/.local/bin/mise activate bash --shims)"' >> ~/.bash_profile
source ~/.bashrc

# Fish
echo '~/.local/bin/mise activate fish | source' >> ~/.config/fish/config.fish
fish_add_path ~/.local/share/
```
