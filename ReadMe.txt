==============================================================================
Installation
==============================================================================

If you have the .NET framework 4.0 then you can just start the application.
If not then install the .NET framework 4.0 from here:
http://www.microsoft.com/download/en/details.aspx?id=17851

You might wan't to go to Preferences > Baiscs (first tab) > Startup Delay
and adjust the value there to something appropriate for your system. The
value should match the minimum time needed to fully load and initialize the
G19 keyboard softawre "Logitech Gaming Software". By default it is set to
25 seconds (which is really safe).

Requirements:
- A working and fully operational G19 Logitech keyboard along with the
  "Logitech Gaming Software" (must be running).
- Works on Windows XP SP3, Windows 7 x86 & x64.


==============================================================================
About
==============================================================================

It is true that the Logitech G19 software comes with a RSS reader. But that
RSS reader has almost no customization (if any at all).
On top of that, Logitech's RSS reader's settings and RSS feeds are all lost
upon a fresh installation of Windows.

This application is highly customizable and puts everything, including all
of it's settings, in it's own application folder. So as long as you put this
application on another partition than the OS then nothing is lost when
Windows is re-installed or such.

Version 0.90 was created in 4 days.


==============================================================================
How To
==============================================================================

Add background:
- Add a new png, jpg, ,jpeg or gif image to the
 <application path>/Backgrounds/ folder
- Restart the application.

Scroll:
- Press the [Cancel] (the arrow pointing left next to the square stop button)
  to scroll the text up & down.

==============================================================================
Features & Limitations
==============================================================================

Features:
- Unlimited RSS feeds.
- Can display channel image/icon.
- Scrolling text
- Backgrounds can be customized both for all channels as well as for each
  individual channel.
- Fonts, text colors (foreground & background), transparent backdrops, etc.
  are all customizable (even for each individual channel if desired).
- RSS feeds can be sorted into groups. Then you can chose wich group to cycle
  or just all of them.
- Each channel can have it's own cycle-speed (how long each feed-item is
  displayed). If it doesn't the default speed is used.
- RSS feeds can be put into groups and then you may chose what groups to
  cycle on the LCD screen.
- LCD menu
- When opening an item, it can optionally be stored until you want to open all
  stored items. This comes in handy when running full-screen DirectX games
  for example and you don't want to lose focus but you don't want to forget
  to open and read the item either.
- Supports channel image/icon (the logo on the top-left of the screen).

Limitations:
- Supports only RSS 2.0
- Does not support HTML inside feeds. The HTML-items will be removed before
  displaying the feed.

==============================================================================
Version History
==============================================================================

Version 0.9.3 (November 25 2012)
  - Added the channel title to main menu
  - Fixed a mistake in the Group-Menu that caused the program to exit the
    menu when attempting to return to the main menu.
  - Added an extra menu option that allows users to clear all marked items
    for all channels.
  - Fixed a crash that occured when all items in the channel were marked as
    read and immediately after the user would navigate back to that channel.

Version 0.9.2 (November 17 2012)
  - First stable (no critical or any known bugs) release.
  - Now closes any previously started instances of this application (if any).
  - Fixed the "Parameter not valid..." crash. The previous version didn't
    seem to (fully) fix this. It seemed that the AABB was sometimes an
	empty rectangle (0,0,0,0).
  - Added the option to refresh the channels manually. Also fixed a bug
    in the Dispose-code that was called via that option.
  - Added a debug-mode for whenever the G19 keyboard is not detected.
  - Opening the error log when no error log was created will no longer
    crash the application.
  - The assembly version is now shown in the error log.
  - Expanded and fixed the preferences.
  - Scrolled items now have their scrolling-value reset when opened again.
  - The 'automatic-item-cycling' timer is now reset upon scrolling.
  - Improved the text-scrolling.
  - The startup has been delayed by 25 seconds to allow the G19 Software to
    fully initialize.
  - Plus more minor enhancements & bug fixes.

Version 0.9.1 (November 9 2012)
  - The application now actually registers itself to the Windows startup.
  - Fixed some spellings mistakes.
  - Fixed a memory leak.
  - Fixed a 'textrendering-measurement bug'.
  - Improved the error-logging and the system tray icon now changes when an
    error occured.
  - Fixed a crash that occured when Render() was called when another
    Render() call from another thread ("Parameter not valid..." crash).


Version 0.9.0 (November 5 2012)
  - First release.