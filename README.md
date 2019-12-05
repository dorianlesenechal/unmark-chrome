# NOTE

## Files of this fork are updated to work with bookmarks.lesenechal.eu
## Ton install the extension, just download the latest release of the extension

## Hey There
Here is our code for Unmark's Chrome extension. Feel free to use it. Below are a few instructions on how to customize it to work with your domain.

## Chrome Extensions Tutorial
Not familiar with how to create Chrome extensions? [Click here to read the documentation](http://developer.chrome.com/extensions/index.html).

## Using your own host
If you want to simply change the endpoint for this extension it's pretty simple.

* Open `manifest.json` and find the block that looks like:

```
"permissions": [
    "tabs",
    "contextMenus",
    "*://unmark.it/"
  ],
```

Change the last line to match your site.

* Open `js/unmark/base.js` and change line 2 to point to the correct endpoint.

```
unmark.host = 'https://unmark.it';
```

* Save

## Loading your version in Chrome
Now you should be able to load the unpacked extension locally and test. To do that simply follow these instructions:

* Go To `chrome://extensions` in Chrome.
* Check the `Developer Mode` checkbox.
* Click the button that says `Load unpacked extension...`.
* Choose the location of your code.


## Shipping your version
When you are ready to ship, just choose the `Pack extension...` button and follow the instructions.
