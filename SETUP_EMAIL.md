# Email Setup Instructions

## How to Receive Assessment Results via Email

Your coaching assessment now includes a form that captures user information and emails the results to you. Here's how to set it up:

### Step 1: Update Your Email Address

1. Open `app.js`
2. Find line 373: `form.action = "https://formsubmit.co/your-email@example.com";`
3. Replace `your-email@example.com` with your actual email address
4. Save the file

Example:
```javascript
form.action = "https://formsubmit.co/lindsay.kloepping@3pillarglobal.com";
```

### Step 2: Verify Your Email (First Time Only)

The first time someone submits the form:

1. FormSubmit will send a **verification email** to your address
2. Click the confirmation link in that email
3. After confirmation, all future submissions will be delivered automatically

### Step 3: What You'll Receive

Each submission will include:

- **First Name**
- **Last Name**
- **Email Address** (of the person taking the assessment)
- **Total Score** (e.g., "92 / 125")
- **Classification** (e.g., "Coachable with Guidance")
- **Dimension Scores** (all 5 dimension averages)

### Email Example:

```
Subject: New Coaching Assessment Results

First Name: John
Last Name: Doe
Email: john.doe@example.com
Total Score: 92 / 125
Classification: Coachable with Guidance
Dimension Scores: Readiness: 4.20, Willingness: 3.80, Realistic: 4.00, Self-Awareness: 3.40, Commitment: 3.60
```

### Alternative Options

If you prefer a different solution:

#### Option 1: Google Sheets Integration
- Use Google Forms integration
- Submissions go directly to a Google Sheet
- Easy to review and export

#### Option 2: EmailJS
- More customizable email templates
- Professional-looking emails
- Requires free EmailJS account

#### Option 3: Backend Database
- Create a simple backend API
- Store in database (Firebase, Supabase, etc.)
- More control over data

Let me know if you'd like help setting up any of these alternatives!

### Notes

- FormSubmit is **free** for unlimited submissions
- No backend server required
- GDPR compliant
- User gets redirected back to results page after submission
- No CAPTCHA needed (disabled for better UX)

### Troubleshooting

**Problem:** Not receiving emails  
**Solution:** Check spam folder, verify email confirmation was completed

**Problem:** Want to change email address  
**Solution:** Update line 373 in app.js and verify new email

**Problem:** Want custom email template  
**Solution:** Consider switching to EmailJS for more customization

