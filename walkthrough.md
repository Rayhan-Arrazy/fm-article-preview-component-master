# 🗺️ Article Preview Component: Step-by-Step Walkthrough

Welcome to the full roadmap! This guide will help you build your component piece-by-piece. Remember: **there's no rush.** Take it one phase at a time.

---

## Phase 1: Filling the Rooms (HTML Content)
**Goal**: Put the actual "stuff" inside the boxes you built.

*   **Room 1 (Visuals)**: Add an `<img>` tag. Use the file path `./images/drawers.jpg`. Don't forget an `alt` attribute (describe what's in the picture)!
*   **Room 2 (Content)**:
    *   **Headline**: Use a heading tag (`<h1>` or `<h2>`).
    *   **Description**: Use a `<p>` tag for the paragraph.
    *   **Author Section**: Create a `<footer>` inside Room 2. This footer needs:
        1. The avatar image (`./images/avatar-michelle.jpg`).
        2. A small container for the Name and Date.
        3. A `<button>` for the Share icon (`./images/icon-share.svg`).

> [!TIP]
> **Why a button for Share?** Even though it looks like a circle, it's something a user *clicks*. Using a `<button>` tag makes it accessible for everyone!

---

## Phase 2: Setting the Stage (CSS Basics)
**Goal**: Define your "Design System" in a `<style>` tag or a new `style.css` file.

1.  **CSS Variables**: Use the `style-guide.md` to create variables for your colors.
    *   *Example*: `--very-dark-blue: hsl(217, 19%, 35%);`
2.  **Google Fonts**: Import the **Manrope** font (weights 500 and 700).
3.  **The Reset**: Set `box-sizing: border-box` on everything. This makes sure padding doesn't make your boxes wider than you expect!

---

## Phase 3: The Big Move (Layout)
**Goal**: Make the card look like a card instead of a tall tower.

1.  **Centering the Card**: Give your `body` a background color and use Flexbox to put the `.card` right in the middle of the screen.
2.  **Splitting the Card**: 
    *   Give your `.card` a `display: flex`. 
    *   Notice how the image and text jump side-by-side? That's the power of Flexbox!
    *   **Hint**: On mobile, you'll want `flex-direction: column`, but on desktop, you'll want `flex-direction: row`.

---

## Phase 4: Styling the Details (UI Design)
**Goal**: Make the text and spacing match the design.

1.  **The Image**: Make sure the image fills its room. You might need `object-fit: cover`.
2.  **Typography**: Set the font-family, sizes, and colors using your variables.
3.  **Author Section**: 
    *   Use `display: flex` on the author footer.
    *   Use `align-items: center` to make sure the avatar, text, and button are all lined up perfectly in the middle.
    *   **Hint**: Use `margin-left: auto` on the share button to push it all the way to the right!

---

## Phase 5: The "Magic" (Share Tooltip)
**Goal**: Create that pop-up menu.

1.  **The Tooltip**: Create a small `<div>` for the share menu. It should have the word "SHARE" and the three social icons.
2.  **Positioning**: Use `position: absolute` to make it "float" above the button.
3.  **The Toggle**: Use a tiny bit of JavaScript.
    *   When the button is clicked, add a class (like `.active`) to your share menu that changes it from `display: none` to `display: flex`.

---

### 💡 Mentor's Parting Advice
Don't worry about making it perfect on the first try. If your image is too big or your text is won't center, that's just a puzzle waiting to be solved!

**Which phase are you going to tackle first?**
