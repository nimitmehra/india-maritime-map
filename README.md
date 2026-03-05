# The Indian Ocean World - A Maritime Perspective

A south-up, India-centered world map that reframes how we view India's geography - from a land power at the bottom of Asia to a maritime power projecting into the Indian Ocean.

**[View the live map](https://nimitmehra.github.io/india-maritime-map/)**

## Why this map exists

Every world map you've seen in a classroom, a textbook, or on Google Maps shares three conventions: north is up, the Prime Meridian (Greenwich, UK) is at the centre, and the Mercator projection inflates northern landmasses. These aren't scientific choices - they're historical ones, established when European colonial powers dominated cartography.

For India, this creates a specific problem. Standard maps make India appear as a peninsular appendage dangling from the bottom of the Asian landmass. The visual emphasis falls on land borders - the Himalayas, Pakistan, China, Bangladesh. The Indian Ocean, which India physically dominates, is pushed to the bottom of the frame where the eye rarely goes.

This map flips that perspective entirely.

## What this map does differently

**South-Up Orientation**: The Southern Hemisphere is at the top. India's peninsula points upward into the Indian Ocean, which now dominates the upper half of the map. The visual effect is immediate - India stops looking like a vulnerable land endpoint and starts looking like what it is: a massive maritime power with the Arabian Sea and Bay of Bengal as its strategic frontyard.

**India-Centered (82.5 deg E)**: The map is centered on India's standard meridian. India sits at the exact horizontal centre. Europe and Africa are to the left; Southeast Asia, Australia, and the Pacific to the right. The Americas are split at the edges - the same thing that happens to Asia on Greenwich-centered maps.

**Equal Earth Projection**: Unlike Mercator, this projection shows countries at their true relative sizes. Africa appears 14x larger than Greenland (as it actually is). India appears correctly larger than all of Western Europe combined.

**Official Indian Boundaries**: India's borders follow the Republic of India's official position. The entire former princely state of Jammu & Kashmir (including Gilgit-Baltistan and PoK), Ladakh (including Aksai Chin), and Arunachal Pradesh are shown as Indian territory. India boundary data sourced from [Datameet](https://github.com/datameet/maps) open data project (Survey of India standard).

## Maritime elements

The map highlights India's maritime geography:

- **10 maritime chokepoints** marked and labeled: Strait of Hormuz, Bab-el-Mandeb, Strait of Malacca, Lombok Strait, Sunda Strait, Palk Strait, Mozambique Channel, Cape of Good Hope, Suez Canal
- **Major sea lanes** shown as dashed routes through the Indian Ocean
- **Indian ports**: Mumbai, Chennai, Kolkata, Kochi, Visakhapatnam, Port Blair (Andaman & Nicobar)
- **Strategic international ports**: Chabahar (Iran), Gwadar (Pakistan), Hambantota (Sri Lanka), Djibouti, Duqm (Oman)
- **Island territories**: Andaman & Nicobar Islands and Lakshadweep labeled
- **Ocean labels**: "INDIAN OCEAN" is the most prominent text on the map

## Technical details

- **Projection**: Equal Earth (pseudocylindrical, equal-area) via D3.js
- **Rotation**: `d3.geoEqualEarth().rotate([-82.5, 0, 180])` - centered on 82.5 deg E with 180 deg gamma for south-up
- **World data**: Natural Earth 50m resolution via [world-atlas](https://github.com/topojson/world-atlas) TopoJSON
- **India boundary**: [Datameet India composite GeoJSON](https://github.com/datameet/maps) - rendered as overlay on top of Natural Earth for correct official boundaries
- **Rendering**: D3.js v7 + TopoJSON client, entirely client-side
- **File**: Single self-contained HTML file, ~42KB, no build step required

## How the projection works

The key line of code is:

```javascript
d3.geoEqualEarth()
  .rotate([-82.5, 0, 180])  // center on India, flip south-up
  .center([0, -4])           // shift 4 deg south to show more Indian Ocean
```

The three rotation parameters are `[lambda, phi, gamma]`:
- `lambda = -82.5`: centers the map on 82.5 deg E longitude (IST meridian, bisects India)
- `phi = 0`: no north-south tilt
- `gamma = 180`: rotates the entire map 180 degrees, putting south at the top

## The argument for reorientation

When you look at this map, several things become immediately obvious that standard maps obscure:

1. **India controls the central Indian Ocean.** The peninsula projects directly into the busiest maritime trade corridor on Earth.

2. **The Andaman & Nicobar Islands sit at the mouth of the Malacca Strait.** In standard maps, these islands are a footnote. In this view, they're visibly positioned at one of the world's most critical chokepoints.

3. **India's energy security is a maritime question.** The sea lanes from the Persian Gulf (Strait of Hormuz) run directly past India's western coast. The routes from Southeast Asia and East Asia pass through the Malacca Strait, within reach of Indian naval assets.

4. **The "land border" framing is incomplete.** Standard maps make India's relationship with China and Pakistan appear primarily as a land border question (Kashmir, Ladakh, Arunachal). This map doesn't diminish those realities, but it adds the maritime dimension that land-focused maps erase.

## Running locally

Download `index.html` and open it in any modern browser. No server required - it fetches D3.js and map data from CDNs. Works offline once the initial ~2MB of TopoJSON data is cached.

## License

The map code is open source. World geography data is from [Natural Earth](https://www.naturalearthdata.com/) (public domain). India boundary data is from [Datameet](https://github.com/datameet/maps) (open data). The Equal Earth projection was created by Bojan Savric, Tom Patterson, and Bernhard Jenny.

## Author

**Nimit Mehra** - [nimitmehra.com](https://nimitmehra.com) - [@NimitMehra](https://twitter.com/NimitMehra)
