# customRoutes

**Tight Not?** Can catch or not? A personal Singapore bus connection planner. One static page (`index.html`), no build step.

- Live arrivals from the free [arrivelah](https://github.com/cheeaun/arrivelah) API, called straight from the browser.
- Each route is planned forward from the next real buses: leave time, spare minutes at every transfer, backup bus, arrival time.
- When a bus has GPS, the same bus is matched at the alighting stop to get its live arrival; otherwise a distance-based ride estimate is used.
- Routes live in the `TABS` array at the top of the script. Walk, train and ride times can be adjusted on the phone under **Times** (saved in the browser).

Hosted with GitHub Pages from the `main` branch root.
