# Sled Dash

A fair, random character sled race for picking gift winners. It's one page with no build step.

## Features
- **30 characters, one per player.** A character can't be taken by two players, and names must be different.
- **Blue or pink sled** for each player (♂ / ♀).
- **Gifts to win:** the top N finishers each win, in finishing order.
- **Prize numbers:** you set the total number of prizes, and a random number is drawn before each race ("Winner gets prize number 5"). Numbers that have been won aren't drawn again until you press Reset.
- **Quick race** with numbered racers.
- Dark menus, background music, and generated sound effects.

## How the draw works
The finishing order and the prize numbers come from a Fisher–Yates shuffle that uses `crypto.getRandomValues`. Every racer has an equal chance, and the race animation is only for show.

## Run it
Open `index.html` in a browser, or serve the folder with GitHub Pages.
Players, prizes and settings are saved in each browser's localStorage.
