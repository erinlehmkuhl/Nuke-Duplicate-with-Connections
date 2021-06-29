# Nuke-Duplicate-with-Connections
Duplicate any node and keep the input node graph connections intact


add this to your menu.py and use it as a hotkey or a menu button

1. if the code is in your menu.py just make sure it is above the line where you insert it into your menu.
cmpdeptmenu.addCommand( 'Commands/Duplicate with Connections', dup_with_connections.main, 'shift+d' )

2. if you put the code in a nukescripts folder (in your nuke path -- probably add that path to your init.py)
then don't forget to import it before you add it to your menu:
init/py >> 
nuke.pluginAddPath( '/servers/RHS/SHOWS/dad/comp_tools/dw_gizmos/nukescripts' )

menu.py >>
import dup_with_connections
cmpdeptmenu.addCommand( 'Commands/Duplicate with Connections', dup_with_connections.main, 'shift+d' )
