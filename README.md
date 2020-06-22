# OOHG - Object Oriented (x)Harbour GUI

OOHG is an object-oriented extended adaptation of the MiniGUI library for building Windows applications using [Harbour](https://harbour.github.io/) and [xHarbour](http://www.xharbour.org/) languages.

Its 32 and 64 bits libraries offer an easy but yet powerfull way of adding a graphical user interface to your (x)Harbour applications under Windows.   

<font size="+1">
```
#include "oohg.ch"

PROCEDURE Main

   DEFINE WINDOW Main TITLE 'Hello Wold!'

      @ 20, 20 LABEL lbl_About ;
         AUTOSIZE ;
         VALUE ( "Built with:" + CRLF + ;
                 OOHGVersion() + CRLF + ;
                 hb_Compiler() + CRLF + ;
                 Version() )

      @ 120, 20 IMAGE img_OOHG ;
         PICTURE "oohg.bmp"

   END WINDOW

   CENTER WINDOW Main
   ACTIVATE WINDOW Main

RETURN
```
</font>

![](hello.png)
