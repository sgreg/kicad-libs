## My component and footprint library for KiCad


### Content
* Nokia_5110-3310_LCD
    * Nokia 5110 / 3310 LCD as used in breakout boards from [Sparkfun](https://www.sparkfun.com/products/10168), [Adafruit](https://www.adafruit.com/product/338), and others, to use the "clip-in" LCD from the breakout board in one's own custom PCB
    * Footprint with and without solder paste layer (to your own liking when ordering stencils)
* LCD_Connectors
    * FPA-WZA201-08-LF connector for [Olimex Nokia 3310 LCD](https://www.olimex.com/Products/Components/LCD/LCD-DISPLAY-NOKIA3310/)
* Artwork_4chord-midi
    * Artwork for the [4chord MIDI project](https://github.com/sgreg/4chord-midi)

### Usage

Add this repo as a submodule to your project.

```
mkdir Libraries && cd Libraries
git submodule add https://github.com/sgreg/kicad-libs.git sgreg-kicad-libraries
```

If you want 3D models, you'll need to
open `Preferences` and `Configure Paths` then add the following enviorment variable:

```
Name: SGREG_3DMODELS
Path: <Path to folder>
```

Add footprints and symbols by using the `Preferences > Manage Symbol Libraries` and
`Preferences > Manage Footprint Libraries`

And if you use kibot, add this to your `pre_flight`

```
preflight:
  ...
  set_text_variables:
    - name: "SGREG_3DMODELS" # 3D models for sgreg nokia 5110 Library
      command: "echo 'Hardware/MYBOARD/Libraries/sgreg-kicad-libraries/3d'"
```
