# pandoc-from-markdown-to-pdf

Use the pandoc command to convert from a markdown file to a PDF file.

This tool uses our favorite settings for layouts, styles, fonts, etc.

You can edit this tool as you wish.

Syntax:

```sh
pandoc-from-markdown-to-pdf <args>
```

Syntax for typical use:

```sh
pandoc-from-markdown-to-pdf <input.md> -o <output.pdf>
```

Example:

```sh
$ pandoc-from-markdown-to-pdf example.md -o example.pdf
```


# Install

Clone this repo to anywhere you want, and add it to your path, such as:

```sh
cd $HOME
git clone https://github.com/SixArm/pandoc-from-markdown-to-pdf.git
export PATH="$PATH:$HOME/pandoc-from-markdown-to-pdf"
```


# Availability

This tool is currently tested on macOS Monterey.

If you want to use this tool on other systems,
then please contact us, or open an issue, to let us know.


# Prerequisites

This script requires these prerequisites to be installed:

* pandoc document converter

* xelatex implementation of LaTex converters

* pygments syntax highlighting

* Bitstream Vera fonts
  
If you want a different choices for any of the above,
then please contact us or open an issue, to let us know.


## macOS install

Example using brew:

```sh
brew install pandoc
brew install mactex
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

## Fonts

This script uses Bitstream Vera fonts because they are
widely available, and use a fair license for this work.

  * main font: Bitstream Vera Serif

  * sans font: Bitstream Vera Sans

  * code font: Bitstream Vera Sans Mono

For help with fonts, see the `fonts` directory:

https://github.com/sixarm/pandoc-from-markdown-to-pdf


## Thanks

Thanks to https://learnbyexample.github.io/customizing-pandoc/

Thanks to https://github.com/sixarm/sixarm-unix-shell-functions/


## Tracking

  * Package: pandoc-from-markdown-to-pdf
  * Version: 1.0.0
  * Created: 2022-03-12T22:05:34Z
  * Updated: 2022-09-08T21:42:49Z
  * License: GPL-2.0-or-later or contact us for custom license
  * Contact: Joel Parker Henderson (joel@sixarm.com)
  