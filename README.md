# Krita-SVG
A simple SVG exporter for KRA files.

## How it works
KRA files are really just glorified zip files, so all you have to do is unzip it and grab the layers.
When you open the file, it is unzipped in memory. Afterwards, it searches for your project folder. In your project folder is another folder with the name of `layers`. The project will then search for every folder in the `layers` folder and grab the SVG, naming it the same as the layer (it grabs `<layername>.shapelayer\` and names the SVG `<layername>.svg`). After all layers are grabbed, they are put in a zip and exported.

Made in Penguinmod, a scratch mod.
