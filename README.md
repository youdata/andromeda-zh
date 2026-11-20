# 仙女座星系 · 哈勃最清晰的仙女座

仙女座星系的深度缩放导览（中文解说）：哈勃 PHAT 拼接图（ESA/Hubble heic1502a），三分之一个仙女座星系，从核球、尘埃带到外盘。

Live: https://youdata.github.io/andromeda-zh/

English version: https://youdata.github.io/andromeda/. This page has no tiles of its own: it reads the pyramid from `../andromeda/andromeda/` (the same origin on github.io).

Its fonts are in `fonts/`, trimmed to the page's characters. The narrated video is not included.

Image: NASA, ESA, J. Dalcanton, B. F. Williams, L. C. Johnson (University of Washington), the PHAT team, and R. Gendler — CC BY 4.0.

## How it is made

From `infographic-examples/andromeda-hubble/build.mjs --lang zh`, with rx (`~/rx-cli`):

```sh
rx export andromeda-hubble-zh.json --out site --app /rx-graphic-editor/web/index.html --canvas --theme dark --lock-layers --tiles dir --tile-base andromeda=../andromeda/
rx publish site --to github:youdata/andromeda-zh --yes
```
