# Install

Clone this repo to anywhere you want, and add it to your path, such as:

```sh
cd $HOME
git clone https://github.com/SixArm/pandoc-from-markdown-to-pdf.git
export PATH="$PATH:$HOME/pandoc-from-markdown-to-pdf"
```


## Prerequisites

This script requires these prerequisites to be installed:

* pandoc document converter

* xelatex implementation of LaTex converters

* pygments syntax highlighting

* Bitstream Vera fonts and/or Adobe Source Pro fonts
  
If you want a different choices for any of the above,
then please contact us or open an issue, to let us know.


## macOS install with brew

Example using brew:

```sh
brew install pandoc
```

If you prefer a heavyweight install:

```sh
brew install mactex
```

If you prefer a lightweight install:

```sh
brew install basictex
eval "$(/usr/libexec/path_helper)"
# Update $PATH to include `/usr/local/texlive/2022basic/bin/universal-darwin`
sudo tlmgr update --self
sudo tlmgr install texliveonfly
sudo tlmgr install adjustbox
sudo tlmgr install tcolorbox
sudo tlmgr install collectbox
sudo tlmgr install ucs
sudo tlmgr install environ
sudo tlmgr install trimspaces
sudo tlmgr install titling
sudo tlmgr install enumitem
sudo tlmgr install rsfs
```

Verify the programs are runnable:

```sh
$ which pandoc
/usr/local/bin/pandoc

$ pandoc --version
pandoc 2.17.1.1

$ which xelatex
/Library/TeX/texbin/xelatex

$ xelatex --version
XeTeX 3.141592653-2.6-0.999993 (TeX Live 2021)
```

See also:

* [Troubleshoot XeLatex](troubleshoot-xelatex.md)
  