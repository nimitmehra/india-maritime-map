# The Indian Ocean World - A Maritime Perspective

An interactive south-up, India-centered world map showing maritime shipping routes, chokepoints, trade corridors, and foreign military presence across the Indo-Pacific.

**[View the live map](https://nimitmehra.github.io/india-maritime-map/)**

## Why this map exists

Every world map you have seen in a classroom or textbook shares three conventions: north is up, Greenwich (London) is at the centre, and the Mercator projection inflates northern landmasses. None of these are scientific choices. All are inherited from when European colonial powers dominated cartography.

For India, this creates a specific problem. Standard maps make India appear as a peninsular appendage dangling from the bottom of Asia. The visual emphasis falls entirely on land borders. The Indian Ocean, which India physically dominates, sits at the bottom of the frame where the eye never goes.

Most of India's trade, energy, and security flows through our oceans, not over our mountains. This map flips that perspective entirely.

The immediate trigger was the Hormuz crisis. On February 28, 2026, the US and Israel struck Iran. By March 2, Iran's IRGC declared the Strait of Hormuz closed. Tanker traffic dropped 90%. Crude spiked above $80. India gets 53% of its LNG through Hormuz, and nearly 80% of its energy imports transit the Indian Ocean. I was doing a cascade analysis of what a Hormuz closure means for India's crude, LNG, fertilizer, and treasury markets — and I wanted to find an interactive map that shows India at the centre of its own maritime trade. One that marks the chokepoints, the shipping lanes, and the routes that every barrel of oil takes to reach Indian ports. It didn't exist. So I built one.

The idea of flipping maps south-up is not new. It dates back to McArthur's Universal Corrective Map (1979) and was popularized in mainstream culture by The West Wing, Season 2 Episode 16 (2001), where the Organization of Cartographers for Social Equality pitches the Peters Projection and flips the map upside down in the White House — a scene that has stayed with me for years. The Equal Earth projection used here was created by Savric, Patterson, and Jenny in 2018. What is new is combining the south-up reorientation with interactive maritime trade data, per-port shipping routes, a strategic island chain overlay, and a foreign military presence layer — all built from India's perspective.

## What the map does

**South-Up Orientation**: The Southern Hemisphere is at the top. India's peninsula points upward into the Indian Ocean, which dominates the upper half of the map.

**India-Centered (82.5°E)**: India sits at the exact horizontal centre. Europe and Africa to the left, Southeast Asia and Australia to the right.

**Equal Earth Projection**: Countries shown at their true relative sizes. Africa appears 14x larger than Greenland as it actually is. No Mercator distortion.

**Official Indian Boundaries**: Borders follow the Republic of India's official position. J&K (including Gilgit-Baltistan and PoK), Ladakh (including Aksai Chin), and Arunachal Pradesh shown as integral Indian territory, using Datameet open boundary data overlaid on Natural Earth.

## What happens when you look at this map

When you look at this map, several things become immediately obvious that standard maps obscure:

1. **India controls the central Indian Ocean.** The peninsula projects directly into the busiest maritime trade corridor on Earth. This is not a peripheral position — it is the centre of global maritime trade.

2. **The Andaman and Nicobar Islands guard the Malacca Strait.** In standard maps, these islands are a footnote. In this view, they visibly sit at the mouth of one of the world's most critical chokepoints, through which 40% of global trade passes.

3. **India's energy security is a maritime question.** The sea lanes from the Persian Gulf run directly past India's western coast. Routes from East Asia pass through the Malacca Strait within reach of Indian naval assets. When Hormuz closes, India's vulnerability is immediate and existential.

4. **Every major trading nation's shipping route to India passes through chokepoints that India can influence.** This is not visible on standard maps.

5. **The foreign military presence overlay reveals the strategic competition.** China's string of ports from Gwadar to Hambantota to Djibouti encircles India. The US maintains a network from Japan to Diego Garcia to Bahrain. India's own overseas footprint — surveillance posts and port access agreements, not bases — is modest by comparison. The map makes this asymmetry visible at a glance.

You cannot build a maritime strategy while staring at maps that orient your thinking toward land borders.

## Interactive features

### Shipping Routes
Hover over any country to see its capital, major ports, and complete shipping routes to India. Each port has its own waypoint-by-waypoint sea route following actual maritime corridors. ~50 countries have complete per-port routes. For example:

- **Los Angeles** crosses the Pacific, through Lombok Strait and Malacca, to Chennai
- **New York** crosses the Atlantic, through Gibraltar, Med, Suez, Red Sea, to Mumbai
- **Vladivostok** goes through the Sea of Japan, South China Sea, Malacca, to Chennai
- **St. Petersburg** goes through the Baltic, English Channel, Atlantic, Gibraltar, Suez, to Mumbai
- **Santos (Brazil)** crosses the South Atlantic, around the Cape of Good Hope, up the East African coast, to Mumbai

13 static shipping corridors show the major global trade architecture through the Indian Ocean.

### Foreign Military Presence Toggle
Click "Show Foreign Bases" to reveal 36 installations across the Indo-Pacific, color-coded by country with shape-coded types (circles for military bases, diamonds for dual-use ports, triangles for intel/surveillance). Bases near the same location cluster into a ring of colored dots — hover to see all countries and their installations at that location.

- **US (silver)** — 15 installations: Yokosuka (7th Fleet HQ), Kadena, Camp Humphreys, Diego Garcia (joint US/UK), NSA Bahrain (5th Fleet HQ), Al Udeid, Camp Lemonnier, and others
- **China (red)** — 11 installations: PLA Djibouti (first overseas base), Gwadar (dual-use port, CPEC), Hambantota (99-year lease), Kyaukphyu (Myanmar), Ream (Cambodia, opened April 2025), Chittagong, Woody Island, Spratlys (3 artificial island bases), Port Sudan, Piraeus (COSCO 67%), Yulin submarine base
- **France (purple)** — Djibouti (largest French overseas base), Reunion Island
- **UK (orange)** — HMS Juffair (Bahrain), Duqm Joint Logistics (Oman)
- **India (saffron)** — 4 installations, none of which are military bases: Agalega (airstrip + surveillance, Mauritius), North Madagascar (listening post), Assumption Island (surveillance, Seychelles), Duqm (port access for logistics & maintenance, Oman)
- **Japan (pink)** — JMSDF Djibouti
- **Turkey (cyan)** — TURKSOM (Mogadishu)

### Strategic Island Chain
Five strategically significant island positions are labeled at small font sizes visible on zoom: Lakshadweep, Maldives, Diego Garcia, Mauritius, and St. Martin's Island (Bangladesh). Together with the Andaman and Nicobar Islands, these form the arc that defines India's maritime perimeter in the Indian Ocean.

### Light/Dark Mode
Toggle between dark mode (for presentations and sharing) and light mode (for print and reports). All elements — map, labels, shipping lanes, chokepoints, foreign bases — adjust colors for each mode.

### Maritime Elements
- 10 chokepoints: Strait of Hormuz, Bab-el-Mandeb, Strait of Malacca, Lombok Strait, Sunda Strait, Palk Strait, Mozambique Channel, Cape of Good Hope, Suez Canal
- 8 Indian cities including Port Blair and Srinagar
- 5 strategic international ports: Chabahar, Gwadar, Hambantota, Djibouti, Duqm
- Ocean and sea labels: Indian Ocean, Southern Ocean, Pacific Ocean, Atlantic, Arabian Sea, Bay of Bengal, South China Sea, Persian Gulf, Red Sea

## Technical details

- **Projection**: Equal Earth via D3.js — `d3.geoEqualEarth().rotate([-82.5, 0, 180]).center([0, -4])`
- **World data**: Natural Earth 50m via world-atlas TopoJSON
- **India boundary**: Datameet open data (Survey of India standard) overlaid on Natural Earth
- **Shipping routes**: ~50 countries with per-port waypoint routes (10-25 waypoints each)
- **Foreign bases**: 36 installations across 7 countries, verified against current sources as of March 2026
- **Rendering**: D3.js v7 + TopoJSON, entirely client-side
- **File**: Single self-contained HTML file (~95KB), no build step, no server

## Running locally

Download `index.html` and open in any browser. It fetches D3.js and map data from CDNs.

## License

Map code is open source. World geography data from Natural Earth (public domain). India boundary data from Datameet (open data). Equal Earth projection by Bojan Savric, Tom Patterson, and Bernhard Jenny. Foreign base locations compiled from publicly available sources including Wikipedia, CSIS, and government announcements.

## Author

**Nimit Mehra** — [nimitmehra.com](https://nimitmehra.com) — [@NimitMehra](https://twitter.com/NimitMehra)
