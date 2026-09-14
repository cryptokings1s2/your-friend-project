# Three-state ARCSultans flow

## What will change
- Replace the rotating background with the supplied `homepage.png` on the landing and success states.
- Switch to the supplied `whitelistpage.png` after “Enter Whitelist” is clicked.
- Keep the existing landing content, whitelist preview, form, corner Sultan GIF cards, links, and fixed footer.
- Show a royal pixel-art confirmation panel only after the form submission succeeds.
- Add “RETURN TO THE KINGDOM” to reset the confirmation back to the landing state.
- Remove the cigarette/face cursor and restore the normal browser cursor everywhere.

## Interaction behavior
- Use three explicit states: Home → Whitelist → Success.
- Fade between states and backgrounds while respecting reduced-motion settings.
- Preserve entered form values while the whitelist form stays open or reports an error.
- Keep users on the whitelist screen when submission fails.

## Technical details
- Use the provided GitHub raw URLs directly with full-viewport, centered `cover` images and pixel-friendly rendering.
- Update the form completion callback so only a confirmed successful response enters the success state.
- Remove custom cursor rendering, cursor-only markers, and related styles.
- Verify desktop and mobile layouts, state transitions, form failure behavior, footer visibility, image loading, and normal cursor behavior.
