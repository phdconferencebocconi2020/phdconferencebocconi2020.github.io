# Website Resources for the PhD Virtual Conference @ Bocconi 2020

This repository contains all resources to create the website we will use for the PhD Virtual Conference at Bocconi University.


## Generating a local preview of the website

The website is generated using Jekyll.
Jekyll is a plug-in package (called _gem_) for Ruby.
The installation instructions differ depending on the Operating System.

- macOS: follow [these](https://jekyllrb.com/docs/installation/macos/) instructions, (prefer `homebrew` to `rbenv`).
- Linux: follow [these](https://jekyllrb.com/docs/installation/ubuntu/) instructions for Ubuntu (non-Ubuntu users will figure it out).
- Windows: follow [these](https://jekyllrb.com/docs/installation/windows/#installation-via-bash-on-windows-10) instructions. You need to set up the Windows Subsystem for Linux (WSL) (info [here](https://docs.microsoft.com/en-us/windows/wsl/install-win10?redirectedfrom=MSDN)).

When you are done installing Ruby, follow Jekyll's [QuickStart guide](https://jekyllrb.com/docs/) (specifically, steps 2 and 3).

Once everything is in place, clone this repository to your computer.
Open a terminal, navigate to the folder and run

```bash
$ bundle exec jekyll serve
```

This will create some output that looks like this.

```
Configuration file: /mnt/c/Users/Andrea/Git/bocconi-phd-conference-2020/_config.yml
            Source: /mnt/c/Users/Andrea/Git/bocconi-phd-conference-2020
       Destination: /mnt/c/Users/Andrea/Git/bocconi-phd-conference-2020/_site
 Incremental build: disabled. Enable with --incremental
      Generating...
       Jekyll Feed: Generating feed for posts
                    done in 0.607 seconds.
 Auto-regeneration: enabled for '/mnt/c/Users/Andrea/Git/bocconi-phd-conference-2020'
    Server address: http://127.0.0.1:4000/
  Server running... press ctrl-c to stop.
```

This means that you can open a browser, enter `127.0.0.1:4000` in the URL bar.
You will see the local version of the website, and you will be able to interact with it as if it was a normal website.
Note that you need to keep the terminal open and running to keep the local preview alive.

Once you are done with the preview, go back to the terminal and press <kbd>Ctrl</kbd>+<kbd>C</kbd> to quit Jekyll.
Only then you can close the terminal.


## Edit content

There are two sort of places where you can change content.
If you want to change stuff in the main part of the website (e.g., the main content), then you should look at the markdown files.
At the time of writing, the files are:

- [`index.md`](./index.md) (the landing page of the website)
- [`timeline.md`](./timeline.md)
- [`logistics.md`](./logistics.md)
- [`about.md`](./about.md)

Each file corresponds to one page of the website.
Each of these files are written in [Markdown](https://daringfireball.net/projects/markdown/syntax).

If, instead, you want to change stuff in the header and footer of the website, you should take a look at the file [`_config.yml`](./_config.yml).
Changing the theme of the website is a different subject and I will not cover it here.
Google for themes for GitHub Pages to have an idea of how to do it.
