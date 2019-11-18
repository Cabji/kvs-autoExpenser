<h1>AutoExpenser Dev Notes</h1>

<h2>Overview</h2>

This note will log anything I found out while I was working on the AutoExpenser project. The file is listed by date and topic.

<h2>20191118</h2>

<h3>Table Widget and Popup Menu problems</h3>

Seems like the tablewidget class isn't really designed for interacting with too much and is mostly designed to show data. My initial idea was to display data parse from a file in a tablewidget and then allow the user to opposite-click the table widget and select options from a popupmenu object.

The tablewidget class seems to not have much utility built into it to let the user interact with it. For example, there is no way to interact with the title or column headers once they are created. In fact, I couldn't find a way to utilise a popupmenu object at all with a tablewidget. The only part of a tablewidget that would work with the mousePressEvent (inherited from the widget class) is its very border, which is a single pixel wide black line on the UI.

Due to this limitation of the tablewidget class, I have had to abandon my UI design for using popupmenu.
