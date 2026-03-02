# Step 9: Deploy a Temporary GitHub Pages Test Site

## Goal
Deploy a simple temporary page so you can verify your full publish workflow before starting your real project.

## Instructions
1. In your local `project-setup` repo, create/update these files at the project root:
   - `index.html`
   - `style.css`
2. Use the starter content from this tutorial's `index.html` and `style.css` files (or the code blocks below).
3. Commit and push both files.
4. On GitHub, open your `project-setup` repo -> **Settings** -> **Pages**.
5. Under Source, choose `Deploy from a branch`, branch `main`, folder `/ (root)`, then save.
6. Wait a few minutes, then open the generated URL.
7. Confirm the live page says this is a temporary deployment demo.

Optional starter HTML:
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Setup Complete - Temporary Deployment</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <main class="wrap">
    <h1>Congratulations. You completed the setup tutorial.</h1>
    <p>
      This is a temporary file used to demonstrate the GitHub Pages deployment process.
      Next, you can replace this with your actual project files.
    </p>
  </main>
</body>
</html>
```

Optional starter CSS:
```css
body {
  margin: 0;
  font-family: "Segoe UI", Tahoma, sans-serif;
  background: #f4f6fb;
  color: #1f2937;
}

.wrap {
  max-width: 760px;
  margin: 10vh auto;
  background: #ffffff;
  border: 1px solid #dbe2ea;
  border-radius: 12px;
  padding: 2rem;
}

h1 {
  margin-top: 0;
}
```

## Checklist
- [ ] I added `index.html` and `style.css` to my setup repo.
- [ ] I pushed both files to GitHub.
- [ ] I enabled GitHub Pages.
- [ ] I opened my live temporary deployment URL.
