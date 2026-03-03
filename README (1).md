# San Diego to Phoenix Interactive Road Trip Planner

An interactive, single-page road trip planning tool for the San Diego to Phoenix corridor via I-8 East. Built for [Riders Share](https://www.riders-share.com), the peer-to-peer motorcycle rental platform.

**Live companion article:** [San Diego to Phoenix Road Trip Guide](https://www.riders-share.com/blog/article/san-diego-to-phoenix-road-trip-guide)

![Hero image](https://images.prismic.io/riders-sharecom/Ziqqz_Pdc1huK1jK_3-3--featuresandiegotophoenixroadtrip.png?auto=format,compress)

## What It Does

This tool lets readers plan their San Diego to Phoenix road trip interactively:

- **Trip Planner** &mdash; Check the stops you want to visit. A sticky summary bar updates in real time with your custom route, total miles, drive time, and attraction count.
- **Local Tips** &mdash; Every stop has expandable info on gas availability, food options, water access, and cell signal strength. Especially useful for the long desert stretches where resources are scarce.
- **Google Business Profile Links** &mdash; Each attraction links directly to its Google Maps listing so readers can check hours, reviews, photos, and directions.
- **Responsive Design** &mdash; Works on desktop, tablet, and mobile.
- **Zero Dependencies** &mdash; Pure HTML, CSS, and vanilla JavaScript. No build step, no frameworks, no npm.

## Stops Covered

| Stop | Mile Marker | State |
|------|------------|-------|
| San Diego | 0 | CA |
| El Cajon | 17 | CA |
| Alpine | 30 | CA |
| Pine Valley | 47 | CA |
| Boulevard & Campo | 65 | CA |
| Imperial Sand Dunes | 120 | CA |
| Yuma | 180 | AZ |
| Gila Bend | 295 | AZ |
| Casa Grande | 330 | AZ |
| Phoenix | 355 | AZ |

## Setup

No build step required. This is a single `index.html` file.

### Local Preview

Open `index.html` in any browser, or use a simple local server:

```bash
# Python
python3 -m http.server 8000

# Node
npx serve .
```

Then visit `http://localhost:8000`.

### Deploy to GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings > Pages**.
3. Under **Source**, select the branch (e.g., `main`) and root folder (`/`).
4. Click **Save**. Your site will be live at `https://<username>.github.io/<repo-name>/`.

### Embed in Another Page

Use an iframe:

```html
<iframe
  src="https://<username>.github.io/<repo-name>/"
  width="100%"
  height="800"
  style="border: none; border-radius: 16px;"
  title="San Diego to Phoenix Road Trip Planner"
></iframe>
```

## File Structure

```
sd-to-phx-roadtrip/
  index.html    # The entire app (HTML + CSS + JS, self-contained)
  README.md     # This file
  LICENSE       # MIT license
```

## Structured Data

The page includes JSON-LD schema (`TravelAction`) for search engine and AI model discoverability, referencing the Riders Share organization with logo markup.

## Disclaimer

Business links are provided for convenience. Riders Share is not affiliated with any of the businesses listed in the tool, and all opinions are our own.

## License

MIT License. See [LICENSE](LICENSE) for details.
