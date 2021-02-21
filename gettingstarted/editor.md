# Editors

There are several different editors people use:

- [Vim](#vim)
- [VSCode](#vscode)
- [IntelliJ](#intellij)
- [Sublime](#sublime_text)

It's worth finding somebody in Otrego who's already using the editor you're
interested in using and asking them how they've configured their editor.

## Vim

[Vim](https://www.vim.org/) is an open source text-editor that comes bundled
with most Unix-style systems, but can be installed on pretty much any system.
It has a bit of a learning curve but is very powerful and versitile  once you
learn how to use it.

**Users**

- @Kashomon

**Resources**

*   [vimtutor](https://superuser.com/questions/246487/how-to-use-vimtutor) --
  still the best introduction to basic vim functionality.
*   [openvim.com](https://openvim.com/) has a nice vimtutor-like experience on the web.
*   Plugins Manager: A plugin manager is basically required to have a good Vim
    experience. There are several good options to choose from. There's a useful
    (although somewhat dated) discussion on
  [Stack Overflow](https://vi.stackexchange.com/questions/388/what-is-the-difference-between-the-vim-plugin-managers).
    *   [Vundle](https://github.com/VundleVim/Vundle.vim) -- A very popular plugin
        manager (@Kashomon uses it), and it works quite well. Like `apt` for Vim.
        In maintenance mode, but still works quite well.
    *   [VimPlug](https://github.com/junegunn/vim-plug) -- Another very popular
        plugin manager like Vundle, but is still maintained.
    *   [Vim8 Plugins](https://medium.com/@paulodiovani/installing-vim-8-plugins-with-the-native-pack-system-39b71c351fea) --
        Vim8 now has plugin-logic built into the system. It's a bit manual compared
        to Vundle or VimPlug, but it works quite well.
*   [Vim Awesome](https://vimawesome.com/) -- Useful collection of Plugins
*   [Vim the Hard Way](https://learnvimscriptthehardway.stevelosh.com/) -- Very
    detailed introduction to vim


**Plugins**

A collection of plugins you'll want for working on Otrego.

*   https://github.com/fatih/vim-go -- The canonical plugin for Vim & Golang.
*   https://github.com/ycm-core/YouCompleteMe -- Amazing autocomplete plugin for vim
*   https://github.com/tpope/vim-sensible -- Sensible collection of vim-defaults
*   https://github.com/kien/ctrlp.vim -- Great fuzzy matcher for vim
*   https://github.com/preservim/nerdcommenter -- Useful for auto-commenting plugin
*   https://github.com/ervandew/supertab -- Simple tab-complete plugin
*   https://vimawesome.com/plugin/fugitive-vim -- Useful vim plugin for git

## VSCode

VSCode is a very popular programming development environment (AKA IDE) that is
open source and developed by Microsoft. It has a huge amount of functionality
and is very well supported.

**Users**

*   @RodDeacon
*   @TrevorPeters
*   @TamaBrian
*   @mhoak

## Install

1. Install Visual Studio Code.  <https://code.visualstudio.com/Download>

    *   Check to ensure that the "Terminal" command line feature is installed
        with VS Code.  (See "Terminal" menu on topline header)
    *   If not installed, install the Terminal feature from the Visual Studio
        catalog of VS Code extensions.

2.  Install the GoLang language extension for VS Code,
    [Open the VSCode Marketplace](https://marketplace.visualstudio.com/vscode)
    and search for "GO".

3.  We use GitHub collaboration tools. GitHub is a website and cloud-based
    service that helps developers, and their collaborators, store and manage
    their code, as well as track and control changes to their code. Learn
    more about
    [GitHub from kinsta.com/knowledgebase](https://kinsta.com/knowledgebase/what-is-github/)

    *   For using GitHub we recommend using Git commands from the Terminal.
    *   We don't recommend installing the GitHub extension for VS Code.

## Sublime Text

**Users**

*   @jonathanmli

**Resources**

*   This [workflow tutorial](https://www.alexedwards.net/blog/streamline-your-sublime-text-and-go-workflow)
    is a great guide towards setting up features such as auto-formatting,
    auto-linting, and auto-completion
