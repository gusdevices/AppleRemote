# AppleRemote
AppleRemote configuration file

Abstract: the AppleRemote application allows to use the Apple Remote with application or system (Apple CPU) not supporting natively the Apple Remote.
The AppleRemote application generates keystrokes from the Apple Remote keys.

Keys generation depends on the topmost application. Keys are defined in 'Configuration.plist':

"com.apple.Music" is the bundle identifier.

Key</key> <integer>124</integer>' to define virtual key code.

'<key>Modifier</key> <integer>1048576</integer>' to define key modifiers (here 0x00100000 = ⌘).

If the front application bundle identifier is not found in 'Configuration.plist', the 'default' behavior is:
- Up = up arrow or general volume +
- Down = down arrow or general volume -
- Left = left arrow
- Right = right arrow
- Center = Enter or 'N' in YouTube mode
- Play = Space
- Menu = Escape or 'P' in Youtube mode
