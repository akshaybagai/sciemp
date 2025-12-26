# Company Logos Guide

This folder is for storing company logos for the Partners section.

## How to Add Logos

### Step 1: Obtain Logos
Download high-resolution logos for each company. The best sources are:
1. Company's official website (usually in their "Press Kit" or "Media" section)
2. Contact the company directly for their official logo
3. Search for "[Company Name] logo png" on Google Images

### Step 2: Save Logos
Save logos in this folder with descriptive names:
- `borosil.png`
- `transasia.png`
- `rankem.png`
- `qualigen.png`
- `biocare.png`
- `genei.png`
- `jmitra.png`
- `arkray.png`
- `reckon.png`
- `himedia.png`
- `pethozyme.png`
- `athenese.png`
- `oxalis.png`
- `aspen.png`
- `rapid.png`
- `immunoscience.png`
- `calbiotech.png`
- `sdbiosensor.png`
- `bluestar.png`

### Step 3: Update HTML
Replace the text in each partner card with an image tag.

**Before:**
```html
<div class="partner-logo">
    <span>Borosil Scientific Ltd</span>
</div>
```

**After:**
```html
<div class="partner-logo">
    <img src="logos/borosil.png" alt="Borosil Scientific Ltd">
</div>
```

### Step 4: Uncomment CSS
In `styles.css`, uncomment the logo image styles (around line 580):
```css
.partner-logo img {
    max-width: 100%;
    max-height: 80px;
    object-fit: contain;
    filter: grayscale(100%);
    opacity: 0.7;
    transition: all 0.3s ease;
}

.partner-card:hover .partner-logo img {
    filter: grayscale(0%);
    opacity: 1;
}
```

## Logo Specifications

**Recommended:**
- Format: PNG with transparent background
- Minimum width: 300px
- Aspect ratio: Preserve original
- File size: < 100KB each

## Company Website Links

Use these to find official logos:

1. **Borosil Scientific**: https://www.borosilscientific.com/
2. **Transasia Bio-Medicals**: https://www.transasiabio.com/
3. **Rankem**: https://www.rankem.com/
4. **Hi-Media**: https://www.himedialabs.com/
5. **J.Mitra & Co**: https://www.jmitra.co.in/
6. **ARKRAY Healthcare**: https://www.arkray.co.in/
7. **SD Biosensor**: https://www.sdbiosensor.com/

For others, search: "[Company Name] official website logo"

## Tips

- Always use official logos provided by the company
- Maintain consistent sizing across all logos
- Use transparent backgrounds when possible
- Test logos on both light and dark backgrounds
- Keep original files as backup before optimization


