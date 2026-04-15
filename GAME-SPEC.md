# IndoPak Runner — Game Specification

## 1. Project Overview
- **Type**: Endless Runner (HTML5 Canvas Game)
- **Concept**: A hero named "Indo" runs through a landscape symbolizing the India-Pakistan divide, collecting unity symbols and leaping over "Hate" obstacles. The visual journey transitions from grey/divide to colorful/harmony.
- **Target**: Mobile-first, playable in browser, shareable as a link
- **Domain**: IndoPak.love

## 2. Visual & Rendering Specification

### Canvas Setup
- Responsive canvas (fills screen, max 800x500 for desktop)
- 60 FPS game loop using requestAnimationFrame
- Pixel-art inspired aesthetic (clean, flat, symbolic)

### Color Palette
- **Sky (negative state)**: #8B8B8B → **Sky (positive state)**: gradient #FF6B6B → #FECA57 (sunrise harmony)
- **Ground**: divided — left side earthy brown (PK), right side warm saffron (IN), transitioning to unified green
- **Hero**: circular mascot with PK-green and IN-saffron halves, white heart in center
- **Obstacles (Hate blocks)**: dark charcoal #2D2D2D with spiky shapes
- **Collectibles**: glowing hearts (❤️), unity stars (⭐), and cultural symbols

### Scenes
1. **Start Screen**: Title "IndoPak Runner" with tagline "Love Wins", hero idle animation, "TAP TO START"
2. **Gameplay**: Side-scrolling runner with parallax backgrounds (clouds, landmarks)
3. **Game Over**: Score display, motivational message, "PLAY AGAIN"
4. **Milestone Screen**: Every 500 points, brief "unity flash" showing a fact about Pak-India friendship

### Visual Elements
- **Hero**: Animated circle sprite with bouncing idle, running legs (simple lines), heart pulse
- **Landmarks** (parallax background): Minar-e-Pakistan (left), Taj Mahal (right), transition to merged iconic silhouette
- **Ground**: Runs from grey/divided to vibrant/unified as score increases
- **Particles**: Heart bursts on collect, shadow burst on collision

## 3. Simulation Specification

### Physics
- Gravity: 0.8 px/frame²
- Jump velocity: -15 px/frame
- Double jump allowed (second jump is smaller, -12 px/frame)
- Ground at y=400 (canvas height dependent)

### Speed & Difficulty
- Base speed: 5 px/frame, increases +0.5 per 100 points (max 12)
- Obstacle spawn: every 1500-2500ms (random), gap decreases with score
- Collectibles spawn between obstacles

### Obstacles (Antagonists)
1. **Hate Block**: Static dark block, must jump over
2. **Grudge Spike**: Triangle spike, must duck or time jump
3. **Rumor Cloud**: Floating cloud that requires crouch (down arrow)

### Collectibles
- **Heart** (❤️): +10 points, spawns heart burst particle
- **Unity Star** (⭐): +25 points, spawns golden particle, occasional "unity flash" fact popup
- **Cultural Symbol**: Miniature icon (sitar, tabla, dupatta, chai) — visual variety, +5 points

## 4. Interaction Specification

### Controls
- **Desktop**: SPACE or UP arrow to jump, DOWN arrow to duck, ENTER to start/restart
- **Mobile**: Tap upper half = jump, Tap lower half = duck
- **Double tap**: Double jump

### UI Elements
- Score display (top left)
- Unity meter (top right) — fills as score increases, represents harmony level
- High score persisted to localStorage

### Audio (Web Audio API — synthesized, no files)
- Jump: Short ascending tone (sine wave, 200Hz→600Hz, 100ms)
- Collect: Pleasant chime (sine, 880Hz, 50ms)
- Collision: Low thud (sawtooth, 100Hz, 150ms)
- Milestone: Ascending arpeggio (C-E-G, sine)
- Background: Subtle ambient drone that shifts from tense to harmonious

## 5. Acceptance Criteria
- [ ] Game loads instantly in browser
- [ ] Hero jumps and ducks responsively
- [ ] Obstacles spawn with increasing difficulty
- [ ] Score increments correctly, high score saves
- [ ] Visual transition from divided to unified atmosphere
- [ ] All 3 obstacle types appear
- [ ] All 3 collectible types appear
- [ ] Start, playing, game-over states work
- [ ] Audio plays without delay
- [ ] Mobile touch controls work
- [ ] Unity meter fills as game progresses
- [ ] Milestone facts appear at 500, 1000, 1500+ points
