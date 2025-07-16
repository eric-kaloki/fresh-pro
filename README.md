# Fresh Pro Website - Hosting Guide

This guide will help you host your Fresh Pro website on Vercel and connect it to your domain `freshpro.co.ke` purchased from NameCheap. No technical expertise required!

## What You'll Need

- Your Fresh Pro website files (you already have these)
- A GitHub account (free)
- A Vercel account (free)
- Access to your NameCheap account
- About 30 minutes of your time

## Step 1: Create a GitHub Account and Upload Your Website

### 1.1 Create GitHub Account
1. Go to [github.com](https://github.com)
2. Click "Sign up" in the top right corner
3. Choose a username, enter your email and create a password
4. Verify your email address when GitHub sends you a confirmation email

### 1.2 Create a New Repository
1. After logging in, click the green "New" button or the "+" icon in top right
2. Name your repository: `fresh-pro-website`
3. Make sure it's set to "Public"
4. Check the box "Add a README file"
5. Click "Create repository"

### 1.3 Upload Your Website Files
1. In your new repository, click "uploading an existing file"
2. Drag and drop ALL your website files (index.html and the images folder)
3. Scroll down and write a commit message like "Add Fresh Pro website files"
4. Click "Commit changes"

## Step 2: Create a Vercel Account and Deploy

### 2.1 Sign Up for Vercel
1. Go to [vercel.com](https://vercel.com)
2. Click "Sign Up"
3. Choose "Continue with GitHub" (this connects your accounts)
4. Authorize Vercel to access your GitHub account

### 2.2 Deploy Your Website
1. On your Vercel dashboard, click "New Project"
2. Find your `fresh-pro-website` repository and click "Import"
3. Leave all settings as default
4. Click "Deploy"
5. Wait 1-2 minutes for deployment to complete
6. You'll see a success message with a temporary URL like `fresh-pro-website.vercel.app`

## Step 3: Connect Your Custom Domain (freshpro.co.ke)

### 3.1 Add Domain in Vercel
1. In your Vercel project dashboard, click "Settings" tab
2. Click "Domains" in the left sidebar
3. Type `freshpro.co.ke` in the domain field
4. Click "Add"
5. Vercel will show you DNS records to add - KEEP THIS PAGE OPEN

### 3.2 Configure DNS in NameCheap
1. Open a new tab and go to [namecheap.com](https://namecheap.com)
2. Log into your NameCheap account
3. Go to "Domain List" and find `freshpro.co.ke`
4. Click "Manage" next to your domain
5. Click on "Advanced DNS" tab

### 3.3 Add DNS Records
You need to add these records exactly as shown:

**Record 1:**
- Type: `A Record`
- Host: `@`
- Value: `76.76.19.19`
- TTL: `Automatic`

**Record 2:**
- Type: `CNAME Record`
- Host: `www`
- Value: `cname.vercel-dns.com`
- TTL: `Automatic`

**Steps to add each record:**
1. Click "Add New Record"
2. Select the record type from dropdown
3. Enter the Host and Value exactly as shown above
4. Click the checkmark to save
5. Repeat for the second record

### 3.4 Remove Default Records (Important!)
1. Look for any existing A Records pointing to parking pages
2. Delete any A Records with values like `192.254.187.96` or similar
3. Keep only the DNS records you just added

## Step 4: Wait and Verify

### 4.1 DNS Propagation
- DNS changes take 5 minutes to 24 hours to work worldwide
- Usually works within 30 minutes
- You can check progress at [whatsmydns.net](https://whatsmydns.net)

### 4.2 SSL Certificate
- Vercel automatically creates a free SSL certificate
- Your site will be accessible via `https://freshpro.co.ke`
- This may take up to 24 hours to fully activate

## Step 5: Test Your Website

1. Wait at least 30 minutes after adding DNS records
2. Try visiting `https://freshpro.co.ke` in your browser
3. Try `https://www.freshpro.co.ke` as well
4. Both should show your Fresh Pro website

## Troubleshooting

### Website Not Loading?
- Wait longer (DNS can take up to 24 hours)
- Check DNS records are entered correctly in NameCheap
- Make sure you deleted any old/default DNS records

### "SSL Error" or "Not Secure"?
- Wait 24 hours for SSL certificate to activate
- Try accessing with `http://` instead of `https://` temporarily

### Still Having Issues?
- Contact Vercel support (they have excellent free support)
- Contact NameCheap support for DNS-related issues
- Double-check all DNS records are exactly as specified

## Future Updates

### To Update Your Website:
1. Make changes to your files on your computer
2. Go to your GitHub repository
3. Upload new files (same process as Step 1.3)
4. Vercel automatically deploys changes within 1-2 minutes

### Benefits of This Setup:
- ✅ Free hosting forever
- ✅ Automatic SSL certificate
- ✅ Fast global CDN
- ✅ Easy updates via GitHub
- ✅ 99.9% uptime
- ✅ Mobile-optimized delivery

## Important Notes

- Keep your GitHub and Vercel accounts secure
- Your website files are backed up on GitHub
- Vercel provides free bandwidth for personal/small business use
- Your domain renewal with NameCheap is separate from hosting

## Contact Support

- **Vercel Support**: [vercel.com/support](https://vercel.com/support)
- **NameCheap Support**: [namecheap.com/support](https://namecheap.com/support)
- **GitHub Help**: [help.github.com](https://help.github.com)

---

**Congratulations!** Once complete, your Fresh Pro website will be live at `https://freshpro.co.ke` 🎉



---
## 📋 Optional Enhancements (Future Considerations):
### If you want to expand later, you could consider:

- Contact form/page
- About us section
- Product gallery
- Blog/news section
- Customer testimonials
- Social media links

---
*Last updated: 16th July 2025*