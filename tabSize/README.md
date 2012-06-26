jquery.tabSize
==============

tabSize is a jQuery plugin for setting the CSS3 property "tab-size" of an element (if supported) to the desired size.

For browsers that do not support the property, existing tabs are *correctly* converted to spaces, to give the same visual result.

Below is an example of some demo text copied from an IDE with 4-space tabs size, to a browser with 8-space tabs size.

    |       |       |       |       |       |       |       |       |       |       |       |       |       
    Rank    Artist                  Song                                    Year
    1               Queen                   Bohemian Rhapsody               1975
    2               John Lennon             Imagine                                 1980
    3               Robbie Williams Angels                                  1997
    4               Beatles                 Hey Jude                                1968
    5               Nirvana                 Smells Like Teen Spirit 1991
    6               Oasis                   Live Forever                    1994
    7               Oasis                   Wonderwall                              1995
    8               U2                              One                                             1992
    9               Verve                   Bitter Sweet Symphony   1997
    10              U2                              With Or Without You             1987
    
After running the plugin...

    jQuery('pre').tabSize(4);


For browsers that support the tabSize, the style.tabSize of the targetted element is set to to 4.
For browsers that do not support the property, tabs are correctly converted to spaces, lining up the text in columns as expected:

    |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |
    Rank    Artist          Song                    Year
    1       Queen           Bohemian Rhapsody       1975
    2       John Lennon     Imagine                 1980
    3       Robbie Williams Angels                  1997
    4       Beatles         Hey Jude                1968
    5       Nirvana         Smells Like Teen Spirit 1991
    6       Oasis           Live Forever            1994
    7       Oasis           Wonderwall              1995
    8       U2              One                     1992
    9       Verve           Bitter Sweet Symphony   1997
    10      U2              With Or Without You     1987


Another demo with some actual code this time:

    |       |       |       |       |       |       |       |       |       |       |       |       |
	import sounds.*;
	
	var damage              :Sound  = new Damage();
	var explosion   :Sound  = new Explosion();
	var laserShoot  :Sound  = new Laser();
	var notify              :Sound  = new Notify();
	var powerUp             :Sound  = new PowerUp();

    |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |   |
	import sounds.*;
	
	var damage      :Sound  = new Damage();
	var explosion   :Sound  = new Explosion();
	var laserShoot  :Sound  = new Laser();
	var notify      :Sound  = new Notify();
	var powerUp     :Sound  = new PowerUp();

tabSize() can be run before additional methods like prettyPrint() to make your code look lovely :)