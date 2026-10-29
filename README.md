# PlateCount

Landing page for **PlateCount** (working name), an app that turns event RSVPs into a realistic headcount so organisers order the right amount of food.

> 200 guests confirm, 150 show up, and 50 plates go to waste. PlateCount closes that gap.

## What is on the page

- Hero with an animated sample dashboard
- Problem section with a confirmed vs arrived visual
- How it works (4 interactive steps)
- Feature overview
- Working demo dashboard with sample data and adjustable show-up rates
- Attendance and catering calculator
- Early-access signup form (front end only)

All numbers on the page are sample data or user-set assumptions, not measured statistics.

## Run locally

No build step. Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy with GitHub Pages

1. Push this folder to a GitHub repository.
2. Go to **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. Your site appears at `https://<your-username>.github.io/<repo-name>/` after a minute or two.

## Connect the signup form

The form validates the email and shows a thank-you message but does not store anything yet. In `index.html`, find the `TODO` comment in the signup handler and send `{ email, role }` to your backend or a form service such as Formspree, Google Forms or Netlify Forms.

## Project structure

```
index.html   # the whole site (HTML, CSS and JavaScript)
README.md
.gitignore
.nojekyll    # tells GitHub Pages to serve the files as they are
```

## Notes

- Fonts (Manrope, Inter) load from Google Fonts.
- The name PlateCount is a placeholder. Check availability before registering a domain or trademark.
- Add a `LICENSE` file of your choice before making the repository public.
