# 🚀 Quick Start Guide - MJC SECURITY Website

Get your professional VAPT website live in minutes!

## Step 1: Add Your Photo (2 minutes)

1. Prepare your professional headshot photo (JPG or PNG)
2. Save it as `founder-photo.jpg` in the root directory
3. The website will automatically display it on the Team section

## Step 2: Update Contact Information (3 minutes)

### Email
Replace all instances of `singhjc083@gmail.com` with your email:
- In the Team section
- In the Contact section (Email link)
- In the footer (optional)

### LinkedIn
Update your LinkedIn URL from:
```
https://www.linkedin.com/in/jagat-singh-b824701b8/
```
To:
```
https://www.linkedin.com/in/your-profile/
```

### Phone (Optional)
Add your phone number in the Contact section:
```html
<div class="info-item">
    <i class="fas fa-phone"></i>
    <div>
        <h4>Phone</h4>
        <p>+91-XXXXX-XXXXX</p>
    </div>
</div>
```

## Step 3: Customize Your Services (5 minutes)

Edit the services in the Services section to match your offerings:

```html
<div class="service-card">
    <i class="fas fa-shield-alt"></i>
    <h3>Your Service Name</h3>
    <p>Your detailed service description</p>
</div>
```

**Current Services:**
1. Vulnerability Assessment
2. Penetration Testing
3. Web Application Penetration Testing
4. Cyber Forensics & Investigation
5. Network Security Testing
6. Security Compliance Audit

## Step 4: Add Your Case Studies (10 minutes)

Replace the portfolio section with your actual projects:

```html
<div class="case-study">
    <div class="case-icon">
        <i class="fas fa-bank"></i>  <!-- Change icon as needed -->
    </div>
    <h3>Your Project Title</h3>
    <p><strong>Client:</strong> Client Name (or "Confidential")<br>
    <strong>Scope:</strong> What you tested<br>
    <strong>Result:</strong> What you found/fixed</p>
</div>
```

**Available Icons:**
- `fa-bank` - Financial
- `fa-hospital` - Healthcare
- `fa-shopping-cart` - E-commerce
- `fa-building` - Enterprise
- `fa-laptop` - Technology
- `fa-lock` - Security

## Step 5: Update Your Credentials (3 minutes)

Edit the Team section to highlight your achievements:

```html
<div class="credentials">
    <span class="badge badge-critical">Your Critical Achievement</span>
    <span class="badge badge-gold">Your Recognition</span>
</div>
```

**Current Credentials:**
- CVE-2023-43187 (CRITICAL 9.8) - Badge color: `badge-critical`
- Top 15 Researcher - NCIIPC India - Badge color: `badge-gold`

## Step 6: Deploy to GitHub Pages (2 minutes)

### One-time Setup:
1. Go to your GitHub repo: `https://github.com/jagat-singh-chaudhary/MJCSECURITY`
2. Click **Settings** → **Pages**
3. Under "Source", select **Deploy from a branch**
4. Choose **main** branch and **/root** folder
5. Click **Save**

### Every Time You Update:
```bash
git add .
git commit -m "Update website content"
git push origin main
```

Your website will be live at:
```
https://jagat-singh-chaudhary.github.io/MJCSECURITY/
```

## Pro Tips ⭐

### 1. Make it SEO Friendly
- Update the `<title>` tag in index.html
- Add your company name and keywords
- Update social media links in footer

### 2. Setup Contact Form
Currently, the contact form shows an alert. To save submissions:

**Option A: Use Formspree (Free)**
1. Go to https://formspree.io/
2. Create account and set up your form
3. Replace the form submission code in `script.js`

**Option B: Use SendGrid**
1. Sign up for free tier
2. Set up API integration
3. Handle form submissions on backend

### 3. Add Google Analytics
Add this to `<head>` section of index.html:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

Replace `GA_MEASUREMENT_ID` with your tracking ID.

### 4. Add Blog Posts
Add new articles in the Blog section:
```html
<article class="blog-card">
    <h3>Understanding OWASP Top 10</h3>
    <p class="date">April 23, 2026</p>
    <p>Your blog excerpt here...</p>
    <a href="/blog/your-post.html" class="read-more">Read More →</a>
</article>
```

### 5. Customize Colors
Edit `:root` variables in `styles.css`:
```css
:root {
    --primary-color: #0066cc;    /* Change to your brand color */
    --secondary-color: #ff6600;  /* Change accent color */
    --text-dark: #1a1a1a;        /* Change text color */
}
```

## Common Issues & Solutions

### Photo Not Showing?
- ✅ Make sure file is named exactly `founder-photo.jpg`
- ✅ File is in the root directory (same folder as index.html)
- ✅ Refresh the page (Ctrl+F5 or Cmd+Shift+R)

### Links Not Working?
- ✅ Check email addresses (singhjc083@gmail.com)
- ✅ Verify LinkedIn URL format
- ✅ Test on different browsers

### Website Not Updating?
- ✅ Hard refresh: Ctrl+Shift+Delete (clear cache)
- ✅ Wait 2-3 minutes for GitHub Pages to rebuild
- ✅ Check GitHub Actions to see build status

### Mobile Menu Not Working?
- ✅ Make sure `script.js` is loaded correctly
- ✅ Check browser console for errors (F12)
- ✅ Ensure JavaScript is enabled

## Performance Optimization

1. **Compress Images**
   - Optimize your photo to under 500KB
   - Use JPG or WebP format

2. **Cache Control**
   - GitHub Pages automatically caches assets
   - Add `cache-busting` if files don't update

3. **Minify Code** (Optional)
   - Use online tools to minify CSS/JS
   - Can improve load time by 20-30%

## Security Tips

1. ✅ Never commit sensitive information (API keys, passwords)
2. ✅ Use HTTPS (automatically enabled on GitHub Pages)
3. ✅ Keep contact form data secure (use Formspree or SendGrid)
4. ✅ Validate all form inputs before processing

## Support & Resources

- 📖 **GitHub Pages Docs**: https://pages.github.com/
- 🎨 **Font Awesome Icons**: https://fontawesome.com/icons
- 🎯 **Color Picker**: https://coolors.co/
- 📱 **Responsive Test**: https://responsively.app/

## Next Level Improvements

1. **Add Subdomain**
   - Buy custom domain (Namecheap, GoDaddy)
   - Point to GitHub Pages (see documentation)

2. **Add HTTPS Certificate**
   - Enable in GitHub Pages settings
   - GitHub provides free SSL/TLS

3. **Add Comments Section**
   - Integrate Disqus or Utterances
   - Allow client feedback

4. **Add Dark Mode**
   - Add CSS dark theme toggle
   - Improve user experience

5. **Add Email Newsletter**
   - Use Mailchimp for email list
   - Grow your audience

---

## 🎉 You're All Set!

Your professional VAPT website is now live and ready to attract clients!

**Checklist:**
- [ ] Photo added
- [ ] Email updated
- [ ] LinkedIn URL updated
- [ ] Services customized
- [ ] Case studies added
- [ ] Deployed to GitHub Pages
- [ ] Website tested on mobile
- [ ] Shared with colleagues

**Share your website:**
```
https://jagat-singh-chaudhary.github.io/MJCSECURITY/
```

**Questions?** Contact: singhjc083@gmail.com

Happy promoting! 🚀