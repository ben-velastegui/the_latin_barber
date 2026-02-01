# The Latin Barber - Website Setup Guide

## 📧 Email Notification Setup (FREE)

Your booking system will send email notifications to: **Benjamin.s.v.lopez@gmail.com**

### Step-by-Step EmailJS Setup:

1. **Create Free EmailJS Account**
   - Go to https://www.emailjs.com
   - Click "Sign Up" and create a free account
   - The free tier includes 200 emails/month (perfect for a barbershop!)

2. **Add Email Service**
   - After logging in, click "Email Services"
   - Click "Add New Service"
   - Select "Gmail" (recommended)
   - Click "Connect Account" and sign in with Benjamin.s.v.lopez@gmail.com
   - Give it a name like "Barbershop Gmail"
   - Copy the **Service ID** (e.g., "service_abc123")

3. **Create Email Template**
   - Click "Email Templates" in the sidebar
   - Click "Create New Template"
   - Use this template:

   **Template Name:** Barbershop Booking Notification
   
   **Subject:** New Booking: {{customer_name}} - {{service_name}}
   
   **Content:**
   ```
   NEW BOOKING RECEIVED
   
   Service: {{service_name}}
   Date: {{date}}
   Time: {{time}}
   Duration: {{duration}} minutes
   Price: {{price}}
   
   CUSTOMER DETAILS:
   Name: {{customer_name}}
   Phone: {{customer_phone}}
   Email: {{customer_email}}
   
   Special Requests:
   {{notes}}
   
   ---
   This is an automated notification from your booking system.
   ```

   - Click "Save"
   - Copy the **Template ID** (e.g., "template_xyz789")

4. **Get Your Public Key**
   - Click "Account" in the sidebar
   - Find your **Public Key** (e.g., "abc123XYZ")

5. **Update booking.html**
   - Open `booking.html` in a text editor
   - Find lines 830-832 (search for "YOUR_PUBLIC_KEY_HERE")
   - Replace with your actual values:
   
   ```javascript
   const EMAILJS_PUBLIC_KEY = 'your_actual_public_key';
   const EMAILJS_SERVICE_ID = 'your_actual_service_id';
   const EMAILJS_TEMPLATE_ID = 'your_actual_template_id';
   ```

6. **Test It!**
   - Open your website
   - Make a test booking
   - Check Benjamin.s.v.lopez@gmail.com for the notification email

---

## 📸 Gallery Image Setup

### Option 1: Using Free Image Hosting (Recommended)

**Using Imgur (Free, Easy):**

1. Go to https://imgur.com
2. Click "New post"
3. Upload your barbershop photos
4. Right-click each image → "Copy image address"
5. Paste the URL into the `galleryImages` array in `gallery.html`

**Using ImgBB (Free, No Account Required):**

1. Go to https://imgbb.com
2. Upload your images
3. Copy the "Direct link"
4. Paste into the `galleryImages` array

### Option 2: Download from Instagram

1. Go to your Instagram (@thelatinbarber_)
2. Use a tool like https://inflact.com/downloader/instagram/photo/ to download your posts
3. Upload downloaded images to Imgur or ImgBB
4. Add the URLs to your gallery

### How to Update the Gallery:

1. Open `gallery.html` in a text editor
2. Find the `galleryImages` array (around line 310)
3. Replace the placeholder URLs with your actual image URLs:

```javascript
const galleryImages = [
    {
        url: 'https://i.imgur.com/YOUR_IMAGE_1.jpg',
        alt: 'Fresh fade haircut'
    },
    {
        url: 'https://i.imgur.com/YOUR_IMAGE_2.jpg',
        alt: 'Skin fade with beard trim'
    },
    // Add more images...
];
```

4. Save the file and upload to your website

---

## 🚀 Uploading to Your Website

### If using a hosting service (GoDaddy, Bluehost, etc.):

1. Log into your hosting control panel
2. Use File Manager or FTP to upload:
   - `index.html`
   - `booking.html`
   - `gallery.html`
3. Make sure they're in your public_html or www folder

### If using GitHub Pages (Free):

1. Create a GitHub account at https://github.com
2. Create a new repository named `thelatinbarber.github.io`
3. Upload all HTML files
4. Your site will be live at: https://thelatinbarber.github.io

---

## ✅ Testing Checklist

- [ ] EmailJS account created
- [ ] Email service connected to Benjamin.s.v.lopez@gmail.com
- [ ] Email template created with correct variables
- [ ] Public Key, Service ID, and Template ID added to booking.html
- [ ] Test booking made and email received
- [ ] Gallery images uploaded to image hosting
- [ ] Gallery URLs updated in gallery.html
- [ ] Website files uploaded to hosting

---

## 🆘 Troubleshooting

**Email not sending?**
- Check that your Public Key, Service ID, and Template ID are correct
- Make sure the EmailJS service is connected to the right Gmail account
- Check browser console for errors (F12 → Console tab)

**Images not showing?**
- Make sure you're using direct image links (ending in .jpg, .png, etc.)
- Check that the image URLs are publicly accessible
- Try opening the image URL in a new browser tab to verify it works

**Need more help?**
- EmailJS Documentation: https://www.emailjs.com/docs/
- Contact me through the website or at Benjamin.s.v.lopez@gmail.com

---

## 💡 Tips

- Update your gallery weekly with new cuts to keep content fresh
- Respond to booking emails within 24 hours
- Consider adding more services to the booking form as you expand
- Share your gallery page on Instagram stories to drive traffic

Good luck with The Latin Barber! 💈✂️
