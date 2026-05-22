# 🌊 Massilia — Pas fâché avec le plaisir

> AI-powered food & lifestyle discovery app for Marseille

---

## 🚀 Run instantly (3 commands)

```bash
npm install
npm start
# Open http://localhost:3000
```

Works out of the box with mock AI responses — no API key needed.

---

## 🤖 Enable real AI (optional)

1. Get a free API key at [console.anthropic.com](https://console.anthropic.com)
2. Create a `.env` file:

```
REACT_APP_ANTHROPIC_API_KEY=your_key_here
```

---

## 📁 Project structure

```
src/
├── App.jsx                  # Router — manages active screen
├── index.js                 # Entry point
├── styles/global.css        # Design system (CSS variables)
├── data/places.js           # Mock data (swap for Supabase)
├── hooks/useAI.js           # Claude API + mock fallback
├── components/
│   ├── BottomNav            # Tab navigation
│   ├── PlaceCard            # Horizontal scroll card
│   └── ListCard             # Vertical list item
└── screens/
    ├── OnboardingScreen     # Welcome + CTA
    ├── HomeScreen           # Mood selector + curated cards
    ├── AIScreen             # Chat concierge
    ├── ExploreScreen        # Map + filtered list
    └── ProfileScreen        # Badges + favourites + prefs
```

---

## 🎨 Design tokens

| Variable       | Value     |
|----------------|-----------|
| `--blue`       | `#29B6F6` |
| `--yellow`     | `#F5B800` |
| `--beige`      | `#FDF6EC` |
| `--dark`       | `#1A1A2E` |
| `--coral`      | `#E8704A` |

---

## 🗄️ Next step — connect Supabase

Replace `src/data/places.js` mock data with real Supabase queries.

Suggested tables: `places`, `profiles`, `reviews`, `saved_places`

---

MIT License · Built with ☀️ in Marseille
