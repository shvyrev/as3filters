Variety of filters for image processing.

## Snapshot ##
![http://raku.to/as3filters/snapshot.png](http://raku.to/as3filters/snapshot.png)

## DEMO ##
You need to enable the camera to run this demo. If you don't have a camera then see following snapshot.

http://raku.to/as3filters/photo_booth.html

## Install ##
You need to check out and link as3filters.swc to your program.

```
% svn checkout http://as3filters.googlecode.com/svn/trunk/ as3filters
% cp as3filters/bin/as3filters.swc /path/to/your-project
```
Link as3filters.swc to your programe.
You can link the as3filters when you use Flex is as follows:
```
% cat > your-programe-config.xml
<?xml version="1.0"?>
<flex-config>
  <compiler>
    <library-path append="true">  
      <path-element>../bin/as3filters.swc</path-element>
    </library-path>  
  </compiler>
</flex-config>
%
```
Otherwise:
You can also use mxmlc's -compile.include-libraries option is as follows:
```
% mxmlc -compiler.include-libraries as3filters.swc  mydemo.as
```
## Usage ##
e.g. You can apply the twirl filter is as follows:

```
var bmd:BitmapData = new BitmapData(width, height, true);
var region:Rectangle = new Rectangle(30, 30, 90, 90)
var twirlFilter:DisplacementMapFilter = Filter.twirlFilter(bmd, region);
bmd.draw(video);
bmd.applyFilter(bmd, bmd.rect, new Point(0, 0), twirlFilter);
```

## Requirements ##
  * Flash 9
  * ActionScript3

## Author ##
  * Rakuto Furutani (http://raku.to/)

## Contribute ##
We'd like to create many kinds of interesting filters for image processing. If you have interesting ideas or skills, please contribute to develop the as3filters. If you have interest for contribute then please e-mail to rakuto@gmail.com.

Thanks!