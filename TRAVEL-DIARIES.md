# Travel Diaries

The Creative Side homepage contains a single link to `travel-diaries.html`. All travel content lives on this separate page.

The page has five sections:

1. **Travel Stories** — add full blog posts to the `posts` array in `content/travel-diaries.json`. Each post needs a unique `slug`, title, date, locations, cover image, excerpt and body. The article opens at `travel-post.html?post=YOUR-SLUG`.
2. **Postcards** — add image objects to the `postcards` array:
   ```json
   { "image": "assets/your-photo.jpg", "alt": "Describe the photograph.", "caption": "Optional caption." }
   ```
3. **Places Worth Returning To** — add objects to `placesWorthReturningTo`:
   ```json
   { "title": "Place name", "location": "Region or country", "note": "Why you would return." }
   ```
4. **Little Travel Notes** — add short strings to `littleTravelNotes`.
5. **Travel Wishlist** — add destination names to `travelWishlist`.

Upload collages and photographs to the repository's `assets/` folder and use repository-relative paths beginning with `assets/`.

Supported article body blocks are `paragraph`, `heading`, and `image`. Use `published: false` to hide a draft story.

The website displays the words you add. It does not add emojis or hashtags or rewrite your content.
