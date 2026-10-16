# Portfolio upgrade notes

## Project type
The supplied project is a static HTML/CSS/JavaScript Bootstrap portfolio template, not a React application. The upgrade preserves the existing template and dependencies.

## Contact form
No backend/email provider credentials or working mail endpoint were included. The form validates fields and prepares an email using `mailto:zolakid50@gmail.com`; the visitor must send it from their email app. The page explicitly does not claim the message was sent.

## Repository links
- Evangadi Forum: `https://github.com/zeleke21977/evangadi-forum`
- GPT Clone: `https://github.com/zeleke21977/gpt-clone`
- Netflix Clone: no repository button is shown because a repository URL could not be verified in the supplied project.

## Remaining configuration
Add exact social profile URLs if you want social links displayed. For server-side contact delivery, configure a real backend or email provider and credentials on the hosting platform; do not put secrets in client-side JavaScript.


## Project logo thumbnails
The project cards now use local, lightweight SVG logo-style thumbnails for Netflix Clone, GPT Clone (ChatGPT-inspired), and Evangadi Forum. Clicking each logo or project title opens that project's supplied live demo in a new tab. These are portfolio thumbnail graphics, not official brand asset downloads.

## Demo link fix (latest)
- Cause: the hover overlay covered each project logo, so clicks landed on the overlay instead of the link. The overlay now wraps only the logo (`.project-media`) and ignores pointer events except for its open-demo icon.
- Logo, project title, hover icon and "Live Demo" button on every card open the matching live demo in a new tab (verified by automated click test).
- Removed the zoom icon: it opened unrelated template stock photos, not the real projects.
- Evangadi Forum uses the bundled `assets/img/projects/forum-logo.svg`. To use the official logo instead, drop it in that path (same filename).
- Added a note that Render free-tier demos can take 30-60 s to wake.

## Final pass
- Added GitHub profile link (github.com/zeleke21977, taken from your repo URLs) to Contact and footer.
- Contact form: mailto plus a "Compose in Gmail" fallback link built from the same fields.
- Breadcrumbs/titles now match nav (Skills, How I Build, Projects); added share meta tags.
- Removed 29 unused template images (smaller download). Checked: no JS errors, no missing files, no horizontal scroll on mobile.
- Still optional: add LinkedIn/other profile URLs and a Netflix repo link when you have them.

## Photos
- Hero: black-blazer photo (right side, fades into dark on the left so text stays readable; stacked above the text on mobile).
- About: navy-blazer photo. The black-turtleneck photo is not used. Project logos unchanged.

## AI Integration photo
The "AI Integration" detail section (How I Build) now uses `assets/img/ai-integration.jpg` (ZolaKid workspace photo).
