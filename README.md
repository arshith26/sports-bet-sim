# Sports Bet Simulator

A sports betting simulation web app with Flask backend and React frontend. Practice betting with virtual coins and daily bonuses.

## Features

- **Virtual Betting**: Bet with fake money, no real money involved
- **Daily Bonus**: Get 100 coins daily when you log in
- **Multiple Sports**: Cricket, Tennis, Football, Basketball
- **Three Bet Types per Match**:
  - Match Result (Win/Loss/Draw)
  - Over/Under
  - Player Props (Top Scorer, etc.)
- **User Dashboard**: Track balance, betting history, and stats
- **Admin Panel**: Manage events, set odds, settle bets

## Tech Stack

**Backend**: Flask (Python), SQLAlchemy, PostgreSQL/SQLite

**Frontend**: React, React Router

## Project Structure

```
sports-bet-sim/
├── backend/
│   ├── app.py              # Flask app entry point
│   ├── __init__.py         # App factory
│   ├── config.py           # Configuration
│   ├── models.py           # Database models
│   ├── routes/
│   │   ├── __init__.py
│   │   ├── auth.py         # Login/signup
│   │   ├── events.py       # Sports events
│   │   ├── bets.py         # Betting logic
│   │   └── wallet.py       # Daily bonus, balance
│   └── requirements.txt
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   │   ├── LoginPage.jsx
│   │   │   ├── SportsPage.jsx
│   │   │   ├── MatchesPage.jsx
│   │   │   ├── MatchDetailPage.jsx
│   │   │   ├── MyBetsPage.jsx
│   │   │   └── WalletPage.jsx
│   │   ├── App.js
│   │   └── index.js
│   └── package.json
└── README.md
```

## Getting Started

### Backend Setup

```bash
cd backend
python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

pip install -r requirements.txt
flask --app app.py init-db
flask --app app.py run
```

### Frontend Setup

```bash
cd frontend
npm install
npm start
```

## Roadmap

- [ ] User authentication
- [ ] Sports and matches listing
- [ ] Betting system with three markets
- [ ] Daily bonus mechanism
- [ ] Admin panel for event management
- [ ] Leaderboards
- [ ] Live updates (WebSockets)
- [ ] Deployment

## License

MIT
