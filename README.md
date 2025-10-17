# KeepAwake
A lightweight single-file utility to prevent the computer from going idle, simulating user activity through cursor movements and optional keyboard presses.

Platform: Windows 10/11
Framework: WinUI 3 (.NET 8 recommended)

CORE FUNCTIONALITY:
	● ON/OFF toggle - start/stop the mouse jiggling process
	● Presence simulation toggle - start/stop the optional simulation of a key press
	● Launch on startup toggle - load the app automatically when Windows boots
	● Minimize to tray toggle - hides window in taskbar and shows tray icon
	● Settings overlay - configuration such as cursor distance, interval, and presence simulation key
	● Theme switcher button - switch between dark/light UI


UI/UX SPECIFICATIONS

Window Properties:
	Width: 266px
	Height: 385px
	Rounded corners: 30px radius
	Frameless (WindowStyle=None)
	Background: Dark theme #1e1e1e, Light theme #ffffff - Default theme when app starts for the first time is Dark. Create settings.ini file sitting next to the 

Header:
	Title: "Work, work..." (Bold 18px)
	Close button: Top-right, transforms to minimize icon when “Minimize to tray” is enabled
	Main section:
		● Toggle switches for ON/OFF, Presence simulation, Launch on startup, Minimize to tray
		● Divider between the ON/OFF and Presence simulation toggles
		● Divider between Presence simulation and Launch on startup toggles
	Settings overlay section:
		● Slightly transparent
		● 2 child sections:
			○ Cursor behavior:
				Distance input field (with description) in pixels
				Timer input field (with description) in seconds
			○ Presence behavior:
				Key input field (with description) to choose simulated key
	Footer:
		Settings button
		Theme switcher button

Animations:
	Settings overlay slides from left and scales up
	Smooth color transitions on theme toggle
	Buttom hover effects (blue highlight in both dark and light theme)
