# Mahdi Rahmati — Portfolio content system

This is a static GitHub Pages portfolio. Content is stored as data in individual folders.

## Add a project
1. Create `Projects/<project-slug>/project.json`.
2. Add the folder slug to `Projects/index.json` → `items`.
3. The Projects section loads and renders it automatically; no HTML/CSS/JS edit is required.

## Add an article
1. Create `Articles/<article-slug>/article.json`.
2. Add the folder slug to `Articles/index.json` → `items`.
3. The Writing section loads and renders it automatically.

## Content format
Use bilingual `en` and `fa` objects for user-facing text. Project JSON fields currently used:
`slug`, `title`, `organization`, `period`, `category`, `role`, `summary`, `details`, `highlights`, `evidence`, `media`.

Article JSON fields currently used:
`slug`, `title`, `date`, `category`, `excerpt`, `content`, `url`.

Keep media inside the same content folder (for example `Projects/<slug>/media/`) and reference it with a relative path from the repository root.

## Evidence policy
Initial project entries are limited to claims supported by the CV. The CV does not list published articles or individual project titles/details, so no article entries or unsupported project specifics have been invented.
