# The Indian Ocean World — A Maritime Perspective

An interactive south-up, India-centered world map showing maritime shipping routes, chokepoints, trade corridors, and military presence across the Indo-Pacific.

**[→ Open the live map](https://nimitmehra.github.io/india-maritime-map/)**

---

## Why this map exists

Standard world maps — Mercator projection, north-up, centred on the Atlantic — were designed for European colonial navigation. They distort the size of landmasses (Greenland appears the size of Africa when it is one-fourteenth as large), push the Indian Ocean to the margins, and make India look like a small peninsula hanging off the bottom of Asia.

This matters because **orientation shapes strategy**. If you look at a conventional map, India appears to be a land power wedged between China and Pakistan. Its coastline looks incidental. Its islands look like footnotes. The Indian Ocean looks like empty blue space between the continents that actually matter.

None of that is true.

**The Hormuz trigger.** On February 28, 2026, the US and Israel struck Iran (Operation Epic Fury). By March 2, Iran's IRGC declared the Strait of Hormuz closed. Tanker traffic dropped 90%. Crude spiked above $80 by March 4. India imports 53% of its LNG through Hormuz and over 80% of its crude by sea. There was no interactive map that showed India at the centre of its own maritime trade — chokepoints, shipping lanes, energy routes, strategic military presence. So we built one.

**Intellectual lineage.** The idea of flipping the map is not new. McArthur's Universal Corrective Map (1979) was the first widely known south-up map. *The West Wing* Season 2, Episode 16 (aired February 28, 2001) — the Organization of Cartographers for Social Equality pitches the Peters Projection and flips the map; that scene stayed with me for years. The Equal Earth projection by Šavrič, Patterson, and Jenny (2018) is what we use — it preserves true relative area without the visual distortions of Peters.

---

## What the map does

- **South-up orientation** with 180° rotation: India's peninsula points upward into the Indian Ocean. The ocean dominates the upper half of the map.
- **India-centered** at 82.5°E: India sits at exact horizontal centre. Europe and Africa to the left, Southeast Asia and Australia to the right.
- **Equal Earth projection**: Countries shown at true relative sizes. Africa appears 14× larger than Greenland, as it actually is.
- **Official Indian boundaries**: India shown with Jammu & Kashmir (including Gilgit-Baltistan and PoK), Ladakh (including Aksai Chin), and Arunachal Pradesh as integral Indian territory, using Datameet boundary data conforming to the Survey of India.

---

## What happens when you look at this map

1. **India controls the central position in the Indian Ocean.** It is not a peripheral land power — it is the geographic centre of the ocean that carries 80% of global seaborne oil trade and one-third of all bulk cargo.

2. **The Andaman & Nicobar Islands visibly guard the Strait of Malacca.** On a conventional map, they are invisible dots. On this map, they sit right above the entrance to the world's busiest shipping lane.

3. **Energy security is maritime security.** The sea lanes from the Persian Gulf run directly past India's western coast. The lanes from Southeast Asia pass through waters India's eastern naval command controls. India is not a bystander to its own energy supply — it is positioned across it.

4. **Every major chokepoint is within operational reach.** Hormuz, Bab-el-Mandeb, Malacca, Lombok, Sunda, Palk Strait — all visible, all within range of Indian naval assets based at Mumbai, Karwar, Visakhapatnam, Kochi, and Port Blair.

5. **The military picture is visible.** Fourteen powers operate 88 installations across the Indo-Pacific. The map shows domestic fleet headquarters, forward-deployed bases, overseas ports, surveillance outposts, and installations under negotiation — with clear status markers distinguishing what is operational from what is aspirational.

You cannot build a maritime strategy while staring at maps that orient your thinking toward land borders.

---

## Interactive features

### Shipping routes
Hover over any country to see animated shipping routes showing how trade reaches India. Per-port waypoint routes for ~50 countries follow actual sea lanes — US cargo from New York via Gibraltar and Suez to Mumbai, Chinese exports from Shanghai through the South China Sea and Malacca to Chennai, Australian bulk via Lombok and the Arafura Sea.

### Military bases (88 installations, 14 powers)
Toggle **"Show Military Bases"** to reveal the complete military picture. When active, non-essential map elements (Indian city markers, strategic port labels) are hidden for clarity — only chokepoints, country names, and base markers remain. All detail is accessible via hover tooltips.

**Three-tier status system:**
- **Solid markers** — Operational (68 installations)
- **Dashed-ring markers** — Agreed / Under negotiation (7 installations)
- **Faint dashed markers** — Unconfirmed / Speculative (2 installations)

**Shape coding:**
- ● Circle = Military base
- ◆ Diamond = Dual-use port
- ▲ Triangle = Intel / Surveillance

#### Which countries have domestic (home) bases on the map — and why

The map shows **domestic fleet headquarters and home bases** for countries whose navy is physically based on the Indian Ocean, its connected seas (Persian Gulf, Red Sea, South China Sea), or whose home fleet must transit a chokepoint visible on this map to reach the Indian Ocean. The filter is: **can this country's warships sail directly into the Indian Ocean from their home port, or must they cross a chokepoint we are tracking?**

| Power | Domestic bases shown? | Reason |
|-------|----------------------|--------|
| **India** | ✅ 6 bases | It is India's ocean. Three naval command HQs (Mumbai, Visakhapatnam, Kochi), Andaman & Nicobar Command (Port Blair), INS Kadamba Karwar, INS Rajali Arakkonam. |
| **Pakistan** | ✅ 4 bases | Directly on the Arabian Sea. Karachi (Naval HQ), Ormara/Jinnah (submarine base built to survive Indian blockade), Turbat (P-3C air station), Gwadar. Primary naval adversary. |
| **Iran** | ✅ 4 bases | Controls the Strait of Hormuz — the trigger for this entire map. Bandar Abbas (Naval HQ), Jask (Indian Ocean projection), Abu Musa Island, Chabahar (IRGC). |
| **China** | ✅ 4 bases | PLAN fleet commands deploy through the South China Sea into the Indian Ocean. Zhanjiang (South Sea Fleet — all Indian Ocean deployments originate here), Ningbo (East Sea Fleet — faces Taiwan Strait), Qingdao (North Sea Fleet — carrier home port), Yulin (submarine base, Hainan). |
| **UAE** | ✅ 1 base | Home fleet is physically in the Persian Gulf. Abu Dhabi Naval Base (Mina Zayed + Fujairah). |
| **Saudi Arabia** | ✅ 1 base | King Faisal Naval Base (Jeddah) — Western Fleet patrols the Red Sea, which is India's Suez route. |
| **Turkey** | ✅ 3 bases | Gölcük (Naval Forces Command HQ), Aksaz (Mediterranean Fleet), Mersin (Eastern Med, closest to Suez). Turkey deployed naval assets to Pakistan's aid during the 1971 war and maintains an adversarial posture toward India. Turkish fleet must transit Suez to reach the Indian Ocean — a chokepoint this map tracks. |
| **United States** | ❌ | The US does not fight in the Indian Ocean from Norfolk or San Diego. It fights from the 5th Fleet (Bahrain), 7th Fleet (Yokosuka), Diego Garcia, Guam. All 18 forward-deployed positions are on the map. Home ports across the Pacific and Atlantic are irrelevant to this ocean. |
| **France** | ❌ | France already has 4 bases inside the Indian Ocean (Djibouti, Abu Dhabi, Reunion, Mayotte). If France fights here, it fights from within the ocean. Toulon (Mediterranean home port) adds no strategic insight. |
| **United Kingdom** | ❌ | Fights from Bahrain and Duqm. Both are on the map. Portsmouth is the other side of the world. |
| **Japan** | ❌ | Anti-piracy contributions staged from JMSDF Djibouti (on map). Home bases in the Sea of Japan are irrelevant to the Indian Ocean. |
| **Russia** | ❌ | Has no operational forward base in the Indian Ocean yet. Port Sudan and Massawa (both agreed/negotiating) are on the map. Vladivostok and Severomorsk are across other oceans. |
| **Israel** | ❌ | Projects into the region through intel and partnerships, not fleet deployments. Haifa (Mediterranean) and Eilat (tiny Red Sea port) would add no insight. Three forward positions (Eritrea intel, Somaliland) are on the map. |
| **Italy** | ❌ | Anti-piracy base in Djibouti (on map). Home fleet in the Mediterranean is not relevant. |

#### Full breakdown: 14 powers, 88 installations

| Power | Count | Key positions |
|-------|-------|---------------|
| **United States** | 25 | 5th Fleet (Bahrain), 7th Fleet (Yokosuka), Yokota (USFJ HQ), Misawa, Iwakuni (F-35B), Kadena (Okinawa), Sasebo, Osan & Kunsan (S. Korea), Guam (Second Island Chain), Philippines EDCA (First Island Chain), Diego Garcia, Camp Lemonnier (Djibouti), Al Udeid (Qatar), Al Dhafra (UAE), Prince Sultan AB (Saudi Arabia), Muwaffaq Salti (Jordan), Pine Gap, Waihopai (NZ Five Eyes), HMAS Stirling (AUKUS, agreed) |
| **China** | 14 | 3 fleet HQs (Zhanjiang, Ningbo, Qingdao), Yulin sub base, Gwadar, Hambantota, Djibouti, Ream, Kyaukphyu, Chittagong, Woody Is. & Spratlys (SCS), Port Sudan, Piraeus |
| **India** | 10 | 3 Naval Commands (Mumbai, Visakhapatnam, Kochi), A&N Command (Port Blair), INS Kadamba Karwar, INS Rajali Arakkonam, Agalega, N. Madagascar, Assumption Is., Duqm |
| **UAE** | 6 | Abu Dhabi Naval Base, Berbera, Mayun/Perim Is., Assab, Socotra, Bosaso |
| **France** | 4 | Djibouti, Camp de la Paix Abu Dhabi, Reunion, Mayotte |
| **Pakistan** | 4 | Karachi, Ormara/Jinnah, Turbat, Gwadar |
| **Iran** | 4 | Bandar Abbas, Jask, Abu Musa Is., Chabahar |
| **Israel** | 3 | Dahlak Is. (unconfirmed), Amba Soira (unconfirmed), Somaliland (agreed) |
| **United Kingdom** | 3 | HMS Juffair (Bahrain), Duqm (Oman), BATUK (Kenya) |
| **Turkey** | 4 | Gölcük (Naval Forces Command HQ), Aksaz (Mediterranean Fleet), Mersin (Eastern Med, closest to Suez), TURKSOM (Somalia) |
| **Russia** | 4 | Severomorsk (Northern Fleet HQ), Vladivostok (Pacific Fleet HQ), Port Sudan (agreed, frozen), Massawa (agreed) |
| **Saudi Arabia** | 2 | King Faisal Naval Base (Jeddah, Red Sea fleet), Djibouti (agreed) |
| **Japan** | 3 | JMSDF Yokosuka (Fleet HQ), JMSDF Kure (submarines/carriers), JMSDF Djibouti |
| **Italy** | 1 | Base Amedeo Guillet (Djibouti) |

Each base marker shows its country's unique color. Hover over any marker for full details: location name, host country, operating country, facility type, operational status, and description.

**Cluster rendering:** Where multiple countries share a location (e.g. Djibouti with 6 presences, Abu Dhabi with US + France + UAE, Gwadar with China + Pakistan), bases render as a ring of colored dots. Hover shows all presences.

### Strategic island chain & chokepoints
10 maritime chokepoints marked with ring + dot + label: Strait of Hormuz, Bab-el-Mandeb, Strait of Malacca, Lombok Strait, Sunda Strait, Palk Strait, Mozambique Channel, Cape of Good Hope, Suez Canal.

Indian strategic islands (Lakshadweep, Andaman & Nicobar), Maldives, Mauritius, Diego Garcia, and St. Martin's Island are labelled.

### Sea lanes
13 shipping corridors — 5 main (thicker) and 8 secondary (thinner) — shown as gold/amber dashed lines tracing actual maritime trade routes.

### Light / Dark mode
Toggle between dark mode (default, ocean-forward) and light mode.

---

## Technical details

- **Single self-contained HTML file** (~108 KB). No build step, no server, no dependencies beyond CDN-loaded D3.js v7 and TopoJSON.
- **Projection**: `d3.geoEqualEarth().rotate([-82.5, 0, 180]).center([0, -4])`
- **World data**: Natural Earth 50m via `world-atlas@2` TopoJSON (CDN with fallback)
- **India boundary**: Datameet composite GeoJSON (~21 KB simplified), clockwise winding, overlaid on top of Natural Earth India
- **Rendering**: 13 SVG layers from ocean gradient to hover interaction
- **Military bases layer**: 88 entries with per-entry status codes (`op`/`ag`/`uc`) controlling opacity and dashed-ring visual treatment. 0.6° proximity clustering with averaged cluster centres. Rich HTML tooltips with country colors, status tags, host country, and structured format. Bases mode hides non-essential city/port labels for clarity.
- **Theme system**: Dual theme objects (~30 color properties each) with per-element SVG recoloring

---

## Running locally

```bash
git clone https://github.com/nimitmehra/india-maritime-map.git
cd india-maritime-map
open index.html
```

No server needed. Opens in any modern browser. The map loads world data from CDN on first open.

---

## Version history

- **v1–v3**: Initial D3.js maps, iterative projection and label fixes
- **v4**: Datameet India overlay (CW winding fix)
- **v5**: Clean rewrite with 50m data, capitals and ports hover system
- **v7**: Sea lanes, per-port shipping routes for ~50 countries, foreign bases overlay (7 powers, 36 installations), light/dark toggle
- **v8** (current): Expanded to **14 powers and 88 installations**. Renamed from "Foreign Bases" to "Military Bases". Added domestic naval bases for India (6), Pakistan (4), Iran (4), China (3 fleet HQs), UAE, Saudi Arabia, Turkey. Added US island chain positions (Guam, Philippines EDCA, HMAS Stirling/AUKUS), France's Gulf and Indian Ocean bases, NZ Five Eyes. Added Israel, Russia, Italy. Three-tier status system (operational / agreed / unconfirmed). Cluster threshold tightened to 0.6°. Structured tooltips with host country, base name, type, and status. Clean bases mode hides non-essential city labels.

---

## License

MIT

## Author

**Nimit Mehra**
[nimitmehra.com](https://nimitmehra.com) · [@NimitMehra](https://twitter.com/NimitMehra) · [GitHub](https://github.com/nimitmehra)
