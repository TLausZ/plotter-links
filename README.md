```
██████╗ ██╗      ██████╗ ████████╗████████╗███████╗██████╗   ██████████████▓▒░
██╔══██╗██║     ██╔═══██╗╚══██╔══╝╚══██╔══╝██╔════╝██╔══██╗  ███████████▓▒░
██████╔╝██║     ██║   ██║   ██║      ██║   █████╗  ██████╔╝  ████████▓▒░
██╔═══╝ ██║     ██║   ██║   ██║      ██║   ██╔══╝  ██╔══██╗  █████▓▒░
██║     ███████╗╚██████╔╝   ██║      ██║   ███████╗██║  ██║  ██▓▒░
╚═╝     ╚══════╝ ╚═════╝    ╚═╝      ╚═╝   ╚══════╝╚═╝  ╚═╝

  ╞════ a short list of plotter resources ════╡
```

# Plotter links

Software, code, machines and people for drawing with a pen plotter or a laser.
Kept short on purpose: every entry here is something I would open again.

## Start here

If you have never plotted anything, the shortest path runs through three of the
links below. Draw the artwork in [p5.js](https://p5js.org) and export it with
[p5.js-svg](https://github.com/zenozeng/p5.js-svg). Run the file through
[vpype](https://github.com/abey79/vpype) once, which sorts the paths, drops the
duplicates and scales the drawing to your paper. Then send it to the machine
with [saxi](https://github.com/nornagon/saxi) if you own an AxiDraw, or with
[juicy-gcode](https://github.com/domoszlai/juicy-gcode) and a GRBL sender if you
built your own. Everything else on this page is a detour worth taking later.

## Software and tools

### Preparing the file

- [vpype](https://github.com/abey79/vpype) — CLI pipeline that cleans, sorts, scales and merges SVG before it goes to the machine
- [vsketch](https://github.com/abey79/vsketch) — sketching framework on top of vpype, live reload and parameter sliders
- [Inkscape](https://inkscape.org) — the editor most plotter extensions plug into
- [contour-drawing](https://github.com/TLausZ/contour-drawing) — my own tool, turns a photo into contour lines and writes plotter ready SVG<br><img src="https://raw.githubusercontent.com/TLausZ/contour-drawing/main/example/warhol.svg" width="150" alt="Andy Warhol portrait as a contour drawing">
- [svgsort](https://github.com/inconvergent/svgsort) — reorders paths to cut down pen travel
- [juicy-gcode](https://github.com/domoszlai/juicy-gcode) — SVG to G-code with proper curve fitting, for GRBL machines

### Drivers and firmware

- [saxi](https://github.com/nornagon/saxi) — fast AxiDraw driver with a browser UI, plans motion better than the stock software
- [AxiDraw CLI and Python API](https://axidraw.com/doc/cli_api/) — the official way to drive an AxiDraw from a script
- [Klipper](https://github.com/Klipper3d/klipper) — firmware that moves the kinematics onto a host computer, worth it for a large or fast self built machine
- [MeerK40t](https://github.com/tatarize/meerk40t) — open source control for K40 and other diode lasers
- [LightBurn](https://lightburnsoftware.com) — the paid standard for laser cutting and engraving, worth it if you burn often
- [LaserGRBL](https://lasergrbl.com) — free GRBL sender for Windows, good starting point before buying LightBurn

## Generative art and code

- [p5.js](https://p5js.org) — easiest path from an idea to an SVG you can plot
- [p5.js-svg](https://github.com/zenozeng/p5.js-svg) — SVG renderer for p5.js, saves the sketch as paths instead of pixels
- [Processing](https://processing.org) — the Java original, still the best for heavy sketches
- [Paper.js](https://paperjs.org) — vector library with boolean operations, useful for hidden line removal
- [Turtletoy](https://turtletoy.net) — turtle graphics in the browser, every sketch exports plotter ready SVG
- [Krbn](https://github.com/vpalos/Krbn) — renders 3D scenes as pencil strokes, hidden lines and hatching solved analytically<br><img src="https://raw.githubusercontent.com/vpalos/Krbn/main/examples/gallery/16-gravity-well.svg" width="150" alt="A sphere resting in a gravity well, drawn in hatching">
- [ln](https://github.com/fogleman/ln) — 3D scene renderer that outputs line art instead of pixels
- [Generative Artistry](https://www.generativeartistry.com) — tutorials that rebuild classic plotter works step by step
- [Sighack](https://sighack.com) — Manohar Vanga on fills, hatching and space filling curves, with code
- [Inconvergent](https://inconvergent.net/generative/) — Anders Hoff's writings on the algorithms behind his plots
- [The Coding Train](https://thecodingtrain.com) — video course for everything from noise fields to L-systems

## Machines and materials

- [AxiDraw](https://axidraw.com) — the reference pen plotter, holds almost any pen
- [NextDraw](https://bantamtools.com/products/bantam-tools-nextdraw) — successor built by Bantam Tools, faster and quieter
- [Line-us](https://www.line-us.com) — small robot arm, cheap way to find out whether plotting is for you
- [BrachioGraph](https://www.brachiograph.art) — build your own from two servos and a clothes peg
- [EggBot](https://github.com/evil-mad/EggBot) — for drawing on spherical objects
- [AxiDraw wiki](https://wiki.evilmadscientist.com/AxiDraw) — manuals, pen holder mods, troubleshooting
- [Evil Mad Scientist pen shop](https://shop.evilmadscientist.com/productsmenu/968) — pens tested to work in a plotter
- [HP Computer Museum](https://www.hpmuseum.net) — documentation for vintage HP pen plotters still in use

## Community and inspiration

- [awesome-plotters](https://github.com/beardicus/awesome-plotters) — the big list, go there when this one is too short
- [DrawingBots](https://drawingbots.net) — hub with software comparisons and an active Discord
- [r/PlotterArt](https://www.reddit.com/r/PlotterArt/) — daily plots, and a [wiki](https://www.reddit.com/r/PlotterArt/wiki/index) with pen and paper recommendations
- [r/plotters](https://www.reddit.com/r/plotters/) — the hardware side, repairs and vintage machines
- [r/proceduralgeneration](https://www.reddit.com/r/proceduralgeneration/) — algorithms first, plenty of it ends up on paper
- [Generative Hut](https://www.generativehut.com) — interviews and tutorials from plotter artists
- [Genuary](https://genuary.art) — one generative prompt a day every January
- [Tyler Hobbs](https://www.tylerxhobbs.com/words) — essays on generative work, start with [flow fields](https://tylerxhobbs.com/essays/2020/flow-fields)
- [Amy Goodchild](https://www.amygoodchild.com/blog) — clear write-ups of her own plotter projects
- [#plottertwitter](https://www.instagram.com/explore/tags/plottertwitter/) — the tag survived the move off Twitter

## Contributing

Open an issue or a pull request. One line per link, say what it is good for.

## License

[CC0](LICENSE). Do whatever you want with this list.
