
# VR

A video.js plugin that turns a video element into a HTML5 Panoramic 360 video player. Project video onto different shapes. Optionally supports Oculus Rift, HTC Vive and the GearVR.

[View Demo](https://videojs-vr.s3.amazonaws.com/0.2.2/example.html)


### Build
```
npm install
npm run build
```

### Download Local Samples
```
npm run local-samples
```

### Run
```
npm run serve
```

## Examples
To test locally, visit localhost:3000/example.html [Hosted example](https://videojs-vr.s3.amazonaws.com/0.2.2/example.html)

For an iframe example using the allowvr attribute, visit localhost:3000/iframe.html [Hosted example](https://videojs-vr.s3.amazonaws.com/0.2.2/iframe.html)

To test macOS and iOS devices with Safari, you need a local/same domain source file. After running `npm run local-samples`, visit localhost:3000/example-local.html [Hosted example](https://videojs-vr.s3.amazonaws.com/0.2.2/example-local.html)

## Setting up your own player

Download:
* [VideoJS](http://www.videojs.com)
* [Three.js](http://threejs.org)
* [webvr-boilerplate](https://github.com/borismus/webvr-boilerplate)
* [webvr-polyfill](https://github.com/borismus/webvr-polyfill)

In your web page (adjust to match the location/layout of your downloaded libs - order is important!):

    <link rel="stylesheet" href="dist/videojs.css">
    <script src="dist/video.js"></script>
    <script src="dist/js/three.js"></script>

    <script type="text/javascript" src="dist/js/VRControls.js"></script>
    <script type="text/javascript" src="dist/js/VREffect.js"></script>
    <script type="text/javascript" src="dist/js/webvr-polyfill.js"></script>
    <script type="text/javascript" src="dist/js/webvr-manager.js"></script>

    <script type="text/javascript" src="dist/js/videojs.vr.js"></script>
    <script type="text/javascript" src="dist/js/webvr.config.js"></script>

Host on a HTTP Server that supports byte range requests if you want the seek bar to work (e.g. Apache).

## Oculus Rift and HTC Vive Support
This plugin leverages the [webvr-boilerplate](https://github.com/borismus/webvr-boilerplate) project (which in turn uses [webvr-polyfill](https://github.com/borismus/webvr-polyfill) and [three.js](https://github.com/mrdoob/three.js)) to create a 'responsive VR' experience across multiple devices.

Oculus Rift and HTC Vive playback requires Firefox Nightly with the WebVR addon, or experimental WebVR-enabled builds of Chromium. Go to [WebVR.info](http://www.webvr.info) for more info.

GearVR playback requires the latest Samsung Internet for Gear VR with WebVR support enabled. Go [here](https://mail.mozilla.org/pipermail/web-vr-discuss/2016-April/001054.html) for more info.

## Credits ##

This project is a conglomeration of a few amazing open source libraries.

* [VideoJS](http://www.videojs.com)
* [Three.js](http://threejs.org)
* [webvr-boilerplate](https://github.com/borismus/webvr-boilerplate)
* [webvr-polyfill](https://github.com/borismus/webvr-polyfill)

## Support ##
This work is sponsored by [Brightcove](https://www.brightcove.com), [HapYak](http://corp.hapyak.com/) and [StreamShark](https://streamshark.io)


## Release History
0.2.2
0.2.0
