# Writing and publishing stories

The Stories page is a reader, not an editor. There are no public write, edit, upload, or delete controls. All writing and publishing happens in this GitHub repository.

## Add a story

1. In GitHub, open `content/stories.json`.
2. Add one object inside the `stories` array. Keep commas and quotation marks valid JSON.
3. Create a folder under `content/stories/` using the story's lowercase hyphenated slug.
4. Add each chapter as a Markdown file in that folder.
5. Commit your changes to `main`. The website will show the story after GitHub Pages deploys.

Example story entry:

```json
{
  "slug": "the-paper-moon",
  "title": "The Paper Moon",
  "author": "Your pen name",
  "genre": "Literary fiction",
  "status": "Ongoing",
  "description": "A short description that invites someone into the story.",
  "cover": "assets/the-paper-moon-cover.jpg",
  "chapters": [
    {
      "title": "Chapter One · The House by the Sea",
      "file": "content/stories/the-paper-moon/chapter-01.md",
      "date": "8 November 2026",
      "wordCount": 850
    }
  ]
}
```

Remove the `cover` property if you do not have a cover image. Add more chapter objects to publish additional chapters.

## Write a chapter

Create a Markdown file at the path specified by the chapter's `file` property. For example:

`content/stories/the-paper-moon/chapter-01.md`

Write the chapter as ordinary text with blank lines between paragraphs. You can use simple Markdown headings:

```md
# Chapter One

The rain began just before sunset.

A second paragraph begins here.

## A New Morning

The next scene begins here.
```

## Edit, reorder, or remove

- Edit a chapter's Markdown file to revise its writing.
- Edit `content/stories.json` to change the title, description, genre, status, cover, chapter titles, chapter order, or chapter file paths.
- To unpublish a story, remove its object from the `stories` array. Its files remain in GitHub unless you separately delete them.

## Important

- Use a unique slug for every story.
- File paths and capitalization must match exactly.
- Use relative paths from the repository root.
- Keep the catalogue valid JSON. A missing comma or quotation mark can prevent the library from loading.
- The live website is read-only. GitHub is the only place where story content can be changed.
