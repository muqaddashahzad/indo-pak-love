# Rhythm of Harmony — Game Specification

## 1. Project Overview
- **Type**: Rhythm / Music Game (HTML5 Canvas + Web Audio API)
- **Concept**: A Pakistani Sufi qawwali beat meets Indian Bollywood rhythm. Notes fall from top to bottom — tap when they hit the target zone. Mixes musical elements from both traditions.
- **Target**: Mobile-first, playable in browser

## 2. Game Mechanics
- 3 lanes: left (tabla/dhol), center (vocals), right (sitar/shehnai)
- Notes fall at tempo-synced intervals
- Tempo increases with level (100 BPM → 140 BPM)
- Combo multiplier for consecutive hits
- Antagonists: "Discord" notes — wrong-lane notes that must be avoided (for miss)
- Unity meter: fills when playing both PK and IN instruments in sequence

## 3. Visual Style
- Stage view — two sides: green (PK Sufi musicians) and saffron (IN classical musicians)
- Notes glow in respective colors
- Hit zone pulses to the beat
- Background visualizes audio waveform
- Unity moment: when both sides play together, full-screen burst of light

## 4. Controls
- Desktop: D/F/J/K keys for 3 lanes
- Mobile: Tap left/center/right third of screen

## 5. Audio
- Web Audio API — synthesized tabla, tanpura drone, melodic tones
- Each lane has distinct instrument sound
- Qawwali-style vocal chant on combos
- Bollywood horn section on big combos

## 6. Acceptance Criteria
- [ ] 3-lane note fall with tempo sync
- [ ] Hit/miss detection with scoring
- [ ] Combo system
- [ ] Both PK and IN musical elements
- [ ] Increasing difficulty
- [ ] Unity moments visual
- [ ] Start/play/gameover states
