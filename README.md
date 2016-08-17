# \<filtered-video\>

university exercise

## In case you have no tooling at all

First install node (LTS should do) - node and npm should be on the path.

```
$ npm install -g bower
$ bower install
```

## Install the Polymer-CLI

Make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

## Viewing Your Application

```
$ polymer serve
```

## Further stuff

This is not a piece on polymer best practice (there is a lot of room for improvement).

The app works in modern Chrome and Firefox Browsers (Edge 14 doesn't work - didn't test Safari 
but I suspect it won't work).

The easiest way to test the component (other than using it in your project) is to navigate to
[this location](http://localhost:8080/components/filtered-video/demo/) (if your running 
instance served via the polymer cli uses another port you have to adjust the URL).

The app should cope with the video formats recognized by the respective browser.
The filter panel is not extremely hardened (only normal 3x3 or 5x5 kernels are
supported - hard validation is not implemented).