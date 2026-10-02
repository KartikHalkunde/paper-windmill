<p align="center">
  <img src="assets/paper-windmill.svg" alt="Colourful paper windmill" width="240">
</p>

<h1 align="center">Paper Windmill</h1>

A lightweight, single-page paper windmill project that shows how moving air can become rotational motion. It combines an interactive windmill simulator with an experiment report covering the build, observations, energy conversion, and real-world wind-powered systems.

## Run it

Open `index.html` in a modern browser. There is no build step, package manager, server, or application dependency. The page's HTML, CSS, SVG, and JavaScript are all in one file. Google Fonts are optional; the page falls back to system fonts when they are unavailable.

## Explore the experiment

1. Drag the **Wind speed** slider from 0 to 8 m/s, or choose a preset condition.
2. Watch the windmill respond and read its estimated RPM, wind level, and blade-tip speed.
3. Select **Record reading** to add a point to the chart and readings table. Use **Clear** to start a new set.
4. Read the experiment report for the materials, construction steps, observations, principle, analysis, and applications.
5. Select **Print report** to print or save the formatted report. Recorded simulator readings are included when available.

Readings are kept in browser memory for the current page session. Refreshing or closing the page clears them.

## How the simulator works

The windmill begins turning above an illustrative 0.5 m/s cut-in speed. Its target blade-tip speed is estimated as `0.6 × (wind speed − 0.5 m/s)`; RPM is then calculated using a 7.5 cm blade radius. The rotor eases toward its target speed so changes in airflow do not look instantaneous.

These values are a teaching model, **not measurements from a physical windmill**. Actual rotation depends on blade shape, balance, friction, wind direction, and construction. The report's qualitative observations describe the expected pattern: stronger airflow generally turns the blades faster.

## Project structure

| File | Purpose |
| --- | --- |
| `index.html` | Interactive simulator, chart, report, illustrations, styles, and print layout |
| `assets/paper-windmill.svg` | Transparent windmill illustration used in this README |
| `README.md` | Project overview and usage notes |

The interface uses a soft blue palette while keeping the paper windmill's original multicolour blades. Decorative clouds move across the background; reduced-motion preferences stop that animation.
