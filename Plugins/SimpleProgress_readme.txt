SimpleProgressCanvas 1.0

An RB custom class with superclass canvas that displays a simple progress bar. There have been reported some problems with the MacOS progress bar so this class may be used as a simple replacement. It cannot display the "barber pole" and does no boundary checking at all.

New Events:

Completed

the sprogress.value is >= sprogress.maximum 

Methods:

Draw()

force drawing of the progress bar. You must call this method when the canvas has been resized. It is also useful if you want to draw a string when there's no change in the progress because the DrawText method does only draw the string when the value has been changed.

GetPercent() as Integer

Return the percentage of progress so far.

Update(value as Integer)

Set the new value; causes the progress bar to be updated.

Properties:

maximum as Integer

The maximum value, default is 100.

value as Integer

The current value of the progress bar.

frame_width as Integer

The width of the inner frame of the progress bar, default is 1.

Back_Color as Color

The background color (where no progress is shown).

Fill_Color as Color

The color the progress is shown with.

Text_Color as Color

The color of the text displayed on the progress bar.

Text_Font as String

The font of the text displayed in the progress bar, default is Monaco.

Text_Size as Integer

The size of the font to displays text, default is 9.

BottomRight_Color as Color

The color of the bottom-right inner frame.

TopLeft_Color as Color

The color of the top-left portion of the inner frame.

TextAlign as Integer

0=left (default), 1 = center, 2 = right

bold as Boolean

Draw the text with bold style applied.

underline as Boolean

Draw the text underlined.

Contact & Legal Stuff:

(c) Copyright1998 by Erich H. Rast

This class is freeware and may be changed and modified as long as I'm mentioned in the readme file. Feel free to play around with the code and enhance the graphics but please make your new class publicly available that everyone can benefit from it.

Send bug reports and comments to:

h0444zkf@rz.hu-berlin.de 

