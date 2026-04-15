# Bridge Builder — Game Specification

## 1. Project Overview
- **Type**: Puzzle / Match-3 lite (HTML5 Canvas)
- **Concept**: Players connect two villages (Pakistani and Indian) by matching tiles to build bridges. Each successful match restores a cultural connection. Antagonists Mr. Hate and Ms. Grudge place obstacles.
- **Target**: Mobile-first, playable in browser

## 2. Game Mechanics
- Grid: 6×6 tiles
- Tile types: PK green, IN saffron, heart (wild), star (wild), cultural symbols
- Tap two adjacent tiles to swap — if 3+ match, tiles dissolve and bridge segment builds
- Every 3 matches = 1 bridge segment complete (5 segments = level done)
- Antagonists: Every 20s, Mr. Hate places a "hate block" that can't be matched (only cleared by 5-match)
- Lives: 3 hearts — lose one when a match isn't made in 15s

## 3. Visual Style
- Split screen — left Pakistani village (green tones), right Indian (saffron), center bridge being built
- As bridge builds, visuals merge — unified village emerges
- Animated water/river between the two sides
- Cultural symbols: chai, tabla, dupatta, cricket bat, book

## 4. Controls
- Desktop: Click two adjacent tiles to swap
- Mobile: Tap two adjacent tiles

## 5. Audio
- Web Audio API synthesized sounds
- Match: chime, 5-match: arpeggio, Hate block: low buzz, Level complete: fanfare

## 6. Acceptance Criteria
- [ ] 6×6 grid renders with distinct tile types
- [ ] Swap/match detection works correctly
- [ ] Bridge segments build visually
- [ ] Antagonist hate blocks spawn periodically
- [ ] Lives system works
- [ ] Level progression (5 levels, increasing speed)
- [ ] Start/play/gameover states
