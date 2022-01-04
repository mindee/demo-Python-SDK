# Sample files

These samples all use Juypter Notebooks.

To start a Jupyter Notebook:

1. [install Jupyter](https://jupyter.org/install)
2. Start the Jupyter instance ```jupyter notebook```
3. A tab will open in the browser and you can naviagte to the ipynb Jupyter file you wish to examine.

To use these dociuments, you'll need a [Mindee API key](platform.mindee.com).  Each APi endpoint uses a different key - so you must generate the key for the endpoint you are working with.


There are 4 docs:

1. invoice
2. receipt
3. passport
4. license plates

Additionally, there are sample images for all of the endpoints. To test with a new document, sinply add to the directory, and change the path for the 'image' variable.

## Drawing the polygon boxes

In the invoice and license plate examples - not only are the various values extracted from the document, but a box is drawn around the location of several of the attributes. This is done by retrieving the polygon data from the Mindee response, converting to a pixel corrdiante, and the using openCV to draw a rectangle on the image.