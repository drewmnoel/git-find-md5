# What's This All About Then?
So I kept running into issues where clients ripped an open source file from a repo directly. What version is this file from? Has it been tweaked after the export from the repo? Well this tool can answer these. I basically just wrapped a gist I found onnline into a package using a PKGBUILD.

# Building
This is like Babby's First PKGBUILD. Building couldn't be easier:

```bash
$ makepkg -s
```

And there you go. If you want to install it, I recommend passing the install flag:

```bash
$ makepkg -si
```

If you want more than that, I didn't write makepkg, so just:

```bash
$ man makepkg
```

# Usage
You need the md5 of the file you want to look for, and the git repo (full history) locally. Just run git-find-md5 md5sum filename. Here's an example:
[![asciicast](https://asciinema.org/a/dzLIfOwZovahnpuIqXaZ64vOq.png)](https://asciinema.org/a/dzLIfOwZovahnpuIqXaZ64vOq)

# Contributing / License
lol
