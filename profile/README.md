<h2><img src="https://flexstack.com/favicon.svg" height=20 alt=""/> FlexStack Apps</h2>

Build and deploy serverless apps on AWS in 1-click.<br/>
[FlexStack](https://flexstack.com) is a cloud native alternative to platforms like Render, Vercel, and Heroku.

### Philosophy

- Use high quality tooling, not too much, mostly Rust-based
- Obey the [12-factor methodology](https://12factor.net/)
- If it runs on my computer, it runs on your computer
- If it runs today, it runs tomorrow
- If you understand one development environment, you understand all environments

### Deploy on FlexStack

Click the "Deploy on FlexStack" button in any app repository to:

- Clone the repo to your a linked GitHub account
- Deploy the app to your own AWS account

<a href="https://flexstack.com/deploy"><img src="https://flexstack.com/deploy-on-flexstack.svg" height=40/></a>

Alternatively, you can clone any of the repos here and deploy later by linking them to a FlexStack project.

### Before you clone

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
