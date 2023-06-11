PICTCanvas 1.0

An RB custom class with superclass canvas that can display pictures and picture files. Version 1.0 has the following features:

		¥ drop pictures or picture files on the canvas to change the current picture
		¥ button and sticky button properties to make the picture a button
		¥ scrolling around with the mouse if the picture is larger than the canvas
		¥ automatic centering of pictures smaller than the canvas
		¥ framing with variable frame size (appearance manager savy)

New Events:

Pushed

the button has been pushed (be it sticky or not)

ButtonChanged( pushed as Boolean )

the sticky button state has been changed to pushed 

PictureChanged (p as Picture, name as String)
 
the picture of the canvas has been changed by dropping an object on it
p is the new picture
name is the name of the picture file, empty ("") if a picture itself has been dropped

Methods:

DrawPicture()

force drawing of the current picture 

DrawBox()

force drawing of the frame if draw_frame = true

Invert_Frame()

invert the frame (exchange top, left frame color with bottom, right color)

Set_BackgroundColor( c as Color)

set the background color for the background area; does not change fill_background property but forces redrawing of the picture and frame

Set_Picture( p as Picture )

set the canvas picture to p

Properties:

draw_frame as Boolean

if true,  the picture is drawn in a frame, default is true

enable_scroll as Boolean

if true, the user may scroll a picture larger than the canvas by dragging it with the mouse

fill_background as Boolean

if true, the canvas will be filled with the background color selected or the appearance manager FillColor

frame_inverted as Boolean

if true, the frame is drawn inverted (don't set this property, use the Invert_Frame() method instead)

frame_width as Integer

the width of the frame in pixels, default is 1

is_button as Boolean

if true, the canvas acts like a button (behavior depending on the sticky property)

sticky as Boolean

if true and is_button is true, the button will be a switch instead of a one-click button

allow_drop as Boolean

if true, the user can drop files or pictures on the canvas to change the picture, default is true

Requirements:

RB release 1; to use the class in a project you have to drop the "HandCursOpen", the "HandCursClosed" and a picture named "DefaultPICT" (can your pict as well, of course) and the PICTCanvas class itself to the project window.
The class does not do any memory checking. That may cause problems when the user drags very large pictures on the canvas. Feel free to add some file size checking etc.
Note: In order to make filedropping possible, you have to create a file type called "PICTs" in the file type dialogs. You may set it to ????/???? to allow any pictures being dropped.

Contact & Legal Stuff:

(c) Copyright1998 by Erich H. Rast

This class is freeware and may be changed and modified as long as I'm mentioned in the readme file.

Send bug reports and comments to:

h0444zkf@rz.hu-berlin.de 

