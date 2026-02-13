# Valentine Web App

A playful, interactive Valentine's Day web application that lets you create personalized Valentine messages and share them with someone special.

## Features

### Quick Link Generation
- Generate Link Button: Create a shareable link instantly without previewing
- Preview Option: See the full Valentine experience before sharing
- Enter recipient's name and optional custom message
- Get a shareable URL in seconds

### Interactive Valentine Experience
- Countdown Animation: Dramatic 3-2-1 countdown before the reveal
- Typewriter Effect: Message appears character by character
- Floating Hearts & Confetti: Beautiful animations throughout
- Playful "No" Button: The "No" button runs away when you try to click it
- Success Celebration: Special animation when they say "Yes"

### Share Options
- Copy Link: One-click copy to clipboard
- WhatsApp Integration: Share directly via WhatsApp (mobile & desktop)
- URL Parameters: Links automatically include name and message

### Design & UX
- Mobile-First Design: Fully responsive across all devices
- Romantic Color Palette: Soft pinks, roses, and corals
- Smooth Animations: CSS animations for hearts, confetti, and transitions
- Touch-Friendly: Optimized for mobile touch interactions
- Accessibility: Proper ARIA labels and semantic HTML

## How to Use

### Option 1: Generate Link (Fast)
1. Open valentine.html in your browser
2. Enter the recipient's name
3. Add a custom message (optional)
4. Click "Generate Link"
5. Copy and share the link immediately

### Option 2: Preview First
1. Open valentine.html in your browser
2. Enter the recipient's name
3. Add a custom message (optional)
4. Click "Preview First"
5. Watch the countdown and see the full experience
6. Share after previewing

### For Recipients
1. Click the link you received
2. Watch the countdown
3. Read the personalized message
4. Answer the question: "Will you be my Valentine?"
5. Try clicking "No" if you dare

## Technical Details

### Technologies Used
- Pure HTML/CSS/JavaScript: No frameworks or dependencies
- CSS Variables: Easy theming and customization
- CSS Animations: Smooth, performant animations
- URLSearchParams API: Clean URL parameter handling
- Clipboard API: Modern clipboard functionality with fallback

### Browser Support
- Modern browsers: Chrome, Firefox, Safari, Edge
- Mobile browsers: iOS Safari, Chrome Mobile
- Fallback support for older browsers

### File Structure
```
valentine.html          Main application file (single-page app)
test-generate-link.html Test suite for Generate Link feature
README.md              Documentation
```

## Customization

### Colors
Edit CSS variables in `valentine.html`:
```css
:root {
  --color-primary: #ff6b9d;        /* Soft pink */
  --color-secondary: #c44569;      /* Deep rose */
  --color-accent: #ffa07a;         /* Light coral */
  --color-background: #fff5f7;     /* Very light pink */
}
```

### Messages
Default message is in the `showReveal()` function:
```javascript
messageToDisplay = "You make my heart skip a beat! 💕 ...";
```

### Animations
Adjust animation speeds in CSS:
```css
--transition-fast: 0.2s ease;
--transition-normal: 0.3s ease;
--transition-slow: 0.5s ease;
```

## Testing

Run the test suite:
```bash
open test-generate-link.html
```

Test cases include:
- Generate Link button visibility
- Link generation with correct parameters
- Copy to clipboard functionality
- WhatsApp share integration
- Form validation
- Mobile responsiveness
- URL parameter parsing

## Mobile Optimization

- Touch-friendly button sizes (minimum 44px)
- Responsive font sizes and spacing
- Optimized animations for mobile performance
- iOS-specific fixes (prevents zoom on input focus)
- Touch events for "No" button evasion

## User Flow

### Fast Flow (New)
```
Input Form → Generate Link → Copy/Share → Done
```

### Preview Flow
```
Input Form → Preview → Countdown → Reveal → Question → Share
```

## Tips

- Leave the message blank for a surprise default message
- The "No" button is intentionally evasive - it's part of the fun
- Links work in incognito/private mode for testing
- Custom messages support emojis and special characters

## Known Issues

None currently. Report issues if you find any.

## License

Free to use for personal Valentine's Day messages.

## Credits

Created with love for Valentine's Day 2026
