# Description
This is a showcase to demonstrate printing web content of a Omnis Studio oBrowser GUI component. 

## Getting started

### Prerequisites
* Omnis Studio 8.1.6 or higher
* Some basic understanding of Javascript
* Some knowledge of the Omnis HTML controls. Documentation about the structure and usage of the oBrowser component and Omnis HTML controls can be found in the [Omnis Programming Manual](https://omnis.net/documentation/programming/11wincomps.html#obrowser).

### Installing
#### Mac
1. If you did not use custom HTML controls before you als have to set the user HTML control folder in the config.json folder. Otherwise you can skip to the step where you copy the HTML control to Omnis Studio/htmlcontrol folder
1. Open Finder and goto the folder ``~/Library/Application Support/Omnis/Omnis Studio 8.1.6/studio``
1. Open de file ``config.json`` in a texteditor
1. Change the property ``defaultHtmlcontrolsFolderInDataFolder`` from ``false`` to ``true`` and save the file.
1. Copy the HTML control folder ``printSample`` to the folder ``~/Library/Application Support/Omnis Software/Omnis Studio 8.1.6``


## Implementation of the print function.
There are two ways to do it. For both you need to add some javascript to the webcontent. I am sure this can be done in several ways. Below you can find two simple ways. There actually quite similar.

1. Implement a print function in the OmnisCallBackObject 
1. Implement a print button in the htm page

The difference between these is that with the first one you have an Omnis pushbutton to invoke the print of the contents. With the latter you have a HTML button which prints the contents. Both have theire (dis)advantages. With both methods it comes down to a javascript command window.print(). 
