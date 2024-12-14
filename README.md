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
1. Clone this repository:
    ```sh
    git clone https://github.com/shadielfares/tmux-config.git ~/.tmux-config
    ```
2. Symlink the Tmux configuration file to your home directory:
    ```sh
    ln -s ~/.tmux-config/.tmux.conf ~/.tmux.conf
    ```
3. Reload the Tmux configuration:
    ```sh
    tmux source-file ~/.tmux.conf
    ```

## Usage 🚀
- **Pane Management**: Easily split windows into multiple panes for a more organized workflow.
- **Custom Key Bindings**: Utilize custom shortcuts to quickly navigate and manage panes.
- **Manual Plugin Installation**: Use `<Prefix> + I` while in Tmux to manually install plugins.

## Contributing 🤝
Contributions are welcome! Please fork this repository and open a pull request with your improvements.

Enjoy an enhanced Tmux experience!
