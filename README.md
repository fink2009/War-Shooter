# Super Mario Bros - Enhanced Edition

A feature-rich Super Mario-style platformer game built with vanilla JavaScript and HTML5 Canvas.

## 🎮 Features

### Gameplay & Mechanics
- **Advanced Physics System**
  - Variable jump height (release jump button early for shorter jumps)
  - Coyote time (grace period after leaving platform edges)
  - Jump buffering (queue jump input before landing)
  - Smooth acceleration and deceleration with configurable friction
  
- **Power-Ups**
  - 🍄 **Mushroom**: Grow bigger, break bricks, gain extra hit point
  - ⭐ **Star**: Temporary invincibility with speed boost and rainbow colors
  
- **Coin System**
  - Collect 100 coins to earn an extra life
  - Coin counter updates in HUD
  - Floating score pop-ups on collection
  
- **Level Progression**
  - Flagpole at level end with scoring sequence
  - Level completion screen with time bonus
  - Checkpoint system - respawn at checkpoint after death
  
### Enemies & AI
- **Goomba**
  - Edge detection (turns around at pits and ledges)
  - Walking animation
  - Stomp-able with score rewards
  
- **Koopa Troopa**
  - Shell mechanics - kick shells to defeat other enemies
  - Retract into shell when stomped
  - Emerges after timeout
  
- **Smart Collision Detection**
  - Stomp vs side hit differentiation
  - Squish animations
  - Score pop-ups on enemy defeat

### Audio & Feedback
- **Procedural Sound Effects** (WebAudio API)
  - Jump, coin collect, enemy stomp
  - Power-up collection, player hit/death
  - Brick break, checkpoint activation
  - Flagpole reach
  
- **Background Music**
  - Chiptune-style looping melody
  - Generated dynamically with WebAudio
  - Mute/unmute toggle (M key)
  
- **Visual Feedback**
  - Particle effects for coins and broken blocks
  - Floating score text
  - Power-up visual indicators

### Visuals & UI
- **Parallax Background**
  - Multi-layer clouds moving at different speeds
  - Background hills for depth perception
  
- **Rich Animations**
  - Player run/walk cycles (3 frames)
  - Enemy walking animations
  - Question block bounce on hit
  - Coin spin/rotation illusion
  - Star power rainbow effect
  
- **Pixel-Perfect Rendering**
  - CSS `image-rendering: pixelated` for sharp pixels
  - Consistent tile sizing (32x32)
  - Subpixel rendering disabled
  
- **Enhanced HUD**
  - Score, coins, lives display
  - Countdown timer with time-up penalty
  - Pause state indicator
  - High score and best time tracking
  
- **Debug Overlay** (Toggle with `~` key)
  - FPS counter
  - Player coordinates and velocity
  - Current power-up state
  - Grounded status

### Controls & Accessibility
- **Keyboard Controls**
  - Arrow Keys or WASD: Move left/right
  - Space / W / Up Arrow: Jump
  - P: Pause/Resume
  - M: Mute/Unmute
  - ~ (Tilde): Toggle debug overlay
  
- **Gamepad Support**
  - Standard gamepad mapping
  - D-pad and analog stick for movement
  - A button for jump
  
- **Mobile Touch Controls**
  - On-screen buttons automatically appear on touch devices
  - Left/Right directional buttons
  - Jump button
  - Responsive touch handling

- **Remappable Controls**
  - Customize keyboard bindings
  - Saved to localStorage
  - Reset to defaults option

### Persistence & Polish
- **Local Storage**
  - High score tracking
  - Best completion time
  - Audio preferences (mute state)
  - Control mappings
  
- **Performance Optimizations**
  - 60 FPS game loop with requestAnimationFrame
  - Delta-time based movement
  - Particle object pooling
  - Off-screen entity culling
  - Minimized canvas state changes
  
- **Extended Level Design**
  - Demonstrates all mechanics
  - Multiple coin groups and question blocks
  - Breakable bricks (when big)
  - Pipes as obstacles and visual elements
  - Floating platforms and stairs
  - Strategic enemy placement
  - Mid-level checkpoint
  - Flagpole ending

## 🎯 How to Play

1. Open `index.html` in a modern web browser
2. Click "START GAME" on the title screen
3. Navigate the level, collect coins, and avoid or stomp enemies
4. Collect power-ups to grow stronger
5. Reach the flagpole to complete the level!

## 🎨 Level Elements

- **Ground & Platforms**: Solid surfaces to walk on
- **Floating Platforms**: Suspended platforms accessible by jumping
- **? Blocks**: Hit from below to get coins or power-ups
- **Brick Blocks**: Can be broken when Mario is big
- **Pipes**: Green pipes as obstacles
- **Coins**: Collect for points and extra lives (100 = 1UP)
- **Enemies**: Goombas and Koopas to avoid or defeat
- **Checkpoint**: Flagpole marker - respawn here after death
- **Flagpole**: Level end goal

## ⚡ Power-Up Guide

### Mushroom 🍄
- Makes Mario grow bigger
- Allows breaking brick blocks by hitting from below
- Grants one extra hit (shrinks back to small on damage)

### Star ⭐
- Temporary invincibility (10 seconds)
- Increased movement speed
- Rainbow color cycling effect
- Defeats enemies on contact

## 📊 Scoring

- **Coin**: 100 points
- **Goomba Stomp**: 100 points
- **Koopa Stomp**: 200 points
- **Shell Kick Kill**: 500 points
- **Brick Break**: 50 points
- **Flagpole**: 100-5000 points (height dependent)
- **Time Bonus**: Remaining time × 50 (at level complete)

## 🏆 Objectives

- Collect as many coins as possible
- Defeat enemies for points
- Complete the level as fast as possible for time bonus
- Try to beat the high score!

## 🔧 Technical Details

- **Engine**: Vanilla JavaScript (ES6+)
- **Graphics**: HTML5 Canvas 2D Context
- **Audio**: Web Audio API (procedurally generated)
- **Resolution**: 800×600 (scales to fit screen)
- **Target FPS**: 60
- **No external dependencies or assets**

## 🌟 Special Features

- All art is procedurally drawn with canvas primitives
- All sound effects are generated with WebAudio oscillators
- Fully self-contained in a single HTML file
- Works offline once loaded
- Mobile-friendly with touch controls
- Accessible with keyboard, gamepad, and touch input

## 🐛 Debug Mode

Press `~` (tilde/backquote key) to toggle the debug overlay showing:
- Current FPS
- Player X/Y position
- Velocity (horizontal and vertical)
- Current power-up state
- Grounded status

Useful for development and understanding game physics.

## 📝 Credits

Enhanced edition featuring:
- Improved physics with coyote time and jump buffering
- Multiple power-ups with visual effects
- Advanced enemy AI with edge detection
- Procedural audio system
- Parallax scrolling backgrounds
- Comprehensive HUD and persistence
- Mobile and gamepad support

Enjoy playing this enhanced Super Mario Bros tribute!
