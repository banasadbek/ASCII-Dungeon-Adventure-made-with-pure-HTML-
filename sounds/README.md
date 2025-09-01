# 🎵 Audio Files Directory

This directory contains all the sound effects and background music for the ASCII Dungeon Adventure game.

## 📁 Required Audio Files

### Background Music (Loop)
- `epic_title.mp3` - Title screen theme music
- `dungeon_entrance.mp3` - Ambient dungeon sounds with dripping
- `forest_birds.mp3` - Peaceful forest birdsong
- `cave_drip.mp3` - Cave water dripping sounds
- `goblin_encounter.mp3` - Tense encounter music
- `confident_battle.mp3` - Heroic battle theme
- `victory_treasure.mp3` - Triumphant treasure room music
- `mystical_portal.mp3` - Ethereal portal ambience
- `magical_tension.mp3` - Suspenseful magical energy

### Sound Effects (One-shot)
- `sword_pickup.mp3` - Metal clang of picking up weapon
- `key_pickup.mp3` - Magical chime of finding key
- `battle_victory.mp3` - Victory fanfare after combat
- `death_sound.mp3` - Game over sound effect
- `victory_fanfare.mp3` - Final victory celebration

## 🎚️ Audio Specifications

- **Format**: MP3 (recommended for browser compatibility)
- **Sample Rate**: 44.1kHz
- **Bitrate**: 128kbps minimum
- **Volume**: Pre-balanced in HTML (0.3-0.8 range)
- **Duration**: 
  - Background music: 1-3 minutes (loops)
  - Sound effects: 1-5 seconds

## 🔍 Where to Find Audio

### Free Sources
- **Freesound.org** - Community-created sounds
- **YouTube Audio Library** - Free music and effects
- **OpenGameArt.org** - Game-specific audio
- **Zapsplat.com** - Professional library (free tier)

### Audio Types to Search For
- "dungeon ambience"
- "medieval sword pickup"
- "magical chime"
- "forest birds loop"
- "cave water drip"
- "victory fanfare"
- "death game over"
- "mystical portal"

## ⚠️ Important Notes

1. **Copyright**: Only use royalty-free or Creative Commons audio
2. **File Size**: Keep files under 1MB each for fast loading
3. **Testing**: Verify audio works across different browsers
4. **Fallback**: Game works without audio files (they'll simply not play)

## 🎮 Implementation

Audio files are automatically loaded by the HTML pages:
```html
<audio src="../sounds/filename.mp3" autoplay loop volume="0.4"></audio>
```

The game will continue to function even if audio files are missing - they simply won't play.
