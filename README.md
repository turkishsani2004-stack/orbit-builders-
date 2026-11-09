# Orbit Builders: Junior Astronaut Mission Trainer

A small mobile-first educational browser game for ages 10–16. It uses plain HTML, CSS and JavaScript. No login, database, payment, API key or build tools are required.

## Files
- `index.html` — screen structure and content
- `style.css` — responsive space-themed design
- `game.js` — mission state, decisions, resource changes and win/loss rules

## Run on a phone or computer
1. Extract `orbit-builders.zip`.
2. Open the `orbit-builders` folder.
3. Open `index.html` in a modern browser (Chrome is recommended).
4. Tap **Start Mission**, choose Moon Base or Mars Base, then choose one action each day.
5. Tap **Next Day** to use daily supplies and advance the mission.

For Android editing, import the extracted folder into SPCK Editor. Open `index.html` in its preview/browser option. You can also upload the files to a static host such as GitHub Pages or Vercel.

## How to test
- Start a Moon Base mission and verify the day starts at Day 1.
- Choose each decision card and confirm it can only be selected once per day.
- Tap Next Day and check that the day counter advances and daily supplies decrease.
- Play until Day 7 to see the success screen.
- For a quick failure test, repeatedly advance days while choosing actions that do not restore a low resource; the mission ends when a resource reaches zero.
- Test both Moon Base and Mars Base, then use Restart Mission.

## Game rules
Resource values are illustrative game points from 0 to 100, not real NASA engineering predictions. Each mission lasts up to 7 days. Players choose one action each day; then daily resource use is applied. Reaching zero in oxygen, water, food, energy or crew health ends the mission. Reaching the end of Day 7 with all resources above zero is a success.

## Customization
Edit `actions` and `dailyUse` in `game.js` to adjust game balance. Change colors and layout in `style.css`. Keep the disclaimer visible if you change the resource values.
