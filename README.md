# Fox Den – Airbnb Landing Page

This repo hosts a simple, standalone website for the **Fox Den** house in Boulder, CO.  
The site is meant to complement the Airbnb listing by showing photos, a description, and a clear “Book on Airbnb” button.

> All bookings and payments are still handled completely through Airbnb.

---

## Live site

Once GitHub Pages is enabled for this repo, the site will be available at a URL like:

- `https://ttuff.github.io/fox_den/`

To check or change this URL:

1. Go to the repo on GitHub.
2. Click **Settings** → **Pages**.
3. Make sure:
   - **Source** is set to your main branch (often `main`).
   - The folder is set to `/ (root)`.

GitHub will show you the exact URL where your site is published.

---

## Where the content lives

The website is a single static page:

- **`index.html`** – The main (and only) page.
- **`images/`** – Folder for photos (living room, kitchen, bedrooms, exterior, etc.).

If you change **`index.html`** and push those changes to GitHub, the live site will update automatically after a short delay.

---

## Editing the text on the page

Most of what you see on the site (titles, paragraphs, amenities, rules, etc.) is defined directly in `index.html`.

### 1. Open the file

1. On GitHub, open this repo.
2. Click **index.html**.
3. Click the **pencil icon** (✏️) to edit.

Or, if you’re working locally, open `index.html` in your code editor.

### 2. Common sections to edit

Search within `index.html` for these headings:

- `Sunny 3BD Retreat Near CU` – main title of the page.
- `Overview` – the main description of the house.
- `Gallery` – short description above the photos.
- `Sleeping arrangements` – text describing each bedroom.
- `Amenities` – list of amenities (Wi-Fi, kitchen, etc.).
- `House rules & good to know` – basic rules section.

You can safely edit the text between the tags, for example:

```html
<h1 class="hero-title">Sunny 3BD Retreat Near CU</h1>
<p class="hero-subtitle">
  Bright, comfortable home in Boulder with easy access to CU campus,
  trails, and downtown.
</p>
Change only the text, not the surrounding <h1> or <p> tags.
3. Updating price / rating / details
In index.html, search for per night (seasonal):
<div class="price-line">
  $XXX <span>per night (seasonal)</span>
</div>
<div class="rating-line">
  <span class="rating-star">★</span> 4.9 average rating
  <span aria-hidden="true">·</span> Superhost
</div>
Update $XXX to roughly match your nightly rate, and adjust the rating text if needed.
Search for 3 bedrooms or 2 bathrooms to update bed/bath counts in the tags:

<span class="tag">
  <span class="tag-icon">🛏</span> 3 bedrooms
</span>
<span class="tag">
  <span class="tag-icon">🚿</span> 2 bathrooms
</span>
Change the numbers or wording as appropriate.
Changing the Airbnb link
The Airbnb listing URL appears several times in index.html.
If your listing URL changes, update all of them.
Search for:

https://www.airbnb.com/rooms/1529214807731831639
Replace it with your new Airbnb listing URL. Keep everything else the same (the surrounding <a> and <button> tags).
Adding or updating photos
Photos are stored in the images/ folder and referenced in index.html.
1. Prepare your image files
Use common formats like .jpg or .png.
Use short, descriptive file names, for example:
living-room.jpg
kitchen.jpg
bedroom.jpg
exterior.jpg
2. Upload images to the images/ folder
On GitHub (web interface):
Click the images/ folder.
Click Add file → Upload files.
Drag and drop your image files.
Commit the changes.
Or, if you’re working locally:
Copy your image files into the images/ folder.
Commit and push your changes.
3. Update the image references in index.html
In the Gallery section, you will see something like:
<div class="gallery-grid">
  <img class="span-2 tall" src="images/living-room.jpg" alt="Living room" />
  <img src="images/kitchen.jpg" alt="Kitchen" />
  <img src="images/bedroom.jpg" alt="Bedroom" />
  <img class="span-2" src="images/exterior.jpg" alt="Exterior of the house" />
</div>
To change which photo appears where:
Update the src="images/..."
Make sure the filename exactly matches the file in the images/ folder.
Update the alt="..." text to describe the photo (this helps accessibility and SEO).
For example, if you upload new-living-room.jpg, rename the line:
<img class="span-2 tall" src="images/new-living-room.jpg" alt="Living room" />
You can reuse the same image in multiple spots if you like.
4. Updating the main hero image
At the top of the page, the large hero image is also defined in index.html:
<img src="images/living-room.jpg" alt="Sunny living room at Fox Den" />
Change the src to any image in your images/ folder to use a different hero photo.
Updating the meta image (link preview)
When you share the site link, platforms may show a preview image. That image is set in the <head> of index.html:
<meta property="og:image" content="https://ttuff.github.io/fox_den/images/living-room.jpg" />
If you change your hero image file name (or want a different preview image):
Make sure the image is in the images/ folder.
Update the content URL to point to the correct file name, for example:
<meta property="og:image" content="https://ttuff.github.io/fox_den/images/new-living-room.jpg" />
House rules & details
In index.html, search for House rules & good to know.
You’ll see a list like this:
<ul class="rules-list">
  <li>Check-in and check-out times follow the Airbnb listing.</li>
  <li>No parties or large events.</li>
  <li>No smoking inside the home.</li>
  <li>Pets only if approved in advance.</li>
  <li>Please respect neighbors and quiet hours.</li>
</ul>
You can:
Add a new rule by adding a new <li>...</li> line.
Edit existing rules by changing the text inside an <li>...</li>.
Make sure each rule stays inside its own <li> tag.
Quick “safe edits” checklist
You can safely do all of the following without breaking the layout:
Change text inside <h1>, <h2>, <p>, and <li> tags.
Update numbers (beds, baths, price) in the visible text.
Update the Airbnb URL (but keep the surrounding HTML tags).
Replace src="images/..." with other image filenames that exist in images/.
Change the alt="..." text on images to better describe the photos.
Avoid changing:
Class names like class="hero-card" or class="gallery-grid".
The surrounding HTML structure (opening/closing tags, <div>, <section>, etc.).
The <style> section unless you’re comfortable editing CSS.
How changes go live
Edit files in GitHub (or locally and push).
Commit your changes.
GitHub Pages automatically rebuilds the site.
After a short delay, refresh your browser at the live URL to see the updates.
If something looks broken, you can always:
Use GitHub’s History view on a file to revert to a previous version.
Restore an earlier commit.
Questions or future improvements
Ideas for future enhancements:
Add more sections (e.g., “For remote workers”, “For families”, “Seasonal notes”).
Include a simple “Contact” section telling people to message you via Airbnb.
Add language about discounts for longer stays if that’s something you offer.
For now, this README should give you (or future helpers) everything needed to safely update photos and text.

---
