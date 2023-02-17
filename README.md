# AppleRemote
AppleRemote configuration file

Abstract: the AppleRemote application allows to use the Apple Remote with application or system (Apple CPU) not supporting natively the Apple Remote.
The AppleRemote application generates keystrokes from the Apple Remote keys.

Keys generation depends on the topmost application. Keys are defined in 'Configuration.plist' located in "/Applications/AppleRemote.app/Contents/Resources":

"com.apple.Music" is the bundle identifier.

"Key 124" to define virtual key code.

"Modifier 1048576" to define key modifiers (here 0x00100000 = ⌘).

If the front application bundle identifier is not found in 'Configuration.plist', the 'default' behavior is:
- Up = up arrow or general volume +
- Down = down arrow or general volume -
- Left = left arrow
- Right = right arrow
- Center = Enter or 'N' in YouTube mode
- Play = Space
- Menu = Escape or 'P' in Youtube mode
