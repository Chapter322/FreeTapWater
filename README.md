# FairTapWater

[![Website](https://img.shields.io/badge/Visit-fairtapwater.com-2ea44f)](https://fairtapwater.com)
[![GitHub](https://img.shields.io/github/stars/Chapter322/FairTapWater?style=social)](https://github.com/Chapter322/FairTapWater)

Discover restaurants and cafés in the Netherlands that offer free or fairly priced tap water. This project promotes fairness and sustainability by highlighting establishments providing tap water as a courtesy, usually when ordering other items.

## Project Status

Currently in **alpha**. Users are submitting data through our form, with these technical characteristics:
- Data is loaded from [`restaurants.json`](https://github.com/Chapter322/FairTapWater/blob/main/restaurants.json) (generated from YouForm submissions)
- Local caching via `localStorage` (24-hour TTL) for faster subsequent loads
- Manual deduplication required for now

## Technologies & Setup

- Static website hosted at [fairtapwater.com](https://fairtapwater.com) (via [GitHub Pages](https://pages.github.com))
- Interactive map using [Leaflet.js](https://leafletjs.com/) with [MarkerCluster](https://github.com/Leaflet/Leaflet.markercluster)
- Data pipeline: [YouForm](https://app.youform.com/forms/ubbqidvt) → [Airtable](https://airtable.com/) → JSON export
- Third-party services:
  - [OpenStreetMap](https://www.openstreetmap.org/) for base tiles
  - [Google Maps](https://maps.google.com/) for direction links
  - [Youform](https://youform.io/) for submission forms
- Client-side caching with `localStorage`

## Installation

No installation required. Just visit [fairtapwater.com](https://fairtapwater.com) in a modern browser.

## Usage

1. Browse the [interactive map](https://fairtapwater.com) with filters by:
   - Water policy (Free/Reasonable/High price)
   - City selection
2. Click markers for:
   - Restaurant details
   - [Google Maps](https://maps.google.com/) directions
3. Optional features:
   - "Find Near Me" (geolocation)
   - Data caching (24h auto-clear)

## Contributing

### Submit Restaurant Data
[![Submit Form](https://img.shields.io/badge/Submit-Data-blue)](https://app.youform.com/forms/ubbqidvt)

Via our [YouForm submission form](https://app.youform.com/forms/ubbqidvt):
- Required fields: 
  - Restaurant name 
  - Address 
  - Water policy
- Optional: 
  - Experience comments
  - Visit date

### Code Contributions
[![GitHub Issues](https://img.shields.io/github/issues/Chapter322/FairTapWater)](https://github.com/Chapter322/FairTapWater/issues)

1. [Fork the repository](https://github.com/Chapter322/FairTapWater/fork)
2. Create a feature branch
3. Commit changes
4. [Open a pull request](https://github.com/Chapter322/FairTapWater/compare)

Priority areas:
- Automated JSON generation
- Deduplication systems
- UI/UX improvements

## Data Handling
- Local cache auto-clears after 24h
- No user tracking
- Owners may email corrections to [contact@fairtapwater.com](mailto:contact@fairtapwater.com)

## Future Roadmap
- [ ] Automated Airtable→JSON pipeline
- [ ] Deduplication system
- [ ] Restaurant verification

## License
[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/Chapter322/FairTapWater/blob/main/LICENSE)

## Contact
[![Email](https://img.shields.io/badge/Email-contact%40fairtapwater.com-blue)](mailto:contact@fairtapwater.com)
[![GitHub Issues](https://img.shields.io/badge/Report-Issues-red)](https://github.com/Chapter322/FairTapWater/issues)