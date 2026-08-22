# Jack and the House Above the Rain

This repository is an editable example story for [Beta Bot](https://github.com/gennitdev/ai-beta-reader-frontend). It is both a complete illustrated story and a canonical, Git-friendly Beta Bot selection bundle.

The same story data is packaged into Beta Bot as its built-in read-only example. Stable IDs, chapter text, summaries, wiki pages, image assignments, and illustrations are shared between both experiences.

## What is included

- Three parts and seven chapters
- A book cover, unique part covers, and chapter illustrations
- Structured summaries for every part and chapter
- Character and location wiki pages with cover images
- Explicit links between chapters and relevant wiki pages
- Eighteen full-resolution image assets

## Try the bundle in Beta Bot

1. Clone or download this repository.
2. Open **Settings** in Beta Bot.
3. Choose the option to import a bundle folder or bundle ZIP.
4. Select this repository folder, or a release ZIP when one is available.
5. Review the import preview and choose **Apply changes**.

This is a selection bundle. It can add or update the example story, but it cannot replace an entire Beta Bot library.

## Try the Git workflow

The prose and story metadata are ordinary Markdown and YAML files:

- Chapters: `books/*/chapters/*/chapter.md`
- Chapter summaries: `books/*/chapters/*/summary.md`
- Parts and part summaries: `books/*/parts/`
- Character and location pages: `books/*/wiki/`
- Book order and cover assignment: `books/*/book.yaml`
- Image metadata and binary files: `books/*/assets/`

A useful experiment is:

1. Create a branch.
2. Edit a chapter, summary, or wiki page.
3. Commit the change.
4. Validate the repository.
5. Import the folder into Beta Bot again and inspect the proposed changes.

Do not edit `_beta-bot/inventory.json`. It is the immutable exported baseline Beta Bot uses to distinguish unchanged, locally changed, and incoming content.

## Validate the repository

From a checkout of the Beta Bot frontend:

```sh
npm run validate:bundle -- /absolute/path/to/example-story-jack
```

The GitHub Actions workflow performs the same validation for branches and pull requests.

## Canonical format

See the [Beta Bot library bundle specification](https://github.com/gennitdev/ai-beta-reader-frontend/blob/main/docs/book-folder-format.md) for the complete file format and import semantics.

## Licensing

The licensing terms for the story and illustrations must be chosen before this repository is promoted for public reuse. No content license is granted by this README.
