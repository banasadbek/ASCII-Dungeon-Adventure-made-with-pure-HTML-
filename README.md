# 🏗️ ASCII Dungeon Adventure

![Game Logo](https://img.shields.io/badge/Game-ASCII%20Adventure-green) ![HTML](https://img.shields.io/badge/HTML-Pure-orange) ![Sound](https://img.shields.io/badge/Audio-Enabled-blue)

**A pure HTML text-based adventure game featuring ASCII art, immersive sound effects, and branching storylines.**

## 🎮 Game Overview

Navigate through a mysterious dungeon using only HTML links! Every choice you make shapes your adventure in this retro-style text-based RPG. No JavaScript required - just pure HTML magic with atmospheric sound design.

### 🌟 Features

- **🎨 ASCII Art**: Hand-crafted scenes for every location
- **🔊 Immersive Audio**: Background music and sound effects for every action
- **🌿 Multiple Paths**: Forest, cave, and dungeon routes with different outcomes
- **⚔️ Inventory System**: Pick up weapons and items that change your options
- **🏆 Multiple Endings**: Death, victory, and secret endings to discover
- **🎯 Pure HTML**: No JavaScript - works in any web browser
- **📱 Responsive**: Plays well on desktop and mobile devices

## 🗂️ File Structure

```
game/
├── index.html              # Title screen & game start
├── rooms/                  # Game locations
│   ├── room1.html         # Dungeon entrance
│   ├── room2.html         # Dark hallway (unarmed)
│   ├── room2_sword.html   # Dark hallway (with sword)
│   ├── forest.html        # Peaceful forest
│   ├── cave.html          # Hidden cave with crystal
│   └── treasure.html      # Victory treasure chamber
├── inventory/              # Item state variations
│   ├── sword.html         # Armed entrance state
│   └── key.html           # Armed + key state
├── transitions/            # Sound effect pages
│   ├── pickup_sword.html  # Sword acquisition
│   ├── pickup_key.html    # Key discovery
│   └── battle_victory.html# Combat victory
├── endings/                # Game conclusions
│   ├── death.html         # Game over
│   ├── win.html           # Standard victory
│   └── secret.html        # Hidden mystical ending
└── sounds/                 # Audio files (add your own!)
    ├── epic_title.mp3
    ├── dungeon_entrance.mp3
    ├── forest_birds.mp3
    ├── cave_drip.mp3
    ├── goblin_encounter.mp3
    ├── confident_battle.mp3
    ├── victory_treasure.mp3
    ├── death_sound.mp3
    ├── victory_fanfare.mp3
    ├── mystical_portal.mp3
    ├── magical_tension.mp3
    ├── sword_pickup.mp3
    ├── key_pickup.mp3
    └── battle_victory.mp3
```

## 🚀 How to Play

1. **Start the Game**: Open `game/index.html` in any web browser
2. **Make Choices**: Click on the yellow links to navigate and make decisions
3. **Manage Inventory**: Pick up items to unlock new options and paths
4. **Explore Multiple Paths**: 
   - **Safe Route**: Forest → Peaceful ending
   - **Combat Route**: Sword → Fight goblin → Treasure
   - **Mystery Route**: Cave → Crystal → Secret ending
   - **Advanced Route**: Sword + Key → Ultimate secret
5. **Discover Secrets**: Look for hidden expandable sections and special choices

### 🎵 Audio Experience

The game features rich audio design:
- **Background Music**: Each location has its own atmospheric soundtrack
- **Sound Effects**: Item pickups, battles, and discoveries have unique sounds
- **Transitions**: Special pages with sound effects between major actions
- **Volume Control**: All audio is pre-balanced for optimal experience

> **Note**: Some browsers may block autoplay audio until user interaction. Click anywhere on the page if audio doesn't start automatically.

## 🎯 Game Mechanics

### Inventory System
The game simulates inventory through **file variations**:
- `room1.html` → No items
- `inventory/sword.html` → Same location with sword
- `inventory/key.html` → Armed with sword AND key

### State Management
Each HTML file represents a complete game state:
- Room description + inventory + available actions
- Links lead to different files based on your current state
- No databases or cookies - everything is in the file structure

### Multiple Endings
- **💀 Death**: Poor choices or lack of preparation
- **🏆 Victory**: Standard success through combat or peace
- **✨ Secret**: Hidden mystical transcendence ending

## 🎨 Technical Architecture

### Pure HTML Adventure Engine
- **Pages = Game States**: Each room/situation is an HTML file
- **Links = Actions**: `<a href>` tags represent player choices
- **ASCII Art**: `<pre>` blocks contain hand-crafted scenes
- **Sound Integration**: `<audio>` tags with autoplay for immersion
- **Responsive Design**: CSS styling optimized for all devices

### Sound System
- **Ambient Loops**: Background music using `autoplay loop`
- **Effect Triggers**: Transition pages play sounds then redirect
- **Volume Balancing**: Each audio element has optimized volume levels
- **Browser Compatibility**: Fallback behavior for audio-blocked browsers

## 🛠️ Customization Guide

### Adding New Rooms
1. Create new HTML file in `rooms/` directory
2. Follow the template structure with CSS styling
3. Add ASCII art in `<pre>` blocks
4. Include background audio with `<audio>` tag
5. Link from existing rooms

### Adding Sound Effects
1. Place audio files in `sounds/` directory
2. Reference with relative paths: `../sounds/filename.mp3`
3. Use `autoplay` for automatic playback
4. Use `loop` for background music
5. Set appropriate `volume` levels (0.1 - 1.0)

### Creating Inventory States
1. Duplicate existing room file
2. Modify ASCII art to show new inventory
3. Update available actions/links
4. Change inventory display section
5. Link from item pickup transition

## 🎵 Audio File Requirements

### Recommended Audio Formats
- **MP3**: Best browser compatibility
- **OGG**: Open source alternative
- **WAV**: Uncompressed option

### Audio Guidelines
- **Background Music**: 1-3 minute loops, volume 0.3-0.4
- **Sound Effects**: 1-5 second clips, volume 0.5-0.8
- **File Size**: Keep under 1MB each for fast loading
- **Sample Rate**: 44.1kHz standard
- **Bitrate**: 128kbps minimum for quality

### Suggested Audio Sources
- **Freesound.org**: Community sound effects
- **Zapsplat.com**: Professional audio library
- **YouTube Audio Library**: Free background music
- **OpenGameArt.org**: Game-specific sounds

## 🎮 Gameplay Tips

### For Players
- **Explore Everything**: Click on expandable sections for hidden content
- **Think Strategically**: Some paths require specific items
- **Multiple Playthroughs**: Different choices reveal new content
- **Audio Immersion**: Play with sound on for the full experience

### For Developers
- **Test All Paths**: Verify every link works correctly
- **Audio Testing**: Check volume levels across different browsers
- **Mobile Optimization**: Test on various screen sizes
- **Load Times**: Optimize audio file sizes

## 🔧 Browser Support

### Fully Supported
- ✅ Chrome/Chromium (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge

### Audio Limitations
- Some browsers block autoplay until user interaction
- Mobile browsers may have different audio policies
- Older browsers might not support all audio formats

## 📝 Development Notes

### Architecture Benefits
- **No Server Required**: Pure client-side HTML
- **Easy to Modify**: Simple file structure
- **Version Control Friendly**: Each state is a separate file
- **Scalable**: Add rooms/paths without complex logic

### Technical Considerations
- **File Duplication**: Inventory states create similar files
- **Audio Loading**: Large audio files may slow initial load
- **Browser Caching**: Repeated playthroughs load faster
- **SEO Friendly**: Each page is indexable HTML

## 🤝 Contributing

Want to expand the adventure?

1. **Fork the Project**
2. **Add New Rooms**: Create additional HTML files with unique ASCII art
3. **Enhance Audio**: Add more sound effects and music tracks
4. **Expand Storylines**: Create new branching paths and endings
5. **Submit Pull Request**: Share your improvements!

### Contribution Ideas
- 🏰 New dungeon levels
- 🎵 Original soundtrack compositions  
- 🎨 Enhanced ASCII art scenes
- 📚 Additional story branches
- 🔧 Mobile interface improvements

## 📜 License

This project is open source and available under the MIT License.

## 🎯 Credits

- **Game Design**: Classic text adventure inspiration
- **ASCII Art**: Hand-crafted for atmosphere
- **Sound Architecture**: Pure HTML audio implementation
- **Responsive Design**: Modern CSS styling

---

**Ready to begin your adventure? Open `game/index.html` and step into the dungeon!** 🗡️✨

*May your choices be wise and your sword stay sharp...*
