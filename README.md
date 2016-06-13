# pathr
Simple `$PATH` manipulation for your bashrc

# Usage

```bash
# in your .basrhc:
source /path/to/pathr

# appends to $PATH
pathr $HOME/.scripts
pathr $HOME/.npm/bin

# --pre prepends to $PATH
pathr /usr/local/bin --pre
```

## Detatching from shell rc
This was originally built so that my `$PATH` could be recreated without needing to source my shell rc file (or care about interactive mode) - specifically for `.xinitrc` with xmonad.

To do this, move all calls to `pathr` into another file, and source that wherever you need it ... but you knew that already.
