# lily-dotfiles

Clone the repo then run the install script!

```sh
git clone https://github.com/lilykiwi/lily-dotfiles.git
cd lily-dotfiles
./install.sh
```

**! ! ! This will delete any files/directories existing at the locations outlined in `./INSTALL.sh` and replace them ! ! !**

## Adding configs

Put a file in the repository, then add a line to `install.sh` constructed like this:

```sh
create_link [filename] [target-dir] #[description]
```

For a dotfile, it's best to have the filename not include the dot, then add a dot to the target dir. An example of this is `create_link zshrc ~/.`, which symlinks `~/.zshrc` .
