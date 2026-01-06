# Assets That Need to Be Created

## Favicon Files

**favicon.svg** - ✅ Created

**favicon.ico** - ⚠️ Needs to be generated
- Use an online tool like [Favicon.io](https://favicon.io/) or [RealFaviconGenerator](https://realfavicongenerator.net/)
- Upload `/favicon.svg` and generate multi-resolution ICO (16x16, 32x32, 48x48)
- Save as `/favicon.ico`

**apple-touch-icon.png** - ⚠️ Needs to be generated
- Size: 180x180px PNG
- Use online converter or image editor to create from `/favicon.svg`
- Background: #fafafa (to match site)
- Save as `/apple-touch-icon.png`

## Open Graph Image

**og-image.jpg** - ⚠️ Needs to be created
- Size: 1200x630px
- Content: ForthBridge logo + tagline on clean background
- Background: #fafafa
- Text: "Health Program Infrastructure for Care Organizations"
- Optimize to <200KB
- Save as `/og-image.jpg`

**Recommended tools:**
- Canva (template: Social Media → LinkedIn Post)
- Figma
- Photoshop/GIMP
- Online OG Image generators

## Quick Generation Steps

### Using online tools (easiest):

1. **Favicons**: Go to https://favicon.io/favicon-converter/
   - Upload `/favicon.svg`
   - Download package
   - Extract `favicon.ico` and `apple-touch-icon.png` to project root

2. **OG Image**: Go to https://www.canva.com/
   - Create 1200x630px design
   - Add logo from `/assets/ForthBridgeLogo.svg`
   - Add tagline
   - Export as JPG
   - Save to `/og-image.jpg`

### Using command line (ImageMagick):

```bash
# Generate favicon.ico from SVG
convert -background transparent favicon.svg -define icon:auto-resize=48,32,16 favicon.ico

# Generate apple-touch-icon.png
convert -background "#fafafa" -resize 180x180 favicon.svg apple-touch-icon.png

# Create OG image placeholder (replace with proper design)
convert -size 1200x630 xc:"#fafafa" -gravity center -pointsize 48 \
  -draw "text 0,0 'ForthBridge'" og-image.jpg
```
