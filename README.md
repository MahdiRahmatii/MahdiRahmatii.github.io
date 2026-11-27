# Mahdi Rahmati — Portfolio

A bilingual (English/Persian), folder-driven static portfolio hosted on GitHub Pages.

## Content architecture

- `Projects/<slug>/project.json` — project cards and case-study metadata.
- `Articles/<category>/<slug>/article.json` — article metadata; article body can live in `content.md`.
- `Services/<slug>/service.json` — services offered.
- `Experience/<slug>/experience.json` — professional roles.
- `Teaching/<slug>/teaching.json` — courses and teaching activities.
- `About/profile.json` — profile identity and the single profile image path.
- `About/education.json`, `About/certifications.json` — education and credentials.
- `Skills/index.json` — skills list.
- `Contact/contact.json` — public contact channels.
- `config/site.json`, `config/navigation.json` — site-wide settings and navigation.

## Add content

Create the folder and its JSON file, then add its slug to that section's `index.json` manifest. The existing site layout and JavaScript do not need to be edited for ordinary content additions.

User-facing text should use bilingual objects:
```json
{ "en": "English text", "fa": "متن فارسی" }
```

Keep project/article media beside the content that uses it. The public site can expose all files committed to this public repository; do not store secrets or private client assets here.

## Profile image

Place one image at `About/media/profile.webp`. The site reads its path from `About/profile.json`. Until a real image is added, the initials placeholder is displayed.

## Evidence

Initial experience and project claims should remain limited to the information supported by the supplied CVs or verified project evidence. Do not publish invented project names, metrics, or article publication claims.
