# dotfiles for dotdrop

This repository is a template for the dotfiles managed by [dotdrop](https://github.com/deadc0de6/dotdrop).

**This repository may include your private data and should not be shared publicly.**

You'd better to fork this repository and use it as a template for your own dotfiles.

## Installation

The installation is managed by [dotfiles](https://github.com/entelecheia/dotfiles) repository through [chezmoi](https://chezmoi.io/) tool.

At initialization of chezmoi, you should specify your forked repository as your repository for dotdrop.

## [`dotfiles-setup-dotdrop` Script](https://dotfiles.entelecheia.ai/usage/dotdrop/)

The `dotfiles-setup-dotdrop` script is designed to help you set up or update the Dotdrop repository and deploy the dotfiles to your system. To use this script, follow these steps:

1. **Configure Environment Variables (optional):**
   If you have specific values for `DOTDROP_PROFILE` or `DOTDROP_CONFIG`, you can set these environment variables before running the script. Otherwise, the script will use the default values specified in the script.

   ```
   export DOTDROP_PROFILE="my-profile"
   export DOTDROP_CONFIG="/path/to/config.yaml"
   ```

2. **Run the Script:**
   Execute the `dotfiles-setup-dotdrop` script:

   ```
   dotfiles-setup-dotdrop
   ```

   This script will perform the following tasks:

   - Ensure that `${HOME}/.local/bin` is included in your `PATH`.
   - Clone or update the Dotdrop repository.
   - If you have a local Dotdrop repository, it will copy or update the repository to `${HOME}/.config/dotdrop`.
   - If you have a remote repository, it will clone or update the repository accordingly.
   - Install or update dotfiles using the specified Dotdrop profile and configuration.

After running the `dotfiles-setup-dotdrop` script, your dotfiles will be managed and deployed using Dotdrop, and your system should be configured according to the specified Dotdrop profile.

## License

This repository is licensed under the MIT License.
