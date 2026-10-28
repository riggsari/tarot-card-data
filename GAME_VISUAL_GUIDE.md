# Tarot Card Matching Game - Visual Guide

## Game Flow

### 1. Start Screen
```
┌─────────────────────────────────────────┐
│     🔮 Tarot Card Matching Game 🔮      │
│   Match each tarot card with its meaning!│
│                                          │
│  Difficulty: [Medium ▼]                 │
│                                          │
│  Time: 0:00  Matches: 0                 │
│  Attempts: 0  Score: 0                  │
│                                          │
│         [Start Game]                    │
└─────────────────────────────────────────┘
```

### 2. Game Board (Face Down)
```
┌─────────────────────────────────────────┐
│  Time: 0:15  Matches: 2  Attempts: 5    │
│  Score: 170                             │
│                                          │
│  ┌───┐ ┌───┐ ┌───┐ ┌───┐ ┌───┐        │
│  │🔮 │ │🔮 │ │🔮 │ │🔮 │ │🔮 │        │
│  └───┘ └───┘ └───┘ └───┘ └───┘        │
│                                          │
│  ┌───┐ ┌───┐ ┌───┐ ┌───┐ ┌───┐        │
│  │🔮 │ │🔮 │ │🔮 │ │🔮 │ │🔮 │        │
│  └───┘ └───┘ └───┘ └───┘ └───┘        │
│                                          │
│  ┌───┐ ┌───┐ ┌───┐ ┌───┐ ┌───┐        │
│  │🔮 │ │🔮 │ │🔮 │ │🔮 │ │🔮 │        │
│  └───┘ └───┘ └───┘ └───┘ └───┘        │
│                                          │
│  ┌───┐ ┌───┐ ┌───┐ ┌───┐ ┌───┐        │
│  │🔮 │ │🔮 │ │🔮 │ │🔮 │ │🔮 │        │
│  └───┘ └───┘ └───┘ └───┘ └───┘        │
│                                          │
│         [Reset Game]                    │
└─────────────────────────────────────────┘
```

### 3. Cards Revealed (During Play)
```
┌─────────────────────────────────────────┐
│  ┌─────────┐ ┌─────────┐ ┌───┐         │
│  │The Fool │ │New begin│ │🔮 │         │
│  │  ⭐     │ │nings... │ │   │         │
│  └─────────┘ └─────────┘ └───┘         │
│   (Selected)   (Selected)                │
│                                          │
│  ┌─────────┐ ┌─────────┐               │
│  │The      │ │Manifesta│               │
│  │Magician │ │tion...  │               │
│  └─────────┘ └─────────┘               │
│   (Matched)    (Matched)                │
└─────────────────────────────────────────┘
```

### 4. End Game Modal
```
┌─────────────────────────────────────────┐
│         🎉 Game Complete! 🎉            │
│                                          │
│  ┌─────────────────────────────────┐   │
│  │ Time: 2:34                      │   │
│  │ Total Matches: 10               │   │
│  │ Total Attempts: 15              │   │
│  │ Accuracy: 67%                   │   │
│  │ Final Score: 900                │   │
│  └─────────────────────────────────┘   │
│                                          │
│  Missed Pairs Review:                   │
│  ┌─────────────────────────────────┐   │
│  │ The High Priestess              │   │
│  │ Trust your intuition, look      │   │
│  │ beneath the surface...          │   │
│  └─────────────────────────────────┘   │
│                                          │
│  ┌─────────────────────────────────┐   │
│  │ The Tower                       │   │
│  │ Sudden upheaval, chaos,         │   │
│  │ revelation, awakening...        │   │
│  └─────────────────────────────────┘   │
│                                          │
│     [Close]    [Play Again]             │
└─────────────────────────────────────────┘
```

## Color Scheme

- **Background**: Purple gradient (mystical theme)
- **Face-down cards**: Pink gradient with crystal ball 🔮
- **Selected cards**: Gold border with glow effect
- **Matched cards**: Soft teal/pink gradient (faded)
- **Wrong match**: Red border with shake animation
- **Text**: Dark purple for card names, gray for meanings

## Responsive Design

### Desktop (1200px+)
- 5 columns of cards
- Large, readable text
- Spacious layout

### Tablet (768px - 1199px)
- 3-4 columns of cards
- Medium text size
- Compact but comfortable

### Mobile (< 768px)
- 2 columns of cards
- Smaller text
- Vertical stats layout
- Touch-friendly card sizes

## Game States

1. **Initial**: Difficulty selector active, Start button visible
2. **Playing**: Cards face-down, timer running, stats updating
3. **Card Selected**: First card revealed with gold border
4. **Checking Match**: Two cards revealed, brief pause
5. **Match Success**: Cards stay revealed with matched styling
6. **Match Failure**: Cards shake, then flip back face-down
7. **Game Complete**: Modal appears with statistics and review

## Accessibility Features

- Large, clickable card areas
- Clear visual feedback for all interactions
- High contrast text
- Keyboard-friendly (can be enhanced)
- Responsive to different screen sizes
- Clear status indicators

## Performance Features

- Smooth CSS animations
- Efficient DOM updates
- Random card selection algorithm
- No external dependencies
- Fast load time
