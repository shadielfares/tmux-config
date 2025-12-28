# Tmux Config 

Welcome to my Tmux configuration repository! This setup is designed to enhance the functionality of Tmux, particularly in conjunction with Neovim, by allowing for additional panes and improved workflow integration.

## Features 
- Custom Tmux configuration tailored for Neovim users
- Efficient pane management
- Enhanced productivity with streamlined shortcuts

## Text Copying Issues 
When working with terminal multiplexers like tmux, especially in conjunction with Neovim, copying text can be challenging. This is a common problem that many users encounter when trying to copy text from tmux panes to the system clipboard.

For a detailed explanation of this issue, see [nvim-config issue #3](https://github.com/shadielfares/nvim-config/issues/3) which describes the copying problem in detail.

### Solution: tmux-yank Plugin
To solve this copying issue, we recommend installing the [tmux-yank plugin](https://github.com/tmux-plugins/tmux-yank). This plugin enables copying to the system clipboard from tmux copy mode.

## Best Works with iTerm2

Just download it and thank me later, also you'll want to setup this for word deletion in TMUX: [video](https://www.google.com/search?q=configure+option%2Bdelete+to+delete+word+in+iterm2&oq=configure+option%2Bdelete+to+delete+word+in+iterm2&gs_lcrp=EgZjaHJvbWUyBggAEEUYOTIHCAEQIRifBTIHCAIQIRifBTIHCAMQIRifBTIHCAQQIRifBTIHCAUQIRifBdIBCDkxNDhqMGo3qAIAsAIA&sourceid=chrome&ie=UTF-8#fpstate=ive&vld=cid:faec4d81,vid:SxRrI2gKT4s,st:26)

Or you could just do this, go in iTerm2:

Profiles > Keys > Key Bindings

Add, set it to Option + Delete, the action will be `Send Hex Code`, should push up `0x1B 0x08`.

Additionally to move over a space you'll want to 

## Must Configure these shortcuts in iTerm2:

<img width="774" height="124" alt="Screenshot 2025-07-20 at 2 47 26 PM" src="https://github.com/user-attachments/assets/3111d1ca-3bbc-417f-9865-869a5f07b3ff" />


**Installation:**
1. Add the plugin to your tmux.conf:
   ```
   set -g @plugin 'tmux-plugins/tmux-yank'
   ```
2. Reload tmux configuration and install the plugin using `<Prefix> + I`

**Usage:**
- Enter copy mode with `<Prefix> + [`
- Select text with `v` (visual mode) or use mouse selection
- Copy to clipboard with `y` (copies to system clipboard)

For a visual demonstration of tmux copying techniques, check out this helpful video: https://vimeo.com/102039099

## Prerequisites 
- Ensure you have Tmux installed on your system. You can install it using your package manager, for example:
    ```sh
    sudo apt-get install tmux
    ```

## Installation 

1. Install Tmux Package Manager (TPM):
    ```
    git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
    ```
2. Clone this repository:
    ```sh
    git clone https://github.com/shadielfares/tmux-config.git ~/.config/tmux/
    ```
3. Reload the Tmux configuration:
    ```sh
    tmux source ~/.config/tmux/tmux.conf
    ```
4. Download the newly added packages, using the command (Note: You must be currently editing the tmux.conf file in tmux):
    ```
    CTRL+B, SHIFT+i
    ```

## Usage 
- **Manual Plugin Installation**: Use `<Prefix> + I` while in Tmux to manually install plugins.
