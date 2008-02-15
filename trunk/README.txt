as3filters

== DESCRIPTION
* http://code.google.com/p/as3filters/

The as3filters includes variety of filters for image processing.
There are effects of Twirl, Squeeze, Pinch, Photic tunnel, Bulge and more.

Effects:
  * Twirl
  * Pinch
  * Fisheye
  * Mirror
  * Photic tunnel
  * Bulge
  * Squeeze
  * Strech

== USAGE

e.g) You can apply filter is as follows:

  var bmd:BitmapData = new BitmapData(video.width, video.height, true);
  var region:Rectangle = new Rectangle(75, 75, 150, 150);
  var filter:DisplacementMapFilter = twirlFiter(bmd, region);
  bmd.applyFilter(bmd, bmd.rect, new Point(0, 0), filter);

If you want to know more usage then see the src/Sample.as.

== LICENSE 
See LICENSE.txt

== Author
Rakuto Furutani <http://raku.to/>

== Developers
Developers be wanted. 

== TODO
* Sphere filter
