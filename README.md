# Riverbend: Screen Reader Practice Site

A fictional city services website with accessibility bugs planted on purpose. Learners use it to practice testing with NVDA and VoiceOver in Deque's instructor-led screen reader training.

**Live site:** https://dequelabs.github.io/screen_reader_practice_riverbend/

> The accessibility bugs on this page are intentional. Please do not fix them in this repo. Each one is a teaching target.

## How to use it

1. Open the live site in the browser that pairs with your screen reader:
   - NVDA: Chrome or Firefox
   - VoiceOver: Safari
2. The page opens in the **version with bugs**.
3. Work through one practice area at a time, using only the keyboard.
4. Press **Show fixed version** in the dark bar at the top to switch to the corrected page. Compare what you hear in each version.

To open the fixed version directly, add `#fixed` to the URL:
https://dequelabs.github.io/screen_reader_practice_riverbend/#fixed

## Practice areas

Each area is labeled on the page and teaches one idea.

| Area | Section | What to test | WCAG success criterion |
| --- | --- | --- | --- |
| 1 | Apply for a permit | Can Tab reach every control? | 2.1.1 Keyboard |
| 2 | Get city updates | Does every control have a name, role, and value? | 4.1.2 Name, Role, Value |
| 3 | Parks and recreation | Does the headings list match the page? | 1.3.1 Info and Relationships |
| 4 | Photo gallery | Does each image say the right thing, or stay silent? | 1.1.1 Non-text Content |

Instructors: the answer key is in the facilitator run sheet, not in this repo, so learners can find the bugs for themselves.

## Commands you need

| Action | NVDA | VoiceOver |
| --- | --- | --- |
| Stop speech | Control | Control |
| Read next item | Down Arrow | VO + Right Arrow |
| Next control | Tab | Tab |
| Activate | Enter or Space | VO + Space |
| List headings, links, images | NVDA + F7 | VO + U |
| Next heading | H | VO + Command + H |

Mac users: in Safari, go to Settings, then Advanced, and turn on **Press Tab to highlight each item on a webpage**. Otherwise Tab skips links.

## About the site

- One self-contained file: `index.html`. All images are embedded, so there is nothing else to install or host.
- Fonts load from Google Fonts. The page works without them.
- The page supports light and dark mode.
- Riverbend, its address, and its services are fictional. This is not a real government site.

## Updating the site

1. Edit `index.html`.
2. Commit to the `main` branch.
3. GitHub Pages republishes within a few minutes.

If you change a practice area, also update the training deck and the run sheet. The deck's screenshots, the answer key, and the expected screen reader announcements all depend on the current markup.

## Credits

- Built by the Deque Systems Instructor-Led Training team.
- Photos come from stock libraries (Unsplash and Pixabay). Check each source's license before reusing them elsewhere.
