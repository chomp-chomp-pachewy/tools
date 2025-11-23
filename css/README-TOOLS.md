# Chomp Tools Pages - Complete Set

All 6 tool pages have been recreated with the new unified design system that matches the recipe site.

## Files Included

### CSS Files (Required for all pages)
- `chomp-shared.css` - Common Chomp branding, colors, fonts, dark/light theme
- `tools.css` - Tools-specific styling

### HTML Pages
1. `index.html` - Tools landing page with links to all tools
2. `encode.html` - Encoding/decoding tool (URI, base64, hex, binary, SHA-256)
3. `ip.html` - IP address lookup with WHOIS and location data
4. `inferno.html` - Inferno Ipsum generator (Dante's Inferno text)
5. `nautical.html` - Nautical Ipsum generator (Moby Dick + nautical terms)
6. `subnet.html` - CIDR and subnet calculator
7. `convert.html` - Unit converter (length, volume, mass, temperature, etc.)

## Design Features

### Unified Styling
- **Font**: Inter (matching recipe site)
- **Colors**: 
  - Primary red: #e73b42 (Chomp red)
  - Accent red: #fe0032 (tools accent)
  - Text: #434343, #666666, #7d7d7d
- **Dark/Light Theme**: Toggle button in top-right corner
- **Responsive**: Mobile-friendly layouts

### Common Components
- Navigation bar (links to chomp.ltd, recipes, tools)
- Theme toggle (persists user preference)
- Consistent buttons, inputs, and form styling
- Info boxes for explanations
- Toast notifications for copy actions

## Implementation

### On Each Page
The HTML structure loads:
```html
<!-- Google Fonts -->
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">

<!-- Shared Chomp styles -->
<link rel="stylesheet" href="chomp-shared.css">

<!-- Tools-specific styles -->
<link rel="stylesheet" href="tools.css">
```

### File Organization
For tools.chomp.ltd:
```
/
├── chomp-shared.css
├── tools.css
├── index.html
├── encode.html
├── ip.html
├── inferno.html
├── nautical.html
├── subnet.html
└── convert.html
```

## Functionality Preserved

All original functionality has been maintained:
- **Encode**: All encoding/decoding operations work
- **IP**: API calls to whatismyip.com for live data
- **Inferno**: Random Dante text generation in English/Italian
- **Nautical**: Moby Dick and nautical term generation
- **Subnet**: CIDR calculations, subnet mask conversions, IP range analysis
- **Convert**: All unit conversions with formula display

## Notes

- The IP tool requires an API key (currently embedded in the HTML)
- Dark mode preference is saved to localStorage
- All tools work client-side except IP lookup (which uses external API)
- Images are loaded from GitHub raw URLs

## Next Steps

1. Upload all files to your tools.chomp.ltd domain
2. Update any image URLs if needed
3. Test dark/light theme toggle
4. Verify all functionality works on live site
5. Consider updating the IP API key if needed
