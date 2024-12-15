# Tmux Config 🎛️

Welcome to my Tmux configuration repository! This setup is designed to enhance the functionality of Tmux, particularly in conjunction with Neovim, by allowing for additional panes and improved workflow integration.

## Features ✨
- Custom Tmux configuration tailored for Neovim users
- Efficient pane management
- Enhanced productivity with streamlined shortcuts

## Prerequisites 📋
- Ensure you have Tmux installed on your system. You can install it using your package manager, for example:
    ```sh
    sudo apt-get install tmux
    ```

## Installation 🛠️

1. Install Tmux Package Manager (TPM):
    ```
    git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
    ```
2. Clone this repository:
    ```sh
    git clone https://github.com/shadielfares/tmux-config.git ~/.config/tmux/tmux.conf
    ```
3. Reload the Tmux configuration:
    ```sh
    tmux source ~/.config/tmux/tmux.conf
    ```
4. Download the newly added packages, using the command:
    ```
    CTRL+B, SHIFT+i
    ```

## Usage 🚀
- **Pane Management**: Easily split windows into multiple panes for a more organized workflow.
- **Custom Key Bindings**: Utilize custom shortcuts to quickly navigate and manage panes.
- **Manual Plugin Installation**: Use `<Prefix> + I` while in Tmux to manually install plugins.

## Contributing 🤝
Contributions are welcome! Please fork this repository and open a pull request with your improvements.

Enjoy an enhanced Tmux experience!
