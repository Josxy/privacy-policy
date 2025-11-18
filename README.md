# Privacy Policy Page

This folder contains the privacy policy page for the Yes! platform, designed to be deployed via GitHub Pages.

## Setup GitHub Pages

### Option 1: Deploy from Branch (Recommended)

1. Go to your GitHub repository settings
2. Navigate to **Settings** > **Pages**
3. Under "Build and deployment":
   - Source: Select "Deploy from a branch"
   - Branch: Select your main branch (e.g., `v1.0-main` or `main`)
   - Folder: Select `/ (root)`
4. Click **Save**
5. Your privacy policy will be available at:
   ```
   https://[your-username].github.io/[repo-name]/privacy-policy/
   ```

### Option 2: Deploy from Specific Folder

1. Go to **Settings** > **Pages**
2. Source: Select "Deploy from a branch"
3. Branch: Select your branch and choose `/docs` folder (you'll need to rename `privacy-policy` to `docs`)
4. This will deploy only the contents of that folder

## Customization Checklist

Before deploying, update the following placeholders in `index.html`:

- [ ] **Effective Date**: Replace `[INSERT DATE]` with the current date (e.g., January 18, 2025)
- [ ] **Company Name**: Replace `[COMPANY NAME]` with your company/developer name
- [ ] **Contact Email**: Replace `[YOUR-EMAIL]` with your support email
- [ ] **Website URL**: Replace `[YOUR-WEBSITE]` with your website URL

### Additional Customizations (Optional)

Consider updating these sections based on your specific setup:

1. **Third-Party Services**: Add specific services you use:
   - Supabase (authentication and database)
   - AWS S3 (game file storage)
   - Any analytics services (Google Analytics, etc.)

2. **Data Collection**: Be specific about what data you collect:
   - Game play metrics (duration, interactions)
   - User preferences and likes
   - Comments and ratings

3. **GDPR/CCPA Compliance**: If targeting EU or California users, add specific clauses for:
   - Right to be forgotten
   - Data portability
   - Opt-out mechanisms

## Testing Locally

To test the page locally before deploying:

```bash
# Using Python 3
cd privacy-policy
python -m http.server 8000

# Then open: http://localhost:8000
```

Or simply open `index.html` directly in your browser.

## Linking from Your App

Once deployed, add the privacy policy link to:

- **Mobile App**: Settings/Profile page
- **Studio**: Footer or account settings
- **Login/Signup**: Link during account creation

Example link format:
```
https://[your-username].github.io/Wally/privacy-policy/
```

## Legal Disclaimer

This is a general template and may not cover all legal requirements for your specific use case or jurisdiction. Consider consulting with a legal professional to ensure compliance with applicable privacy laws such as GDPR, CCPA, COPPA, etc.

## Updates

When updating the privacy policy:
1. Update the "Effective Date" at the top
2. Consider notifying users of significant changes
3. Keep a backup of previous versions for record-keeping
