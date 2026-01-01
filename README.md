# Sunny 3BD Retreat Near CU – GitHub Pages Site

![Fox Den logo](docs/assets/fox_den_logo.png)

This repo hosts a simple, one-page website for the Airbnb listing:

- https://www.airbnb.com/rooms/1529214807731831639

The live site is published using GitHub Pages from the root of this repo (the `index.html` file).

## Editing text

1. Open `index.html` in your browser (on GitHub) or in a code editor.
2. Look for the sections you want to change, such as:
   - The main title: `Sunny 3BD Retreat Near CU – Great Winter Rates`
   - The `Overview` section
   - `Sleeping arrangements`
   - `Amenities`
   - `House rules &amp; good to know`
3. Edit only the text between the HTML tags, for example:

```html
<h1 class="hero-title">Sunny 3BD Retreat Near CU – Great Winter Rates</h1>
<p class="hero-subtitle">
  Bright, comfortable 3 bedroom home in Boulder, close to CU campus, trails, and downtown.
</p>
Avoid changing the surrounding <h1>, <p>, <div>, or class="..." attributes unless you know what you are doing.
Updating price, beds, and other listing details
In index.html, search for:
per night (seasonal) to update the rough nightly rate.
3 bedrooms or 2 bathrooms in the tag line to match your listing exactly.
The Sleeping arrangements section to describe each bedroom more precisely.
These are purely informational — the real source of truth for pricing and rules should remain on Airbnb.
Changing the Airbnb link
If the Airbnb URL ever changes:
In index.html, search for https://www.airbnb.com/rooms/1529214807731831639.
Replace it with the new Airbnb listing URL everywhere it appears.
Keep everything else (the surrounding <a> and <button> tags) the same.
Adding or updating photos
Add your photos into the images/ folder (e.g., living-room.jpg, kitchen.jpg, bedroom.jpg, exterior.jpg).
In index.html, find the Gallery section and update the src paths to match your filenames:
<img class="span-2 tall" src="images/living-room.jpg" alt="Living room with plenty of natural light" />
<img src="images/kitchen.jpg" alt="Kitchen with modern appliances" />
<img src="images/bedroom.jpg" alt="Cozy bedroom with comfortable bed" />
<img class="span-2" src="images/exterior.jpg" alt="Exterior view of the Sunny 3BD Retreat Near CU" />
Update the alt="..." text to describe each photo.
The large hero image at the top of the page also uses an image from images/:
<img src="images/living-room.jpg" alt="Sunny living room at the Sunny 3BD Retreat Near CU" />
You can point this to any image file in the images/ folder.
GitHub Pages
This site is designed to be served directly from index.html in the root of the default branch.
In the GitHub repo:

Go to Settings → Pages.
Under Source, choose:
Deploy from a branch
Branch: your main branch (often main)
Folder: / (root)
Save.
GitHub Pages will rebuild automatically whenever you push changes. After a minute, refresh the live site URL to see updates.
If something looks wrong, you can use GitHub’s history to revert index.html or README.md to a previous version.

4. Do NOT modify anything else
Do NOT delete any other files.
Do NOT modify other config or docs unless explicitly instructed above.
After applying these changes, briefly summarize:
That index.html was replaced with a property-specific landing page using the Airbnb link.
That images/ exists and is tracked (with .gitkeep if needed).
That README.md now explains how to edit text, photos, the Airbnb URL, and GitHub Pages settings.
::contentReference[oaicite:0]{index=0}
