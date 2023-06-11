The big and ugly URLEditfield for RB 1 and 2 
Version 1.0

You always wanted it, now you get it! This Editfield class does display colored
URLs and can determine which link you have double-clicked. However, it's a real
nasty, inefficient hack. But to finally ruin my reputation, I have decided to
give it away. :-)

New Events

NewWord ( start as Integer )

A new word starting at start has been added to the field.


URLSelected( url as String )

An URL has been selected. Use the ShowURL method to launch it.

Methods

DefineTags( tags as String )

Takes a comma seperated list of tags to parse for. Default is
"http:,ftp:,gopher:,https:,mailto:,telnet:,wais:"

HighlightLinks

Causes the field to be parsed for URLs and colors them. Unfortunately, coloring
causes much flicker when the editfield has a scrollbar.

Properties    these properties are not available in the lite version!


linkColor as Color

The color the URLs will appear with.


normalColor as Color

The default color for non-link text.


This class is provided "as is" and is open source and free for anyone. Note: If
you run into problems with unwanted URLSelected events when adding text using
selText = "yourstring", contact me (eh, I have corrected this but lost my
changes...)

Erich Rast ( h0444zkf@rz.hu-berlin.de )


