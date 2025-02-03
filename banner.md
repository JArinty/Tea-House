📌 Explanation of the Code (Relative & Absolute Positioning in Tailwind CSS)


✅ 1. The Outer Container (relative)

##html
```html
<div class="relative">
```
relative: This class sets the position of the parent container to relative.
It means the container will stay in its normal flow, but it becomes the reference point for any absolutely positioned child elements inside it.
Without this, the absolutely positioned card would be placed relative to the entire page instead of this specific container.

✅ 2. The Image

##html

```html
<div>
  <img class="w-full" src="./images/banner.png" alt="" />
</div>
```

w-full: 
 Makes the image take the full width of its parent container.
This acts like a banner or background over which the card will be placed.

✅ 3. The Card (absolute)
html
```html
<div class="absolute flex items-center bg-white shadow-lg p-2 md:px-10 md:py-4">
```
absolute: Positions the card absolutely within the nearest ancestor that has relative (which is the outer container).
This means the card will float over the image, not affecting the normal flow of elements.
Placement: Since no top, left, right, or bottom values are provided, the card defaults to the top-left corner of the parent container.


✅ 4. Card Content (Icon + Text)
Icon Section:

html
```html
<div><i class="fa-solid fa-star font-bold text-amber-500"></i></div>
```
Displays a star icon with a bold, amber color.
Text Section:

html
```html
<div class="ml-2">
  <h1 class="text-2xl font-bold">5.00</h1>
  <p class="text-gray-500">Trust Pilot Ratings</p>
</div>
```
ml-2: Adds margin to the left, creating space between the icon and text.
Typography: Bold, large font for the rating and muted gray color for the description.

🎯 How Relative & Absolute Work Together:
The relative class creates a positioning context.
The absolute class positions the card inside that context, allowing it to overlap the image.
Think of the parent as a canvas (relative), and the card as a sticker (absolute) placed anywhere on that canvas.
