# Game Artwork

NextUI looks for accompanying media for each emulator under `/Roms/[Emulator]/.media` folder.

Create the `.media` folder if it does not exist. 

Put an image in `PNG` format with the exact same name as the ROM file and NextUI will automatically scale the artwork.

Here's an example:

```
# With an SFC game located at:
# /Roms/SFC/My Awesome Game.smc
# The Box Art or In-game Preview is located at:

/Roms/SFC/.media/My Awesome Game.png
```

The [Artwork Scraper pak](https://github.com/josegonzalez/minui-artwork-scraper-pak/) can also be used
to automatically download artwork for your device.

For multi-Disc games - the art work should match the name of the folder - and the artwork needs to be in the .media folder along with the rest of the art, not in a separate folder within the .media folder

Here's an example:

```
Example: Awesome Game (USA) has two disks:
Awesome Game (USA) (Disc 1).chd
Awesome Game (USA) (Disc 2).chd
Awesome Game (USA).m3u
And are stored in a folder called Awesome Game (USA)

When generating art, the art needs to be titled "Awesome Game (USA)" (without the quotation marks) and the art is placed in the .media folder along with all other art, and not in a subfolder within .media
