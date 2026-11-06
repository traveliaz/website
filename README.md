# Traveliaz website

**The world is yours.** Hostels, hotels, flights, car rentals and local tours for solo travelers, starting with Egypt (Cairo, Luxor, Aswan, Hurghada, Sharm El Sheikh, Alexandria).

Website design and branding by [EGO Web Services LLC](https://egowebservices.com).

## Structure

| Path | What it is |
|---|---|
| `index.html` | The full site: one self-contained page (HTML, CSS and JS inline) |
| `assets/brand/` | Logo kit: horizontal, stacked, white and classic lockups, icon, app icon, favicons |
| `favicon.png` | 32px browser icon |

No build step. Open `index.html` in a browser, or serve the folder with any static host.

## Adding real photos

Every photo spot shows an illustrated stand-in labelled with the shot it needs. Add your images to `assets/photos/` and fill in the `PHOTOS` list near the top of the script in `index.html`:

```js
const PHOTOS = {hero:"assets/photos/hero-giza.jpg", cairo:"assets/photos/cairo.jpg", ...};
```

Keys: `hero, cairo, luxor, aswan, hurghada, sharm, alexandria, flights, cars, b2b`. Use landscape photos, at least 2400px wide for `hero` and 1200px for the rest.

## Still to connect

- Booking.com, Expedia, Hostelworld and Agoda affiliate feeds for live rates and booking links (listings and prices are samples)
- Flight and car-rental partners for the package and car search
- A form backend for the business quote form
- A live USD/EGP exchange rate (currently a fixed sample rate)

## Deploying

Works as-is on GitHub Pages (Settings → Pages → Deploy from branch `main`, folder `/`), Vercel or Netlify.
