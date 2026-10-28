# Tarot Card Matching Game

A fun and educational matching game that helps you learn tarot card meanings by pairing each card name with its corresponding meaning.

## Features

- **Three Difficulty Levels:**
  - Easy: 6 pairs (12 cards)
  - Medium: 10 pairs (20 cards)
  - Hard: 15 pairs (30 cards)

- **Game Mechanics:**
  - Cards are displayed face-down with a mystical crystal ball icon
  - Click to reveal card names and meanings
  - Match each tarot card name with its correct meaning
  - Cards stay revealed when matched correctly
  - Wrong matches briefly show an error animation before flipping back

- **Scoring System:**
  - Earn 100 points for each correct match
  - Lose 10 points for each incorrect match
  - Track your accuracy percentage

- **Performance Tracking:**
  - Timer tracks how long it takes to complete the game
  - Attempts counter shows total matching attempts
  - Matches counter shows successful pairs
  - Real-time score updates

- **Review Screen:**
  - After completing the game, view detailed statistics
  - Review all missed pairs with their correct meanings
  - Learn from mistakes to improve tarot knowledge

## How to Play

1. **Select Difficulty:** Choose Easy, Medium, or Hard from the dropdown menu
2. **Start Game:** Click the "Start Game" button
3. **Match Cards:** 
   - Click any card to reveal it
   - Click a second card to try to match it
   - If the card name and meaning match, they stay revealed
   - If they don't match, they flip back face-down
4. **Complete the Game:** Match all pairs to finish
5. **Review Results:** Check your stats and review any missed pairs

## Data Source

The game uses authentic tarot card data from the repository:
- **Major_Arcana.json**: 22 Major Arcana cards
- **Minor_Arcana.json**: 56 Minor Arcana cards (4 suits)

Each card includes:
- Card name
- Upright meaning
- Keywords
- Additional interpretations for love, career, and finance

## Technical Details

- Pure HTML, CSS, and JavaScript (no external dependencies)
- Responsive design works on desktop and mobile devices
- Fetches card data dynamically from JSON files
- Random card selection ensures different games each time
- Beautiful gradient design with smooth animations

## Running the Game

### Option 1: Direct File Access
Simply open `matching-game.html` in a web browser. Note: Some browsers may block local file access to JSON files due to CORS policies.

### Option 2: Local Server (Recommended)
Run a local web server in the repository directory:

```bash
# Using Python 3
python3 -m http.server 8000

# Using Python 2
python -m SimpleHTTPServer 8000

# Using Node.js (if you have http-server installed)
npx http-server -p 8000
```

Then open your browser to `http://localhost:8000/matching-game.html`

## Tips for Better Scores

1. **Focus on Keywords:** Pay attention to the keywords associated with each card
2. **Learn Patterns:** Major Arcana cards often have more philosophical meanings
3. **Suit Themes:** Minor Arcana cards follow suit themes (Wands=action, Cups=emotion, Swords=thought, Pentacles=material)
4. **Take Your Time:** Accuracy is more important than speed
5. **Review Missed Pairs:** Use the review screen to learn cards you struggled with

## Educational Value

This game helps you:
- Memorize tarot card names and meanings
- Understand the core message of each card
- Build intuitive connections between card names and their interpretations
- Practice active recall, a proven learning technique

Perfect for tarot beginners, students, and anyone wanting to deepen their tarot knowledge in an engaging way!

## License

The tarot card data is licensed under CC0 1.0 Universal (Public Domain) from Oraclume (https://oraclume.com).
