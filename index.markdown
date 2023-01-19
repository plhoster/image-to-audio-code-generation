---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
- Project by <a href="https://github.com/PicoLuetjens">Pico Lütjens</a>

# General
This tool generates audio snippets from an image using Processing and the Earsketch Environment. The generated snippet depends on parameters that are taken into account such as the width of the image, percentage of bright parts, percentage of dark parts etc.

# Installation
The main program is written in Processing. So you need to download Processing from the Foundation Website <a href="https://Processing.org">here</a>.<br>
Then clone the <a href="https://github.com/PicoLuetjens/Image-to-Audio-Code-Generation">repository</a> from github to your local computer.

# Usage
Paste the target image in the data-Folder and open the GenerateCode.pde file with the Processing IDE.<br>
Change line 9 to load the new target image:
```Processing
source = loadImage("NewTargetImage.png")
```

By default the GeneratedCode.txt file will be overwritten. If you want to keep it change line 12 to output to another path:
```Processing
generator.savetofile("data/outputpathfile.txt")
```

If you run the program a python code file will be generated and written to the date folder.<br>
Copy the code in the file and go to <a href="https://earsketch.gatech.edu/landing/#/">Earsketch</a>.<br>
Go to "start coding" and select python as the language. Then paste your text to the python file and click on run.<br>
Now the file will be interpreted and a sound will be generated. To play the sound press the play button on the top.