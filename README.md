# customRoutes

**Tight Not?** Can catch or not? A personal Singapore bus connection planner. One static page (`index.html`), no build step.

- Live arrivals from the free [arrivelah](https://github.com/cheeaun/arrivelah) API, called straight from the browser.
- Each route is planned forward from the next real buses: leave time, spare minutes at every transfer, backup bus, arrival time.
- When a bus has GPS, the same bus is matched at the alighting stop to get its live arrival; otherwise a distance-based ride estimate is used.
- Routes live in the `TABS` array at the top of the script. Walk, train and ride times can be adjusted on the phone under **Times** (saved in the browser).

Hosted with GitHub Pages from the `main` branch root.

## Trip mode

Tap **Go** on any plan to follow that trip. The app then:
- keeps a progress bar (walk → wait → bus → … → arrive) that moves on taps ("I'm at the stop", "I'm on the 298", "I got off") or on its own when the expected time has passed, with a "Not yet" undo;
- tracks your actual bus by its arrival time and GPS, and updates your drop-off time and the spare time for the next bus;
- flashes an alert (and vibrates) when a connection is missed or very tight. If another route in the same tab boards at that stop and arrives sooner, it offers a one-tap switch; otherwise it shows the next bus on your route.

"Already walking?" options list buses that come sooner than your walk time, for when you have already left. The trip is saved on the phone, so it survives refreshes and closing the app.
