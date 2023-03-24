
# Troubleshoot XeLatex

If the `xelatex` command is not found, then look for it:

```sh
find / -name xelatex
```

Example result on macOS after brew install:

```sh
/Library/TeX/texbin/xelatex
```

Then add xelatex to your path:

```sh
export PATH="$PATH:/Library/TeX/texbin/xelatex"
```

If that works, then adjust your path as you wish, such as in your `.env` file, or `~/.zshenv` file, etc.
