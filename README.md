# Sheffield Neighbourhoods Archive

An interactive map and reference list of Sheffield's 147 neighbourhoods, created by Data For Action (2022-2025).

## 🗺️ View the Archive

Visit: https://[your-username].github.io/sheffield-neighbourhoods/

## 📋 Contents

- **index.html** - Main webpage with interactive map
- **data/neighbourhoods.geojson** - Neighbourhood boundary data
- **LICENSE** - Creative Commons Attribution 4.0 International

## 🚀 Setting Up GitHub Pages

### Quick Setup (5 minutes)

1. **Create a new GitHub repository**
   - Go to https://github.com/new
   - Name it `sheffield-neighbourhoods` (or any name you like)
   - Make it public
   - Don't add README, .gitignore, or license (we have them)

2. **Upload these files**
   - Upload `index.html` to the root
   - Create a `data` folder and upload `neighbourhoods.geojson` inside it
   - Upload the LICENSE file

3. **Enable GitHub Pages**
   - Go to your repository Settings
   - Scroll to "Pages" in the left sidebar
   - Under "Source", select "Deploy from a branch"
   - Select "main" branch and "/" (root) folder
   - Click Save

4. **Access your site**
   - Wait 1-2 minutes for deployment
   - Visit https://[your-username].github.io/[repository-name]/

### Command Line Setup

If you prefer using Git:

```bash
# Clone or create your repository
git clone https://github.com/[your-username]/sheffield-neighbourhoods.git
cd sheffield-neighbourhoods

# Copy the files
cp index.html .
mkdir -p data
cp neighbourhoods.geojson data/

# Commit and push
git add .
git commit -m "Initial commit: Sheffield Neighbourhoods Archive"
git push origin main
```

Then enable GitHub Pages in repository settings as described above.

## 🎨 Customization

### Update Contact Details

Edit `index.html` around line 225 to change:
- Organization name
- Contact email
- Website link

### Change Map Style

The map uses MapLibre's free demo tiles. To use different tiles, edit line 214 in `index.html`:

```javascript
style: 'https://demotiles.maplibre.org/style.json',
```

### Modify Colors

The neighbourhood boundaries use colors defined around line 294:
- Fill color: `#2c3e50`
- Border color: `#333333`

## 📊 Data

### Neighbourhoods

147 neighbourhoods are mapped across Sheffield, including:
- City Centre areas (Cathedral Quarter, Cultural Industries Quarter, etc.)
- Residential areas (Ecclesall, Crookes, Hillsborough, etc.)
- Outer suburbs (Totley, Dore, Mosborough, etc.)

### Data Format

The GeoJSON file contains:
- **Type**: FeatureCollection
- **Features**: 147 polygon features
- **Properties**: Each feature has a `name` property with the neighbourhood name

## 📜 License

This work is licensed under a [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

You are free to:
- **Share** — copy and redistribute the material
- **Adapt** — remix, transform, and build upon the material

For any purpose, including commercial use, provided you give appropriate credit to Data For Action.

## 📧 Contact

**Data For Action**
- Email: hello@dataforaction.uk
- Website: https://tomcw.xyz

## 🛠️ Technical Details

### Dependencies

- **MapLibre GL JS** v4.0.0 - Loaded from CDN, no installation needed
- No API keys required
- No build process required
- Works offline once cached

### Browser Support

Works in all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)

### File Size

- index.html: ~13KB
- neighbourhoods.geojson: ~170KB
- Total: <200KB

## 🐛 Troubleshooting

**Map doesn't load:**
- Check browser console for errors
- Ensure `data/neighbourhoods.geojson` is in the correct location
- Verify GitHub Pages is enabled in repository settings

**Neighbourhoods not showing:**
- Check that the GeoJSON file is valid
- Ensure the file path in index.html matches your folder structure

**Page not found:**
- Wait a few minutes after enabling GitHub Pages
- Check the repository name matches the URL
- Ensure the repository is public

## 🙏 Acknowledgments

Neighbourhood data compiled by Data For Action from various sources including:
- OpenStreetMap
- Sheffield City Council administrative boundaries
- Local community groups and organizations

---

Created by **Data For Action** (2022-2025)
