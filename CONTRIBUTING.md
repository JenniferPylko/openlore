# Contributing

If you notice an inconsistency or missing information, you can submit an issue. If you are looking for lore within a specific genre and none of the settings fit, submit an issue. If you find any content that appears *not* to be in the public domain, submit an issue.

If you'd like to add to Open Lore, fork the repo then submit a pull request. Note that I will only accept pull requests that meet the following requirements:

- [x] Any content created by you is marked with CC0 or an equivalent license that places it in the public domain.
- [x] Any content not created by you is in the public domain. For example, you could potentially borrow concepts from existing ancient mythologies, but you could not include anything from someone's copyrighted retelling.
- [x] Your contributions do not contradict existing content or themselves, as far as you or I can tell. The exception to this is that people *in-lore* could be wrong about stuff, so in-lore "sources" may contradict each other. The key concept here is *verisimilitude*.
- [x] Your contributions are reasonably well-formatted and well-written. I realize that this is pretty subjective, so if I don't think the pull request meets these requirements we can have a discussion about it.
- [x] Your contributions are a good fit for Open Lore. Like the previous point, this one's also subjective, and we can discuss it.

If your pull request doesn't meet all of those requirements, it's not a big deal: **you're still free to do whatever you want with Open Lore content!** Not meeting these requirements just means your changes won't make it back upstream.

## Ways to Contribute

Contributions of all types are welcome! This could be just the description of a fictional creature, a record of a fictional historical event, a map, a drawing, a short story, or anything else that adds to the multiverse.

## Style Guide

For consistency's sake, please follow these guidelines.

1. All text content should be Markdown
2. Use relative paths for links
   - This will be most compatible with various tools and environments
3. Only use lowercase letters, numbers, and hyphens in filenames
4. Don't add any more Markdown files to the root directory
   - Add a directory containing an `introduction.md` instead
5. Write descriptions of the multiverse in the past tense
   - This way we avoid setting a specific present moment
6. Write descriptions of the real world in the appropriate tense
   - For example: `Istanbul is a city that used to be called Constantinople`
7. Quoted punctuation goes inside quotes, non-quoted punctuation goes outside
   - For example: `"What?", she exclaimed, defensively.`
8. Always use Oxford commas
9. Include exactly 1 top-level heading per file as the title of the file
10. Do not indent paragraphs
11. Do not use curly quotes
12. When writing out block quotes, do not include quotation marks
    - Italicize the quoted text, then put the source preceded by a hyphen on its own line
13. Avoid multiple links in the same file with the same target
14. Aim for 100-1000 words per file
    - Files much smaller than this should probably be combined, and files much larger should be split

## Tips

I highly recommend using VSCode to read and edit this repository. The `Markdown All in One` and `md-graph` extensions are super useful, and dictionary entries for `Code Spell Checker` are included in `.vscode/settings.json`.

This repository is set up with a GitHub Pages workflow using mdBook. To function properly, every directory must have a file called `introduction.md`, which the auto-summary preprocessor looks for. The root directory is exempt from this, because the workflow renames `README.md` to `introduction.md`. Additionally, the mdBook build workflow deletes the `.gitignore` file, `book.toml`, and the `.github`, `.vscode`, and `media-sources` directories. Files not meant to be uploaded to GitHub Pages should likely go in `media-sources`.

I know many people like Obsidian.md, but I can't personally vouch for it and I don't know if it will work well for this project.