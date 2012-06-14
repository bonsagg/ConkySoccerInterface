ConkySoccerInterface
===================

What to do
----------
Place csi.py in this folder: ~/.conky 
You might need to create this folder first.

Dependencies
-----------
 * python-suds or python2-suds (depending on your distribution)

How to configure conky
----------------------
 * Edit ~/.conkyrc
 * Add some lines like these:
````${font size=11:italic}${color slate grey}Fußball EM 2012 ${hr}${color }${font }````
````${execi 60 python ~/.conky/csi.py}````
 * If you use a distribution with Python3 as default, you need to replace 'python' with 'python2' in the command above
 * Notice: This way conky will call the script every 60 seconds

Known issues
------------
 * Sometimes conky will not show any results after running the script. Just wait for the next update in case.
 * Depending on your conky-configuration some letters might be truncated
