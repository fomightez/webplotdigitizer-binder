# webplotdigitizer-binder
see if the webplotdigitizer runs in a MyBinder session

----------

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fomightez/webplotdigitizer-binder/HEAD?labpath=Trying_WebPlotDigitizer-4.6-linux-x64.ipynb)

**Current status**: This doesn't work.  
I was curious what the 'Download' in the upper right side of [the main WebPlotDigitizer](https://automeris.io/WebPlotDigitizer/) yielded and if it could ultimately be used to automate conversion of a lot of images of plots to data. The first error encountered when trying to run the executable that was unzipped from the download lead me to [here](https://stackoverflow.com/a/73733429/8508004) which was fortunate because it seemed consistent as each of those I ended up adding to `apt.txt` configuration file were listed there. Finally, it errored out running saying it needed X server or display.
I think the way to go further would be to first try a Binder where the Linux Desktop GUI is present (like the SPyder demo) and add the dependencies that I worked out in `apt.txt`. Then get WebPlotDigitizer, unpack it, and see what happens.
Alternatively I can trying using it with X server like I did with Orca and [did things with xvfb)(https://github.com/search?q=owner%3Afomightez%20xvfb&type=code).  
However, that's a lot to do when I don't know how useful what it provides it is even going to be. (I wish they had something describing what you get from the Download but I haven't found anything.)  
Plus, I found something that looks promising for what I am currently thinking I'll need:

[PlotDigitizer](https://github.com/dilawar/PlotDigitizer)  
>"A Python3 command line utility to digitize plots. This utility is useful when you have a lot of similar plots that needs to be digitized such as EEG, ECG recordings."