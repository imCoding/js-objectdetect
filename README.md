# js-objectdetect #

*js-objectdetect* is a javascript library for real-time object detection.

This library is based on the work of Paul Viola and Rainer Lienhart and compatible to stump based cascade classifiers used by the OpenCV object detector.

All modern browsers including IE 9+ are supported.

### Classifier ###
All stump based classifiers used by [OpenCV](http://opencv.org/). Classifiers for face, hand and eye detection are already included. More can be found on the web ([classifier repository](http://alereimondo.no-ip.org/OpenCV/34)).

![face](http://mtschirs.github.com/js-objectdetect/media/face.png) ![eye](http://mtschirs.github.com/js-objectdetect/media/eye.png) ![fist](http://mtschirs.github.com/js-objectdetect/media/handfist.png) ![hand](http://mtschirs.github.com/js-objectdetect/media/handopen.png)

### Examples ###

*js-objectdetect* can be used for object detection, tracking and, in combination with mordern HTML5 features such as [WebRTC](http://caniuse.com/stream), for all sorts of augmented reality applications that run in the browser without any plugin.

![glasses](http://mtschirs.github.com/js-objectdetect/media/glasses.gif)

![gesture](http://mtschirs.github.com/js-objectdetect/media/gesture.gif)

### Usage - jQuery ###

The provided jQuery plugin provides a simple interface to the object detection library:
	
	<script src="js/objectdetect.js"></script>
	<script src="js/objectdetect.frontalface.js"></script>

	<script src="js/jquery.js"></script>
	<script src="js/jquery.objectdetect.js"></script>

	<img id="image" src="image.png">
	<script>
		$("#image").objectdetect("all", {classifier: objectdetect.frontalface}, function(coords) {
			...
		});
	</script>

### Download ###

- The actual library:
	- [objectdetect.js](https://raw.github.com/mtschirs/js-objectdetect/master/js/objectdetect.js)
- One or more classifier:
	- [objectdetect.frontalface.js](https://raw.github.com/mtschirs/js-objectdetect/master/js/objectdetect.frontalface.js)
	- [objectdetect.eye.js](https://raw.github.com/mtschirs/js-objectdetect/master/js/objectdetect.eye.js)
	- [objectdetect.handopen.js](https://raw.github.com/mtschirs/js-objectdetect/master/js/objectdetect.handopen.js)
	- [objectdetect.handclosed.js](https://raw.github.com/mtschirs/js-objectdetect/master/js/objectdetect.handclosed.js)
- The jQuery plugin:
	- [jquery.objectdetect.js](https://raw.github.com/mtschirs/js-objectdetect/master/js/jquery.objectdetect.js)

### License ###

*js-objectdetect* is distributed under [GPL3](https://github.com/mtschirs/js-objectdetect/LICENSE.txt). The included classifiers are subject to [their own licenses](https://github.com/mtschirs/js-objectdetect/CLASSIFIER-LICENSES.txt).