# Travel Diaries: add a new blog post

The Creative Side homepage links to \`travel-diaries.html\`. Add all future travel blogs to the Travel Diaries archive, not to the homepage.

## Steps

1. Upload your collage or photographs into the repository's \`assets/\` folder.
2. Open \`content/travel-diaries.json\`.
3. Add a new object to the \`posts\` array. Keep each post's \`slug\` unique.
4. Use the existing first entry as the structure to copy.

Each entry can contain:
- \`slug\`: URL-safe unique id, e.g. \`weekend-in-goa-2027\`
- \`title\`, \`date\`, \`locations\`
- \`cover\`: path to its main collage or cover image, e.g. \`assets/goa-collage.jpg\`
- \`coverAlt\`: image description
- \`excerpt\`: opening paragraph shown on the archive
- \`body\`: blocks in reading order. Use \`paragraph\`, \`heading\`, or \`image\`.
- \`gallery\`: optional additional photographs
- \`published\`: set to \`false\` to hide a draft

Article links are created automatically at \`travel-post.html?post=YOUR-SLUG\`.

The site displays the text you enter. It does not add hashtags or emojis or rewrite your content.
