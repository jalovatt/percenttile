# percenttile

I like setting my code editor to take up the left two-thirds of its screen, leaving space on the right for either a terminal or a browser's dev tools. As much as I love XFCE's tiling shortcuts, it doesn't offer enough control to do this.

`percenttile` offers a more customizable approach to window positioning by accepting percentage coordinates and dimensions based on the window's current display.

**Note:** The script is coded with my particular setup in mind - two monitors with the same resolution, either horizontal or stacked, with a 28px XFCE panel reserving space at the bottom edge of the overall desktop. The panel size can be changed (or set to 0) at the top of the script.

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

Apps that are line- or column-based, like a terminal, may need some fiddling to get them exactly where you want. For instance, I have to use a height of `0.98` with my terminal to fill as much of the available space as possible without adding a line and spilling past the bottom panel.

## Dependencies

- xwininfo
- wmctrl
- xdotool

## Cheers To

- @jc00ke for `move-to-next-monitor`, from which this borrows a fair bit
