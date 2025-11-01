# Field Questionnaire - Netlify Deployment

A beautiful, interactive questionnaire built with HTML/CSS and deployed on Netlify with form handling.

## Features

- Clean, modern design with smooth animations
- Netlify Forms integration for automatic form handling
- Responsive design that works on all devices
- Auto-deployment from GitHub
- Custom thank-you page after submission

## Project Structure

```
questionnaire-netlify/
├── index.html          # Main questionnaire page
├── thank-you.html      # Success page after form submission
├── netlify.toml        # Netlify configuration
└── README.md           # This file
```

## Customizing the Questions

To update the questionnaire with your questions, edit `index.html`:

1. **Update the header:**
   - Change the title and subtitle in the `.header` section

2. **Update the purpose section:**
   - Modify the purpose text and instructions

3. **Update each question:**
   - Find each `.question-group` div
   - Update the question text in the `.question` element
   - Update the explanation in the `.question-explanation` element
   - Update the example responses in the `.examples` section
   - Update the textarea placeholder

4. **Update the closing section:**
   - Modify the closing reflection text

5. **Add or remove questions:**
   - Copy a complete `.question-group` div to add a new question
   - Remember to update the question number and form field name (e.g., `name="question7"`)

## Deploying to Netlify

### Option 1: Deploy from GitHub (Recommended)

1. **Push this repository to GitHub** (if not already done)

2. **Connect to Netlify:**
   - Go to [Netlify](https://app.netlify.com/)
   - Click "Add new site" > "Import an existing project"
   - Choose "GitHub" and select this repository
   - Netlify will auto-detect the settings from `netlify.toml`
   - Click "Deploy site"

3. **Auto-deployment is now active:**
   - Every push to your GitHub repository will automatically deploy to Netlify
   - You'll get a live URL (e.g., `https://your-site-name.netlify.app`)

### Option 2: Deploy via Netlify CLI

```bash
# Install Netlify CLI (if not already installed)
npm install -g netlify-cli

# Login to Netlify
netlify login

# Deploy
netlify deploy --prod
```

### Option 3: Drag and Drop

1. Go to [Netlify Drop](https://app.netlify.com/drop)
2. Drag the entire project folder
3. Your site will be live instantly

## Viewing Form Submissions

After deploying to Netlify:

1. Go to your Netlify dashboard
2. Select your site
3. Click on "Forms" in the top navigation
4. All form submissions will appear here
5. You can set up email notifications for new submissions in the form settings

## Environment Setup

No build process or dependencies required - this is a static HTML site!

## License

MIT

## Support

For Netlify-specific issues, check the [Netlify documentation](https://docs.netlify.com/).
