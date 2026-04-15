# Clash of Hearts — Game Specification

## 1. Project Overview
- **Type**: Turn-Based RPG Lite (HTML5 Canvas)
- **Concept**: Team Pakistan vs Team India... until they realize they're being pitted against each other by "The Shadow" — a villain representing ignorance, poverty, and division. The final act: both teams unite.
- **Target**: Mobile-first, playable in browser

## 2. Battle Mechanics
- Turn-based: Player turn → Enemy turn
- Player controls: Hero + ally (swappable)
- Move types:
  - **Harmony Strike** (10 DMG): Requires both PK and IN moves used previous turn
  - **Pakistan Attack** (8 DMG): Flag/ crescent move
  - **India Attack** (8 DMG): Chakra/ om move
  - **Heal** (restore 15 HP): Heart move
  - **Unity Defense** (block 80%): Combined shield
- Enemies scale with story progression

## 3. Story Progression
- Stage 1: Pakistan side — fight "Hate Soldier"
- Stage 2: India side — fight "Grudge Knight"
- Stage 3: The Reveal — both teams realize the truth
- Stage 4+: United — fight "The Shadow" together
- Final Boss: "Division Lord"

## 4. Characters (CSS-drawn, simple shapes)
- **Ahmed (PK Hero)**: Green shirt, brave expression
- **Priya (IN Hero)**: Saffron dupatta, determined expression
- **The Shadow**: Dark amorphous form
- **Division Lord**: Giant with chains

## 5. Visual Style
- RPG battle screen — left (PK side), right (IN side)
- Health bars with respective colors
- Spell animations using particles
- Unity moment: combined energy attack (green + saffron = golden)

## 6. Controls
- Desktop: Arrow keys to navigate menu, Enter to select
- Mobile: Tap menu buttons

## 7. Audio
- Battle: synthesized combat sounds
- Harmony Strike: angelic choir
- Unity moment: orchestral swell

## 8. Acceptance Criteria
- [ ] Turn-based combat functional
- [ ] HP/MP system works
- [ ] All 4+ stages with story
- [ ] Team unite mechanic (story trigger)
- [ ] Win/lose conditions
- [ ] Battle animations
- [ ] Start/playing/gameover/victory states
