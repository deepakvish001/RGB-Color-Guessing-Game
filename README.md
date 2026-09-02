# ColorSense

ColorSense is a browser-based color recognition game that helps players understand RGB values by turning color matching into a quick visual challenge. The current version supports Easy and Hard modes, randomized color palettes, instant feedback, and replayable rounds without requiring a build tool or backend.

## Current features

- Generate random RGB colors for every round
- Choose between three-color Easy mode and six-color Hard mode
- Receive immediate feedback after every guess
- Reveal the correct palette after a successful answer
- Start a new round without reloading the page
- Run entirely in the browser with no external dependencies

## Technology

- HTML5 for the game structure
- CSS3 for the responsive color grid and visual states
- Vanilla JavaScript for DOM updates, event handling, and random color generation

## Project structure

```text
ColorGameSolution/
├── colorGame.html   # Game markup
├── colorGame.css    # Layout and visual styles
├── colorGame.js     # Game state and interactions
├── Image1.png       # Gameplay screenshot
└── Image2.png       # Gameplay screenshot
```

## Run locally

No package installation is required.

1. Clone the repository.
2. Open `ColorGameSolution/colorGame.html` in a modern browser.
3. Select a difficulty and choose the tile matching the displayed RGB value.

For a local HTTP server, run one of the following commands from the repository root:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080/ColorGameSolution/colorGame.html`.

## How a round works

1. The game creates a palette of random RGB values.
2. One value is selected as the target and displayed in the header.
3. The player compares the RGB channels with the available color tiles.
4. Incorrect tiles are removed from the round.
5. A correct answer reveals the selected color across the complete grid.

## Development roadmap

ColorSense will be expanded in small, reviewable steps. Planned areas include keyboard navigation, accessible announcements, score tracking, timed challenges, additional difficulty levels, deterministic color utilities, unit tests, mobile improvements, theme support, saved preferences, and progressive-web-app capabilities.

## Quality goals

Every contribution should preserve the dependency-free experience, keep game rules understandable, support current browsers, avoid inaccessible color-only feedback, and include focused verification steps.

## Contributing

1. Create a branch from `master`.
2. Keep each change focused on one improvement.
3. Test Easy and Hard modes in at least one desktop and one mobile-sized viewport.
4. Open a pull request describing the behavior before and after the change.
