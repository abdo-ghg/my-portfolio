# 🌐 Abdelrahman Bakr Ghazy — Portfolio

Personal portfolio site showcasing work and skills in **Computer Science**, **Artificial Intelligence**, and **Data Science**.  
Includes Education, Experience, Projects, Tools, Recommendations and Contact. Built with plain **HTML / CSS / JavaScript** and optimized for fast static deploys.

---

## 🚀 Live demo
Replace with your real URL after deploy:  
`https://your-username.github.io/my-portfolio/`

---

## 📂 Project structure
```
my-portfolio/
├─ index.html        # Main website
├─ styles.css        # Global styles (or inline styles if used)
├─ script.js         # JS: animations, modals, form handling
├─ photos/           # All images used (replace with your links)
└─ README.md         # This file
```

---

## ⚙️ Quick local preview
1. Clone the repo:
```bash
git clone https://github.com/YOUR-USERNAME/my-portfolio.git
cd my-portfolio
```
2. Open locally:
- Double-click `index.html` OR
- Serve via a simple static server (recommended):
```bash
# Python 3
python -m http.server 3000
# then open http://localhost:3000
```

---

## ✅ What to edit (fast)
- `index.html` — main content (hero, about, education, projects, contact).
- `styles.css` — theme colors, spacing, typography.
- `script.js` — animations, contact form logic, modal behavior.
- `photos/` — replace placeholder images; update `<img src="photos/your.jpg">` in HTML.

**Tips**
- Use consistent filenames (no spaces).
- If hosting images externally, use absolute URLs.
- Keep important text in `index.html` so recruiters can find it fast.

---

## ✉️ Contact form (Email delivery) — EmailJS (no backend)
If you want messages sent to your email automatically, use **EmailJS** (no server required).

### Steps (EmailJS)
1. Create an account at https://www.emailjs.com  
2. Add an Email Service (e.g., link your Gmail or SMTP) → copy the **Service ID** (e.g., `service_xxx`).  
3. Create an **Email Template** (HTML content). Use these variables that match the form:
   - `from_name`
   - `from_email`
   - `subject`
   - `message`
   - `phone` (optional)
   - `time`
   - `page_url`
   - `user_agent`  
4. Copy your **Template ID** (e.g., `template_xxx`) and **Public Key** (API key).

### Update your site JS
Replace placeholders with your real keys:
```js
emailjs.init("YOUR_PUBLIC_KEY"); // replace

// on form submit
emailjs.sendForm("YOUR_SERVICE_ID", "YOUR_TEMPLATE_ID", "#contact-form")
  .then(() => { /* success */ })
  .catch(err => { /* handle error */ });
```

### Recommended EmailJS template (HTML)
Use this HTML in the EmailJS template editor (it matches the form field names used in the site):
```html
<div style="font-family: system-ui, sans-serif, Arial; font-size: 14px; color: #2c3e50;">
  <div style="margin-bottom: 15px;">
    <strong>📩 New message received from your portfolio website</strong>
  </div>

  <div style="margin: 15px 0; padding: 15px; border: 1px dashed lightgrey; border-radius: 6px; background: #f9f9f9;">
    <table role="presentation" width="100%">
      <tr>
        <td style="vertical-align: top; padding-right: 12px;">
          <div style="font-size: 28px;">👤</div>
        </td>
        <td style="vertical-align: top;">
          <div style="font-size: 16px; font-weight: bold;">{{from_name}}</div>
          <div style="color: #888; font-size: 13px;">✉️ {{from_email}}</div>
          <div style="color: #888; font-size: 13px;">📞 {{phone}}</div>
          <div style="margin-top: 8px; font-size: 15px;"><b>Subject:</b> {{subject}}</div>
        </td>
      </tr>
    </table>
  </div>

  <div style="margin: 15px 0; padding: 15px; border: 1px solid #eee; border-radius: 6px; background: #fff;">
    <div style="font-size: 15px; line-height: 1.6; white-space: pre-wrap;">{{message}}</div>
  </div>

  <div style="margin-top: 20px; font-size: 12px; color: #777;">
    <p>🕒 Sent at: {{time}}</p>
    <p>🔗 Page: {{page_url}}</p>
    <p>💻 Browser: {{user_agent}}</p>
  </div>
</div>
```

### Test
- Submit the form on your site and check `abdoghaz079@gmail.com`.  
- If messages go to Spam, mark “Not spam” and consider adjusting template subject text.

---

## 📦 Deploy (recommended options)

### GitHub Pages (fast, free)
1. Push to GitHub `main` branch:
```bash
git add .
git commit -m "deploy"
git push origin main
```
2. On GitHub → **Settings** → **Pages** → Source: `main` / root → Save.  
3. Visit `https://YOUR-USERNAME.github.io/REPO-NAME/` after a minute.

### Netlify (drag & drop or repo link)
- Drag & drop your site folder on Netlify dashboard OR connect repo for CI/CD.
- Netlify gives instant URL + SSL.

### Vercel
- Connect your GitHub repo, deploy. Good if you plan to expand later.

---

## 🔧 Maintenance & tips
- Replace placeholders: `YOUR_MAIN_PHOTO_LINK`, `PROJECT_IMG_LINK_*`, `EXP_IMG_LINK_*`.  
- Optimize images (WebP/PNG compression) for performance.  
- Add Google Fonts `<link>` in `<head>` if you use custom fonts.  
- Accessibility: include descriptive `alt` for images, semantic HTML.  
- SEO: update `<title>`, `<meta name="description">`, and add Open Graph tags.

---

## 🧾 License
This project is released under the **MIT License**.

```
MIT License

Copyright (c) 2025 Abdelrahman Bakr Ghazy

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 📞 Contact
- **Email:** abdoghaz079@gmail.com  
- **Phone:** +20 101 791 5206  
- **LinkedIn:** https://www.linkedin.com/in/abdelrahman-bakr-ghazy-34737629a/  
- **GitHub:** https://github.com/abdo-ghg

---

If you want, I can push this `README.md` to your repository for you — give me the repo URL and I’ll provide the exact `git` commands to run locally.
