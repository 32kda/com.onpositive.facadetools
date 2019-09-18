# com.onpositive.facadetools
X-Plane facade tools project contains two small Java-based tools I've created for more convenience in creating and viewing X-Plane facades

## Prerequisites
You'll need at least Java 8 JRE or JDK to use these programs. 

You can get JRE e.g. [here](http://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html "")  

See section "JAR Files as Applications" [here](https://docs.oracle.com/javase/tutorial/deployment/jar/run.html "") on how to launch executable jar file. 

## Facade viewer
Facade Viewer can be used for viewing facades - it will show first wall defined in facade description and markup lines for it, dividing it into regions.
Usage - simply choose "open" action on toolbar and select folder, facades from which you want to view. Facades list (if they are present in given folder) will be shown in the left part of window, if you click some facade file - it's image and markup will be shown in the right part. 
Use "refresh" button to update list if you added/removed files in it.

![Facade viewer](https://32kda.github.io/com.onpositive.facadetools/viewer1.png "Facade viewer")

[Download](https://32kda.github.io/com.onpositive.facadetools/facadeviewer-0.0.1.jar "facadeviewer-0.0.1.jar") 

## Facade marker
Facade Marker was created for simplifying creation of facade markup, which automatically calculates image S-T coordinates and then copies them to clipboard.

For example, to make vertical markup for new facade, click "Mark Vertical", place lines on image using left mouse button (in any order, they will be ordered automatically) and click "End Mark". 

![Vertical marking process](https://32kda.github.io/com.onpositive.facadetools/marker1.png "Vertical marking process")

Smth like following will be copied to clipboard, which you can use in your facade file. 

`BOTTOM 0.755859375 0.835937500`  

`MIDDLE 0.835937500 0.916015625`  

`TOP 0.916015625 1.000000000`

Default type constants (TOP, BOTTOM, etc) are generated for markup, change them manually to what you need if necessary.
You can use Right Mouse Button, if you want to delete previously added line.

Using same way you can mark horizontal lanes - just use "Mark Horiz", place lines you need and choose "End Mark" You'll get smth like following in the clipboard:

`LEFT 0.001953 0.210938`

`CENTER 0.210938 0.435547`

`CENTER 0.435547 0.560547`

`CENTER 0.560547 0.664063`

`RIGHT 0.664063 0.996094`

![Horizontal marking process](https://32kda.github.io/com.onpositive.facadetools/marker2.png "Horizontal marking process")

[Download](https://32kda.github.io/com.onpositive.facadetools/facademarker-1.1.0.jar "facademarker-1.1.0.jar")

Read more about S-T coordinates and facade creation [here](https://developer.x-plane.com/article/facade-creation/#Understanding_S-T_coordinates)

 