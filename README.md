# The Indian Ocean World - A Maritime Perspective

A south-up, India-centered interactive world map that reframes India's geography from a land power at the bottom of Asia to a maritime power projecting into the Indian Ocean.

**[View the live map](https://nimitmehra.github.io/india-maritime-map/)**

## Why this map exists

Every world map you have seen in a classroom or textbook shares three conventions: north is up, Greenwich (London) is at the centre, and the Mercator projection inflates northern landmasses. None of these are scientific choices. All are inherited from when European colonial powers dominated cartography.

For India, this creates a specific problem. Standard maps make India appear as a peninsular appendage dangling from the bottom of Asia. The visual emphasis falls entirely on land borders. The Indian Ocean, which India physically dominates, sits at the bottom of the frame where the eye never goes.

Most of India's trade, energy, and security flows through our oceans, not over our mountains. This map flips that perspective entirely.

## What the map does

**South-Up Orientation**: The Southern Hemisphere is at the top. India's peninsula points upward into the Indian Ocean, which dominates the upper half of the map.

**India-Centered (82.5 deg E)**: India sits at the exact horizontal centre. Europe and Africa to the left, Southeast Asia and Australia to the right.

**Equal Earth Projection**: Countries shown at their true relative sizes. Africa appears 14x larger than Greenland as it actually is.

**Official Indian Boundaries**: Borders follow the Republic of India's official position. J&K (including Gilgit-Baltistan and PoK), Ladakh (including Aksai Chin), and Arunachal Pradesh shown as integral Indian territory.

## Interactive features

**Hover over any country** to see:
- Country name and capital city (with map marker)
- Major commercial port cities (with map markers)
- Complete shipping routes from each port to India

**Per-port shipping routes**: Each port has its own waypoint-by-waypoint sea route following actual maritime corridors. For example, hovering over the United States shows three distinct routes:
- Los Angeles goes across the Pacific, through the Lombok Strait, Strait of Malacca, to Chennai
- New York goes across the Atlantic, through Gibraltar, the Mediterranean, Suez Canal, Red Sea, to Mumbai
- Houston goes through the Gulf of Mexico, across the Atlantic, through Suez, to Mumbai

Hovering over Russia shows:
- St. Petersburg goes through the Baltic, English Channel, Atlantic, Gibraltar, Suez, to Mumbai
- Vladivostok goes through the Sea of Japan, South China Sea, Malacca, to Chennai
- Novorossiysk goes through the Black Sea, Mediterranean, Suez, to Mumbai

**13 static shipping corridors** visible on the map showing major global trade routes through the Indian Ocean, including the Hormuz-Malacca central axis, Suez-Bab-el-Mandeb route, Cape of Good Hope route, and connections to Europe, East Asia, Africa, and the Americas.

**10 maritime chokepoints** marked: Strait of Hormuz, Bab-el-Mandeb, Strait of Malacca, Lombok Strait, Sunda Strait, Palk Strait, Mozambique Channel, Cape of Good Hope, Suez Canal.

**Indian ports and cities**: New Delhi, Mumbai, Chennai, Kolkata, Kochi, Visakhapatnam, Port Blair, Srinagar. Island territories: Andaman and Nicobar Islands, Lakshadweep.

**Strategic international ports**: Chabahar, Gwadar, Hambantota, Djibouti, Duqm.

## The argument for reorientation

When you look at this map, several things become immediately obvious that standard maps obscure:

1. India controls the central Indian Ocean. The peninsula projects directly into the busiest maritime trade corridor on Earth.

2. The Andaman and Nicobar Islands sit at the mouth of the Malacca Strait. In standard maps, these islands are a footnote. In this view, they visibly guard one of the world's most critical chokepoints.

3. India's energy security is a maritime question. The sea lanes from the Persian Gulf run directly past India's western coast. Routes from East Asia pass through the Malacca Strait within reach of Indian naval assets.

4. Every major trading nation's shipping route to India passes through chokepoints that India can influence. This is not visible on standard maps.

You cannot build a maritime strategy while staring at maps that orient your thinking toward land borders.

## Technical details

- **Projection**: Equal Earth via D3.js with `d3.geoEqualEarth().rotate([-82.5, 0, 180]).center([0, -4])`
- **World data**: Natural Earth 50m via world-atlas TopoJSON
- **India boundary**: Datameet open data (Survey of India standard) overlaid on Natural Earth
- **Shipping routes**: ~50 countries with per-port waypoint routes (10-25 waypoints each following actual sea lanes)
- **Rendering**: D3.js v7 + TopoJSON, entirely client-side, single HTML file
- **File size**: ~75KB, no build step, no server required

## Running locally

Download `index.html` and open in any browser. It fetches D3.js and map data from CDNs.

## License

Map code is open source. World geography data from Natural Earth (public domain). India boundary data from Datameet (open data). Equal Earth projection by Bojan Savric, Tom Patterson, and Bernhard Jenny.

## Author

**Nimit Mehra** - [nimitmehra.com](https://nimitmehra.com) - [@NimitMehra](https://twitter.com/NimitMehra)
