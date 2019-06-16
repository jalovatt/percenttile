# percenttile

I like setting my code editor to take up the left two-thirds of its screen, leaving space on the right for either a terminal or a browser's dev tools. As much as I love XFCE's tiling shortcuts, it doesn't offer enough control to do this.

This script offers a more customizable approach to window positioning by accepting percentage coordinates and dimensions based on the window's current display.

## Installation

```sh
wget https://raw.githubusercontent.com/jalovatt/percenttile/master/percenttile
chmod +x percenttile
mv percenttile ~/bin #or anywhere in your PATH
```

## Usage

```sh
percenttile x=0.5 y=0.333 w=0.2 h=1
```

## Dependencies

- xwininfo
- wmctrl
- xdotool

## Cheers To

- @jc00ke for `move-to-next-monitor`, from which this borrows a fair bit
