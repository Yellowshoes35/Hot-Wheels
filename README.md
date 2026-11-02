# Hot Wheels Garage

A browser-based garage and race-timing dashboard for tracking Hot Wheels cars, registering racers, and recording portal passes.

## Features

- **Portal connection:** Connect to the Hot Wheels timing portal from the app and view its connection status.
- **Car detection:** Scan cars by rolling them through the connected portal. Cars without a readable/printed ID are grouped as **Other**.
- **Racer registration:** Create a racer with or without a car. A racer must have a car assigned before racing.
- **Car assignments:** Assign available cars to racers; each car can be assigned to only one racer at a time.
- **Leaderboard:** View recorded car speeds and race results.
- **Speed display:** Optionally show scale speed in mph (×64) and adjust the speed calibration factor.
- **Photos and voice:** Add or change a car photo and use the voice announcer.
- **Garage controls:** Refresh the car list, scan a new car, and clear the recorded car list.
- **Technical log:** View or copy diagnostic messages when troubleshooting.

## Getting started

1. Open the deployed site over **HTTPS** (or use a supported localhost development setup).
2. Use **Chrome on Android** for the portal connection.
3. Turn on and prepare the Hot Wheels portal.
4. Open the app and tap **Connect to portal**.
5. Approve the browser's Bluetooth permission request if prompted.
6. Roll a car through the portal to detect it and add it to the garage.
7. Register racers and assign cars. Racers without an assigned car can be registered, but cannot race until a car is assigned.

> Keep the phone or tablet near the portal while connected. If the portal disconnects, reconnect from the app.

## Repository contents

- `index.html` — the complete Hot Wheels Garage app. The interface, styles, and application code are contained in this single file.

## Notes

- The app uses browser storage to retain garage information on the device/browser where it is used. Clearing browser site data may remove locally stored information.
- Bluetooth availability and permissions depend on the browser, device, and operating system.
- This project is intended for use with compatible Hot Wheels portal hardware.

## Development

This is a standalone HTML app. To work on it, edit `index.html` and commit the changes to this repository. No separate build step is required for the current single-file version.
