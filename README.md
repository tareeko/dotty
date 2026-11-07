# Dotty

Dotty is a Mac menu bar app for 32x32 iPixel LED screens. Put the screen on your desk facing the room, and it tells people whether to come over: In a meeting, Deep focus, Back soon, or one you've made yourself. The rest of the time it's a clock.

**[Download Dotty](https://github.com/tareeko/dotty/releases/latest/download/Dotty.dmg)** · **[Buy a license](https://dottyled.com/buy)**

## What it does

- Office statuses: Available, Deep focus, In a meeting, On a call, On air, Do not disturb, Quiet please, Back soon, At lunch, Praying, On a break, Away and Low social battery. Each can run for a set time or until you clear it.
- Your own statuses, made with a live preview: two lines, a colour and a real emoji drawn on the LEDs.
- Focus sessions with rounds and breaks. The whole session goes to the screen as one animation, so it keeps counting if your Mac sleeps or leaves the room.
- 25 clock faces, several with live weather from Open-Meteo. The clock goes to the screen as one looping animation, so it keeps going when your Mac sleeps or leaves the room: a whole day, or a week on faces that show the date. While your Mac is away, the weather stays as it was last sent.
- Your own GIFs, videos and pictures, converted to fit the screen.
- On a call, shown by itself while an app is using your microphone or camera (you can turn this off).
- A local HTTP API and a `dotty` command-line tool, so scripts, Shortcuts and build jobs can change the screen.

## What you need

- A Mac with macOS 14 or later, Apple silicon or Intel.
- A 32x32 LED screen made for the iPixel Color phone app. These are generic screens made in China and sold under many brand names, usually as a bare panel about 13 cm square on a suction-cup arm, with a USB cable. Look for the iPixel Color app in the listing, and the 32x32 size: 16x16 and 64x64 versions don't work yet, and look-alike frames that use the iDotMatrix or Divoom apps never will. [dottyled.com](https://dottyled.com/#screen) has a checklist and listings that match.
- Bluetooth. The screen takes one connection at a time, so close the iPixel Color app on your phone first.

## Price

Everything works free for 14 days. After that the clock keeps working, and statuses, focus sessions and media need a license: $15 once, for up to 3 of your Macs. The key arrives by email after you pay.

## Installing

1. Open `Dotty.dmg` and drag Dotty to Applications.
2. Open Dotty. It lives in the menu bar, and the first time it opens its window too.
3. Allow Bluetooth when macOS asks, then pick your screen under Settings, Screen.

Dotty keeps the screen's own playlist empty, so it shows only what you pick. That permanently deletes the demo animation a new screen comes with, and anything saved on it with the iPixel app. Only choose your own screen.

If other screens are in range, Blink turns a screen's display off and on so you can see which is which, and you can give each one a name. The nearest are listed first.

To activate a license, click Activate in the email on your Mac, or paste the key under Settings, License. To move a license to another Mac, use Remove from this Mac under Settings, License first. If that Mac is gone, Dotty lets you move the seat from the new one.

## What leaves your Mac

Pictures go to your screen over Bluetooth. For the weather, Dotty sends the place you type, and later its coordinates, to Open-Meteo. When you activate or check a license, it sends the key, your Mac's name and an ID made from a one-way hash of its hardware ID to the license server at led.tareknology.com. It contacts nothing else.

## Credits

Made by [Tarek Alward](https://tarekalward.com). The Bluetooth protocol is ported in part from [pypixelcolor](https://github.com/lucagoc/pypixelcolor) by Lucas Balmès, under the MIT licence; see [NOTICE.md](NOTICE.md).
