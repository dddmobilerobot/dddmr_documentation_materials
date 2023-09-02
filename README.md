# dddmr_documentation_materials
Use following command to convert mp4 to gif
```
ffmpeg -i open_file.mp4 -filter_complex "[0:v] fps=12,scale=1280:-1,split [a][b];[a] palettegen [p];[b][p] paletteuse" open_file.gif
```
