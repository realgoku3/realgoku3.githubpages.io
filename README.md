# thisrules.fyi

Personal blog — currently under construction. 🚧

Live site: [https://thisrules.fyi](https://thisrules.fyi)

## Deploy to GitHub Pages

1. Create a new repo on GitHub (e.g. `thisrules-fyi`).
2. Push this folder to the repo:

   ```bash
   git init
   git add .
   git commit -m "Initial commit: under construction homepage"
   git branch -M main
   git remote add origin git@github.com:YOUR_USERNAME/thisrules-fyi.git
   git push -u origin main
   ```

3. In the repo on GitHub, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
5. Choose branch **main** and folder **/ (root)**, then save.
6. Wait a minute or two — your site will be at `https://YOUR_USERNAME.github.io/thisrules-fyi/`.

## Custom domain (thisrules.fyi)

This repo includes a `CNAME` file for the custom domain. After enabling Pages:

1. In **Settings → Pages → Custom domain**, enter `thisrules.fyi` and save.
2. At your DNS provider, add these records:

   | Type  | Name | Value              |
   |-------|------|--------------------|
   | A     | @    | 185.199.108.153    |
   | A     | @    | 185.199.109.153    |
   | A     | @    | 185.199.110.153    |
   | A     | @    | 185.199.111.153    |
   | CNAME | www  | YOUR_USERNAME.github.io |

3. Enable **Enforce HTTPS** once DNS verifies.

## Local preview

Open `index.html` in a browser, or serve it locally:

```bash
python3 -m http.server 8080
# visit http://localhost:8080
```

## Structure

```
.
├── CNAME       # Custom domain for GitHub Pages
├── index.html  # Homepage
└── README.md   # This file
```
