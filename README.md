# 🪐 checklist

A responsive study timer and task manager built with HTML, CSS,
and vanilla JavaScript.

Stay focused, organize your next steps, and track completed study sessions.

## Features

- Focus and short-break timer modes
- Customizable focus duration: 1–180 minutes
- Customizable break duration: 1–60 minutes
- Start, pause, resume, and reset controls
- Circular timer progress indicator
- Optional session-completion sound
- Task checklist with individual delete controls
- Clear completed tasks
- Completed focus-session and focus-minute totals
- Light and dark themes
- Local storage for tasks, preferences, and statistics
- Responsive layout and reduced-motion support

## Getting Started

1. Download or clone the repository.
2. Open `index.html` in your browser.

No dependencies, installation, or API keys required.

For local development, you can also run:

    python3 -m http.server 8000

Then visit http://localhost:8000.

## How to Use

1. Add the tasks you want to complete.
2. Set your preferred focus and break durations.
3. Select **Focus** and click **Start session**.
4. Pause or resume whenever needed.
5. When the session finishes, start the prepared break timer.
6. Check off completed tasks and review your focus statistics.

Only fully completed focus sessions increase your session
and focus-minute totals. Breaks do not count toward these totals.

## Project Structure

    orbit-focus/
    ├── index.html
    └── README.md

All HTML, CSS, and JavaScript are included in `index.html`.

## Technologies

- HTML5
- CSS3
- Vanilla JavaScript
- SVG progress ring
- Web Audio API
- Browser localStorage

## Saved Data

When browser storage is available, Orbit Focus saves:

- Tasks and completion states
- Completed focus-session totals
- Completed focus-minute totals
- Timer duration preferences
- Theme and sound preferences

Data stays in the current browser and does not sync between devices.
Clearing browser storage removes the saved data.

## Timer Behavior

- Refreshing the page resets an unfinished timer.
- Switching modes resets the current timer.
- Changing a duration resets the current timer.
- The next mode is prepared after completion but starts manually.
- Background tabs may delay completion sounds or messages.
  The timer recalculates from its deadline when the tab becomes active.

## Customization

Edit the CSS variables inside `index.html` to change the colors.
Update the JavaScript defaults to change the initial timer durations.

## Privacy

The website does not upload tasks or statistics to a server.
No account is required.
