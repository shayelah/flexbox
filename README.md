# Learning CSS Flexbox

**Web Design I — Coding Exercise**

Flexbox is a CSS layout tool for organizing items **in one direction at a time**: a row or a column. It is especially useful for navigation menus, groups of buttons, spacing items, and centering content.

In this exercise, you'll work through **six guided demonstrations** with your instructor, then complete **four On Your Own challenges** to practice making layout decisions without copying along.

> **The big idea:** The **parent** becomes a flex container, and Flexbox arranges its **direct children** (the flex items). We'll use **CSS Grid** for more complex layouts that need to organize rows *and* columns.

## Getting started

1. Create your own repository from my GitHub template, following the directions in Canvas.
2. Clone **your** repository using GitHub Desktop.
3. Open the **entire project folder** in Visual Studio Code.
4. Open `index.html` using the **Live Preview** extension.
5. Write your Flexbox code in the labeled rules near the **top of `styles.css`**. Save regularly and watch your page change.

## What's in this project?

| File or folder | Purpose |
| --- | --- |
| `index.html` | The HTML page containing the demonstrations and challenges. Most of the HTML is already written for you. |
| `reset.css` | Our familiar reset stylesheet. It loads before your other styles and clears out the browser's default styles. |
| `styles.css` | **This is where you'll write code.** Use the labeled sections near the top. The styles farther down control the page's appearance and should not need changes. |
| `targets/` | Pictures showing what the On Your Own challenges should look like when completed. |

## Guided demonstrations

Follow along during class. Don't just copy: **predict what each change will do before you preview it**.

1. **Turn On Flexbox:** See what happens when a parent becomes a flex container.
2. **Direction:** Compare arranging items in a row versus a column.
3. **Main-Axis Spacing:** Experiment with positioning and spacing items along the main axis.
4. **Cross-Axis Alignment:** Explore alignment in a taller container and how two axes work together.
5. **Wrapping and Gap:** See how items behave when they need more room, and add spacing between them.
6. **Navigation Menu:** Apply Flexbox to a real HTML navigation list.

## On Your Own challenges

After the demonstrations, complete all four challenges in `index.html`:

1. **Navigation Links:** Arrange and space links horizontally.
2. **Perfectly Centered:** Center a message within its container.
3. **Flexible Toolbar:** Place buttons in a row with consistent spacing; let them move to another line when needed.
4. **The Axis Challenge:** Arrange a vertical group at the bottom center of a tall container.

Use the target pictures to judge your results. The instructions tell you **what the finished layout should do**, but you must decide **which CSS properties to use**. Resize the preview when testing the toolbar. If you get stuck, check your notes and the optional hints in Canvas.

## Flexbox glossary: Your quick reference

| Property or term | What it means |
| --- | --- |
| **Flex container** | The parent element whose CSS controls how its direct children are arranged. |
| **Flex items** | The direct children of a flex container. |
| `display: flex;` | Turns an element into a flex container. Its items appear in a row by default. |
| `flex-direction` | Sets the direction of the **main axis**. `row` goes across; `column` goes down. |
| **Main axis** | The direction in which flex items are arranged. With `row`, it is horizontal; with `column`, it is vertical. |
| **Cross axis** | The axis perpendicular to the main axis. |
| `justify-content` | Controls how items are positioned or spaced **along the main axis**. Common values: `flex-start`, `center`, `flex-end`, `space-between`, `space-evenly`. |
| `align-items` | Controls alignment **along the cross axis**. Common values: `stretch`, `flex-start`, `center`, `flex-end`. |
| `flex-wrap` | Determines whether items stay on one line (`nowrap`, the default) or can move to additional lines (`wrap`). |
| `gap` | Adds consistent space **between** flex items, without needing margins on each item. |

**Remember:** `justify-content` does **not** always mean horizontal, and `align-items` does **not** always mean vertical. Their directions depend on `flex-direction`.

### A good way to choose a property

Ask yourself these questions before writing CSS:

1. **Which element is the parent** of the items I want to arrange?
2. Should the items form a **row or column**?
3. Am I trying to move or distribute them on the **main axis**, or align them on the **cross axis**?
4. Should they **wrap** if they run out of room?
5. Do they need more **space between** them?

## Troubleshooting

**Nothing changed after I typed CSS.**  
Save `styles.css`, refresh Live Preview if needed, and check that you're editing the correct file. Make sure the braces `{ }`, colons `:`, and semicolons `;` are correct.

**My items are still stacked vertically.**  
Check that you applied Flexbox to the **parent** containing those items—not just to one of the children.

**The items move in a direction I didn't expect.**  
Check `flex-direction`. Remember that it determines the main axis, and the cross axis changes with it.

**`align-items` doesn't seem to do anything.**  
There may not be much extra space along the cross axis. Look at the size of your container and the items inside it.

**My items won't move onto another line.**  
Check the wrapping behavior on the container. Also make sure the items have a reason to wrap: try narrowing the preview window.

**The spacing doesn't match the target.**  
Compare the *space between items* with the *space at the outer edges*. Those are not always controlled in the same way.

**My changes aren't appearing on GitHub.**  
Saving in VS Code changes your local files only. Open GitHub Desktop, **commit** your changes, and **push** them to GitHub.

## Finishing and submitting

When you finish, compare the demonstrations and challenges with their descriptions and target pictures. Then follow the Canvas directions to commit, push, and publish your work with GitHub Pages, and submit your **GitHub repository URL** (not just your Pages URL).

### Coming next: CSS Grid

Flexbox is great for arranging **a row or a column of items**. For more involved **two-dimensional layouts**, such as main content plus a sidebar or several page regions, we'll learn **CSS Grid** next.
