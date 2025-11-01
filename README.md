# MoveWise

A small React app that helps users find their ideal U.S. city based on personal preferences like temperature and political lean.

Users adjust sliders and set how important each factor is, and the app ranks cities from a dataset to show which ones are the best fit.

My primary purpose for this project was to gain experience using AI to develop code, as I don't for school and can't for work. Mostly used GPT-4o via GitHub CoPilot. The app is currently in a demo state. 

---

## Features

- Interactive quiz with sliders and importance buttons  
- Real-time city ranking based on preferences  
- Easy to add more questions or cities  

---

## Setup

Clone the repository and start the app locally:

```bash
git clone https://github.com/rreop/MoveWise.git
cd where-should-i-live
npm install
npm run dev
```

---

## How to Customize

City attributes are expressed as a number value between 0 and 100. For example, average_temperature being 0 means the city is among the coldest in the United States, and 100 means the city is among the hottest.

Add new quiz questions in App.jsx by extending the questionHooks array and adjusting the scoring algorithm.

Update or add cities in src/data/cities.json.
Each city entry looks like:
```json
{
  "name": "Seattle, WA",
  "average_temperature": 60,
  "political_lean": 80
}
```

---

## TODO

- Add more quiz questions (e.g., cost of living, importance of low crime, population size)
- Add more cities
- Use accurate city information
- Rebuild scoring algorithm to allow for easier question addition
- Switch to a quiz submission and results page format
- Host the app online
- Improve styling and layout
