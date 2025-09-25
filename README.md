# Audio Files for Zendesk Multi-Tool

This directory contains the audio files used by the Zendesk Multi-Tool (Ringtone Selector) application.

## Required Audio Files

The application expects the following audio files to be present:

### Ticket Notification Sounds
- `notification.mp3` - Default notification sound
- `chime.mp3` - Gentle chime sound
- `bell.mp3` - Bell sound
- `alert.mp3` - Alert sound

### Call Notification Sounds
- `phone.mp3` - Default phone ring sound
- `ring.mp3` - Classic ring sound
- `urgent.mp3` - Urgent call sound
- `classic.mp3` - Classic phone sound

## Audio File Requirements

- **Format**: MP3 (recommended) or WAV
- **Duration**: 1-3 seconds recommended
- **File Size**: Keep under 100KB per file for optimal performance
- **Sample Rate**: 44.1kHz or 48kHz
- **Bit Rate**: 128kbps or higher for MP3

## Adding Custom Audio Files

1. Place your audio files in this directory
2. Update the `ringtones` object in `app.js` to reference your new files
3. Ensure file names match exactly (case-sensitive)

## Browser Compatibility

The application uses the Web Audio API with HTML5 Audio fallback for maximum compatibility:
- Chrome/Edge: Full Web Audio API support
- Firefox: Full Web Audio API support  
- Safari: HTML5 Audio fallback
- Mobile browsers: HTML5 Audio fallback

## Security Note

All audio files are loaded from the local app bundle to comply with Content Security Policy requirements. External audio URLs are not supported in the production version.
