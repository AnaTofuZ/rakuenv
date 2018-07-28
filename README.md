# p6env

env family for perl6

## Install

Note that if you are familiar with `*env` such as rbenv or plenv,
then you can safely ignore this describution, I think:)

1. Clone p6env into `~/.p6env`.

    ~~~ sh
    git clone https://github.com/skaji/p6env ~/.p6env
    ~~~

2. Add `~/.p6env/bin` to your `$PATH`.

   * For **bash**:
     ~~~ bash
     $ echo 'export PATH="$HOME/.p6env/bin:$PATH"' >> ~/.bash_profile
     ~~~

   * For **Ubuntu Desktop**:
     ~~~ bash
     $ echo 'export PATH="$HOME/.p6env/bin:$PATH"' >> ~/.bashrc
     ~~~

   * For **Zsh**:
     ~~~ zsh
     $ echo 'export PATH="$HOME/.p6env/bin:$PATH"' >> ~/.zshrc
     ~~~

   * For **Fish shell**:
     ~~~ fish
     $ set -Ux fish_user_paths $HOME/.p6env/bin $fish_user_paths
     ~~~

3. Set up rbenv in your shell.

   ~~~ sh
   $ ~/.rbenv/bin/rbenv init
   ~~~

4. Restart your shell so that PATH changes take effect. (Opening a new
   terminal tab will usually do it.)

5. Install [perl6-build](https://github.com/skaji/perl6-build),  which provides the
   `p6env install` command that simplifies the process of
   installing new Perl6 versions.

   ~~~ sh
   $ git clone https://github.com/skaji/perl6-build ~/.p6env/plugins/perl6-build
   ~~~

## Usage

~~~ sh
$ p6env install -l

$ p6env install rakudo-star-2018.04

$ p6env global rakudo-star-2018.04

$ perl6 -v
~~~

## License

p6env is a fork of https://github.com/rbenv/rbenv;
you can redistribute it and/or modify it under the same terms as rbenv itself.

See [LICENSE](LICENSE) for rbenv's license.
