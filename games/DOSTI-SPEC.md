# The Dosti Diaries — Game Specification

## 1. Project Overview
- **Type**: Visual Novel / Interactive Story (HTML5)
- **Concept**: A Pakistani child (Ahmed) and Indian child (Priya) become pen pals despite their families' prejudice. Choices determine if they overcome obstacles together.
- **Target**: Mobile-first, playable in browser

## 2. Story Structure
- 5 chapters, each ~3-4 choice points
- Chapter 1: The Letter Arrives (Pakistani side)
- Chapter 2: The Reply (Indian side)
- Chapter 3: Misunderstanding (antagonist creates conflict)
- Chapter 4: Standing Up (choices to defend friendship)
- Chapter 5: The Reunion (ending determined by accumulated choices)

## 3. Mechanics
- Choices: 2 options each — one builds unity, one feeds division
- Unity Score: 0-100, determines ending
- Ending A (Unity > 80): Friendship wins, families embrace
- Ending B (Unity 40-80): Bittersweet — separated but still pen pals
- Ending C (Unity < 40): Division wins — families separate them

## 4. Visual Style
- Illustrated storybook aesthetic (CSS-drawn characters, not pixel art)
- Split panels: left = Ahmed's world, right = Priya's world
- Colors shift from grey/divided to warm/unified based on Unity Score
- Backgrounds: Pakistani mountain village, Indian coastal village, city in middle

## 5. Controls
- Desktop: Click choice buttons
- Mobile: Tap choice buttons

## 6. Audio
- Ambient background music (crossfade between PK/IN styles)
- Soft piano on emotional moments
- Heartbeat sound on tension

## 7. Acceptance Criteria
- [ ] All 5 chapters playable
- [ ] Choices affect Unity Score
- [ ] 3 distinct endings
- [ ] Visual shift based on unity level
- [ ] Back/Next navigation
- [ ] Character dialogue boxes
- [ ] Animated transitions
