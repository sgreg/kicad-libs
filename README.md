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
Footprints:

1. Clone the repository somewhere to your local system.
2. Open the KiCad Footprint Library Wizard in Pcbnew (Preferences -> Footprint Library Wizard)
3. Select "Files on my Computer" and press Next
4. Select a library from the location you cloned the repository into (/path/to/repo/footprints/\*.pretty/) and press Next
5. Review and confirm, press Next
6. Choose if you want the footprint to be available globally or only in the current project (whichever suits you) and press Finish

