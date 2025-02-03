##Simple Explanation of relative and absolute in CSS
Imagine you're putting a sticker on a notebook:

##The notebook is the container with relative positioning.
The sticker is the card with absolute positioning.
Now, here’s how it works:

✅ 1. relative = "The Notebook"
When you add relative to the container, you’re saying:
"Hey, this is the notebook where I’ll stick things."
The notebook stays in its place like normal (it doesn’t move), but now it’s a reference point for the sticker.
✅ 2. absolute = "The Sticker"
When you add absolute to the card, it’s like placing the sticker anywhere on the notebook.
The sticker doesn’t care about other pages or tables nearby; it only cares about where it’s placed on the notebook (because the notebook is relative).
You can move the sticker around using top, left, right, or bottom.
⚡ Without relative:
If you don’t mark the notebook as relative, the sticker will try to stick itself to the entire desk (the whole page). That’s not what we want.

🎯 Key Point:
relative = Defines the area where things can be positioned.
absolute = Positions things freely inside that area.
