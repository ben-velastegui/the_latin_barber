# The Latin Barber - Website Files

## 📁 What's Included

Your complete multi-page website with:

- **index.html** - Homepage with hero section and service preview
- **services.html** - Detailed services page with all offerings
- **booking.html** - Fully functional booking system (FIXED!)
- **gallery.html** - Photo gallery showcase
- **contact.html** - Contact information and hours

## ✨ Design Features

- **Apple-inspired minimalist design**
- Clean, sleek UI with refined typography
- Smooth transitions and subtle animations
- Fully responsive (mobile, tablet, desktop)
- Professional black, white, and gold color scheme
- No cringe copy - clean, professional language

## 🚀 Quick Start

### Option 1: Test Locally
1. Download all 5 HTML files
2. Put them in the same folder
3. Double-click `index.html` to open in your browser
4. Navigate between pages using the menu

### Option 2: Deploy to Web
Upload to any hosting service:

**Free Options:**
- **Netlify** - Drag & drop deployment (recommended)
- **Vercel** - Free hosting with custom domain
- **GitHub Pages** - Version control + hosting

## 🎯 Working Booking System

The booking system is now **fully functional** with:

✅ 4-step booking process
✅ Service selection with pricing
✅ Date picker (prevents past dates)
✅ Time slot selection
✅ Blocked/booked slot management
✅ Customer information capture
✅ Booking summary and confirmation
✅ Form validation at each step

### How It Works:

1. **Step 1:** Customer selects service (Classic Fade, Skin Fade, etc.)
2. **Step 2:** Picks date and sees available time slots
3. **Step 3:** Enters name, phone, email
4. **Step 4:** Reviews booking and confirms
5. **Success:** Confirmation page with booking details

## 🔧 Customization

### Add Your Photos to Gallery

In `gallery.html`, replace:
```html
<div class="gallery-placeholder">✂️</div>
```

With:
```html
<img src="your-photo.jpg" alt="Haircut" style="width: 100%; height: 100%; object-fit: cover;">
```

### Add Google Maps

In `contact.html`, replace the map placeholder with:
```html
<iframe 
    src="https://www.google.com/maps/embed?pb=YOUR_EMBED_CODE"
    width="100%" 
    height="500" 
    style="border:0;" 
    allowfullscreen="" 
    loading="lazy">
</iframe>
```

Get your embed code: Google Maps → Share → Embed a map

### Update Contact Info

Search and replace in all files:
- `+441234567890` → Your phone number
- `info@thelatinbarber.com` → Your email
- Update business hours if different

### Change Colors

In any HTML file's `<style>` section, modify:
```css
:root {
    --primary: #1d1d1f;    /* Main dark color */
    --accent: #C9A961;      /* Gold accent */
    --secondary: #f5f5f7;   /* Light background */
}
```

## 📱 Making Bookings Live

Currently, bookings are saved locally (demo mode). To make it production-ready:

### Option 1: Calendly (Easiest - $0-8/month)

1. Create account at https://calendly.com
2. Set up your services with pricing
3. Replace the booking form with Calendly embed
4. Automatic email/SMS confirmations

### Option 2: Square Appointments (Professional)

1. Sign up at https://squareup.com/appointments
2. Add services and pricing
3. Take payments online
4. Built-in calendar and SMS

### Option 3: Custom Backend

Build your own with:
- **Backend:** Node.js, Python, or PHP
- **Database:** Firebase, MongoDB, PostgreSQL
- **SMS/WhatsApp:** Twilio API
- **Calendar:** Google Calendar API

See INTEGRATION_GUIDE.md for detailed instructions.

## 🎨 Design Philosophy

This site uses **refined minimalism** inspired by Apple:

- Generous white space
- Subtle animations
- Clean typography (-apple-system font stack)
- Consistent spacing and alignment
- Professional, understated elegance
- Mobile-first responsive design

## 📊 Browser Support

Works on all modern browsers:
- Chrome, Safari, Firefox, Edge
- iOS Safari, Chrome Mobile
- Tablet and desktop layouts

## 🔍 SEO Ready

Add to `<head>` of each page:
```html
<meta name="description" content="Professional barbering in Newcastle & Gateshead">
<meta name="keywords" content="barber Newcastle, fade haircut, beard trim">
```

## 📈 Next Steps

**Week 1:**
- [ ] Test all pages locally
- [ ] Add your real photos to gallery
- [ ] Update contact information
- [ ] Test booking flow

**Week 2:**
- [ ] Deploy to web hosting
- [ ] Set up Calendly or booking system
- [ ] Add Google Maps embed
- [ ] Connect social media

**Week 3:**
- [ ] Set up Google Business Profile
- [ ] Create Instagram integration
- [ ] Test on multiple devices
- [ ] Launch!

## 💡 Pro Tips

1. **Compress Images:** Use TinyPNG before uploading photos
2. **Custom Domain:** Buy yourname.com for $10/year
3. **SSL Certificate:** Free with Netlify/Vercel
4. **Analytics:** Add Google Analytics to track visitors
5. **Mobile Test:** Check on real phones, not just browser resize

## 🆘 Troubleshooting

**Booking not working?**
- Open browser console (F12) to check for errors
- Make sure all files are in same folder
- Verify date field allows future dates

**Pages not linking?**
- Check all files are named exactly: index.html, services.html, etc.
- Files must be in the same directory

**Styles broken?**
- Make sure you're opening the HTML file (not the code)
- Try a different browser
- Clear cache (Ctrl+Shift+R)

## 📞 Support Resources

- **Hosting Help:** https://docs.netlify.com
- **Calendly Setup:** https://help.calendly.com
- **Google Maps:** https://developers.google.com/maps

---

**Built with precision. Ready to launch.** 🚀
