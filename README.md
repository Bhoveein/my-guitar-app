# My Guitar Chords App 🎸

A simple, web-based guitar chords reference app. Store your favorite songs with chord notations, transpose to different keys, and auto-scroll while practicing.

## Features

### ✨ Core Features
- **Add & Manage Songs** - Store unlimited guitar songs with chord notations
- **Edit & Delete** - Update songs anytime or remove ones you don't need
- **Chord Transposition** - Transpose chords to any key (±12 semitones)
- **Auto-Scroll** - Practice with hands-free auto-scrolling
- **Local Storage** - All songs saved locally in your browser

### 🐛 Bugs Fixed
- **Chord transposition enharmonic equivalents** - Properly handles Bb→A#, Eb→D#, etc.
- **Transpose calculation overflow** - Fixed modulo arithmetic for proper 12-semitone cycling
- **XSS prevention** - HTML escaping on all user input
- **Storage overflow handling** - Graceful handling when storage limit reached
- **Responsive mobile UI** - Better touch targets and mobile layout

### 🚀 Improvements
- **Enhanced UI** - Modern card-based design with better visual feedback
- **Edit songs** - Direct edit button from both list and viewer
- **Delete confirmation** - Modal dialog to prevent accidental deletion
- **Toast notifications** - Feedback for all actions
- **Storage versioning** - Migration-ready storage format
- **Performance** - Better list rendering with grid layout
- **Accessibility** - Better keyboard navigation and focus management

## Usage

### Entering Chords
Use square brackets to denote chords:
```
[G] Amazing grace, [C] how sweet the [G] sound
That [D] saved a wretch [G] like me
```

### Transposing
- Use **Key +** / **Key −** buttons to transpose up/down by semitones
- Display shows current transpose value
- Changes update in real-time

### Auto-Scroll
- Click **Scroll** button to start auto-scrolling
- Click **Stop** to pause
- Great for practicing without holding the phone

## Technical Details

- **Pure JavaScript** - No frameworks or dependencies
- **localStorage API** - All data stored locally on your device
- **Responsive Design** - Works on desktop, tablet, and mobile
- **Cross-browser** - Works on modern browsers (Chrome, Firefox, Safari, Edge)

## Supported Chords

All standard guitar chords:
- **Natural notes**: C, D, E, F, G, A, B
- **Sharps**: C#, D#, F#, G#, A#
- **Flats**: Db, Eb, Gb, Ab, Bb (auto-converted to sharps for consistency)
- **Extensions**: Add m, maj7, 7, sus4, etc. after the chord (e.g., `[Am7]`, `[Cmaj7]`)

## Keyboard Shortcuts

- Add Song: Click "+ Add Song" button
- Back: Click "← Back" button
- Save: Click "Save Song" button

## Browser Compatibility

- ✅ Chrome/Chromium (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)

## Storage Limit

- Maximum 100 songs (~5MB typical)
- Each song limited to 2GB text (practical limit: a few thousand lines)
- Data persists until browser cache is cleared

## License

This project is open source and available under the MIT License.

## Contributing

Found a bug or have a feature request? Please open an issue on GitHub!

---

**Live Demo**: https://bhoveein.github.io/my-guitar-app/
