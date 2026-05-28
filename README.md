# 🃏 Tarot Card Data

An open-source, structured dataset of all **78 tarot cards** (22 Major Arcana + 56 Minor Arcana) with detailed meanings, keywords, and interpretations.

**Source:** [Oraclume](https://oraclume.com) — your free guide to tarot, astrology, angel numbers & numerology.

## 📦 Dataset Structure

```
tarot-card-data/
├── index.json             # All 78 cards combined (single file)
├── Major_Arcana.json      # 22 Major Arcana cards only
├── Minor_Arcana.json      # 56 Minor Arcana cards (4 suits)
└── README.md              # This file
```

## 📋 Card Schema

Each card entry includes:

| Field | Type | Example |
|-------|------|---------|
| `id` | Integer | 0 |
| `name` | String | "The Fool" |
| `number` | String/Integer | 0 |
| `arcana` | String | "Major" |
| `keywords` | String[] | ["beginnings", "innocence", "spontaneity"] |
| `upright.meaning` | String | "New beginnings, fresh start..." |
| `upright.love` | String | "A new romantic adventure..." |
| `upright.career` | String | "Starting a new job..." |
| `reversed.meaning` | String | "Recklessness, risk-taking..." |
| `reversed.love` | String | "Fear of commitment..." |
| `reversed.career` | String | "Quitting impulsively..." |
| `element` | String | "Air" |
| `astrological` | String | "Uranus" |
| `yes_no` | String | "Yes — take the leap" |

Minor Arcana cards also include:
- `suit` — Wands, Cups, Swords, or Pentacles
- `upright.finance` — Financial interpretation
- `reversed.finance` — Reversed financial interpretation

## 🎯 Quick Start

```bash
# Use directly from GitHub
curl -s https://raw.githubusercontent.com/smallcat419/tarot-card-data/main/index.json

# Or clone the repo
git clone https://github.com/smallcat419/tarot-card-data.git
cd tarot-card-data
```

### Python Example

```python
import json

with open('index.json') as f:
    data = json.load(f)

# Find a card by name
the_fool = next(c for c in data['cards'] if c['name'] == 'The Fool')
print(f"{the_fool['name']}: {the_fool['upright']['meaning']}")
```

### JavaScript Example

```javascript
const data = await fetch('https://raw.githubusercontent.com/smallcat419/tarot-card-data/main/index.json')
  .then(r => r.json());

// Get all Major Arcana cards
const majorArcana = data.cards.filter(c => c.arcana === 'Major');
console.log(majorArcana.map(c => c.name));
```

## 🔮 Use Cases

- **Tarot reading apps** — Build your own digital tarot app
- **Educational tools** — Create learning resources about tarot
- **Websites & blogs** — Power your tarot content with structured data
- **AI training** — Use as structured training data for tarot-related AI models
- **Games** — Build tarot-themed games or interactive experiences

## 📖 Card List

### Major Arcana (22 cards)

| # | Card | Keyword |
|---|------|---------|
| 0 | The Fool | Beginnings, innocence, spontaneity |
| 1 | The Magician | Willpower, skill, manifestation |
| 2 | The High Priestess | Intuition, mystery, inner knowledge |
| 3 | The Empress | Femininity, abundance, nurturing |
| 4 | The Emperor | Authority, structure, stability |
| 5 | The Hierophant | Tradition, spiritual guidance |
| 6 | The Lovers | Love, harmony, choices |
| 7 | The Chariot | Willpower, determination, victory |
| 8 | Strength | Courage, inner strength, compassion |
| 9 | The Hermit | Introspection, solitude, wisdom |
| 10 | Wheel of Fortune | Change, cycles, destiny |
| 11 | Justice | Fairness, truth, law |
| 12 | The Hanged Man | Surrender, pause, new perspective |
| 13 | Death | Transformation, endings, rebirth |
| 14 | Temperance | Balance, moderation, patience |
| 15 | The Devil | Bondage, addiction, materialism |
| 16 | The Tower | Sudden change, upheaval, revelation |
| 17 | The Star | Hope, inspiration, serenity |
| 18 | The Moon | Illusion, fear, uncertainty |
| 19 | The Sun | Joy, success, vitality |
| 20 | Judgement | Rebirth, inner calling, accountability |
| 21 | The World | Completion, accomplishment, fulfillment |

### Minor Arcana (56 cards)

**Wands** (Fire) — Creativity, action, passion
Ace through Ten, Page, Knight, Queen, King

**Cups** (Water) — Emotions, relationships, intuition
Ace through Ten, Page, Knight, Queen, King

**Swords** (Air) — Thoughts, truth, conflict
Ace through Ten, Page, Knight, Queen, King

**Pentacles** (Earth) — Material world, work, finances
Ace through Ten, Page, Knight, Queen, King

## 📄 License

This dataset is released under **CC0 1.0 Universal (Public Domain)**.

You can use, modify, and distribute this data for any purpose without attribution (though attribution is always appreciated ❤️).

## 🤝 Contributing

Found an error or want to add more data? Open an issue or submit a pull request!

## 🌐 About Oraclume

This dataset is maintained by [Oraclume](https://oraclume.com) — a free online resource for exploring tarot card meanings, angel numbers, astrology, zodiac signs, and numerology.

---

⭐ **Star this repo if you find it useful!**
