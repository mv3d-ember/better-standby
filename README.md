# Better Standby

A StandBy-style clock for your iPhone in landscape: big time, day of the week, date, and a photo slideshow behind it.

Tap the screen to show the ⚙️ gear (it hides after 5 seconds). The menu has:
- **Layout**: tap **Edit layout** to drag the time, day, date, calendar and battery anywhere, pinch (or use the slider) to resize, and change alignment, color or hide each one. Landscape and portrait each keep their own layout. You can also pick a font (Classic, Rounded, Fancy, Code, Tall, Pixel), clock thickness, Fill/Fit photos and photo darkness.
- **Brightness**: dims the screen more than iOS lets you
- **Color tint**: preset colors (Night red is easy on your eyes in the dark), a custom color picker, and a strength slider
- **Photo album**: upload photos, tap thumbnails to pick ones to remove, choose how often they change, shuffle, clear all
- 12/24-hour clock and accent color

A battery level display shows in the top-left on Android phones and computers. iPhone Safari doesn't let websites read the battery, so it hides itself there.

Photos and settings stay saved on your phone, inside the browser. Nothing gets uploaded anywhere. The page asks iOS for protected storage, remembers the last photo shown, and has **Backup / Restore** (one `.json` file you can save to the Files app).

**Important:** Safari tabs and the Home Screen app keep *separate* storage. Add the page to your Home Screen first, then add your photos from there.

## Google Calendar (tomorrow's events)

Open ⚙️ → **📅 Google Calendar** and follow the steps there. In short: tap **Copy script**, paste it into a new project at script.google.com, deploy it as a **Web app** (Execute as: Me, Who has access: Anyone), then paste the `/exec` URL into the page and tap **Connect**.

The script runs in your own Google account and only answers requests that include the secret key built into it. The page refreshes every 15 minutes and keeps the last events it got, so they still show if you're offline.
