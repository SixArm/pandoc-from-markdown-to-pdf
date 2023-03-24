# Fonts


## Font families: Bitstream Vera and Adobe Source Pro

This script repository has two font families,
and you can use these, or choose your own fonts.


### Bitstream Vera 

Bitstream Vera fonts are widely available, and use a fair license for this work.

  * main font: Bitstream Vera Serif

  * sans font: Bitstream Vera Sans

  * code font: Bitstream Vera Sans Mono


### Adobe Source Pro

Adobe Source Pro fonts are widely available, and use a fair license for this work.

  * main font: Source Serif Pro

  * sans font: Source Sans Pro

  * code font: Source Code Pro


## Install a font

We have tried various ways to install fonts.

  * Download a font file and install it via macOS "Font Book" app. This works well.

  * Download a font file to an expected directory `~/.fonts`. This works well for `fc-list` but XeLatex sometimes can't find these fonts.

  * Run `brew install --cask font-*`. This works well for general use but XeLatex sometimes can't find these fonts.


## Install a font via macOS + download + Font Book

In our experience, this way is the most likely to succeed:

  1. Download a font file

  2. Launch the macOS app "Font Book"

  3. Use the app to add the font.


## Install a font via macOS + brew 

In our experience, this way doesn't work reliably.

We explain it here, in case someone can help solve it.

Commands we try:

```sh
brew install --cask font-bitstream-vera-serif
brew install --cask font-bitstream-vera-sans
brew install --cask font-bitstream-vera-sans-mono

brew install --cask font-source-serif-pro
brew install --cask font-source-sans-pro
brew install --cask font-source-code-pro
```

In practice, the fonts sometimes are not packaged in the brew repo.

In practice, the fonts sometimes don't show up in XeLatex.


## Install a font via download and directory

In our experience, this way doesn't work reliably.

We explain it here, in case someone can help solve it.

  1. Download a font file `.ttf`.

  2. Put the file into an expected directory such as `~/.fonts`.

  3. Refresh the font cache by running `sudo fc-cache -fv`.

  4. Confirm the font has been loaded by running `fc-list | grep Foo`

  5. Add the mainfont variable to the Pandoc command: `-V mainfont="Foo"`.


## List fonts

To list the xelatex fonts that are usable:

```sh
$ fc-list
````
