# Coaching Assessment Tool

A comprehensive 5-page assessment tool designed for coaching and professional development. Features a modern single-page web application with a cover page, 5 assessment sections (10 questions each), and detailed results with radar chart visualization.

## Features

- **5 Assessment Dimensions**: Problem Discovery, Growth & Learning, Collaboration & Agility, Execution & Delivery, and Stakeholder & Insight Orientation
- **Interactive Rating Scale**: 0-5 Likert scale for each question
- **Progress Tracking**: Visual progress indicator and navigation between sections
- **Detailed Results**: Radar chart visualization with comprehensive analysis
- **Export Options**: Download results as PNG chart or CSV data
- **Responsive Design**: Works on desktop and mobile devices
- **Local Storage**: Progress automatically saved in browser

## Quick Start

### Option 1: Direct Browser
Open `index.html` in a modern browser. No build step required.

### Option 2: Local Development Server
```bash
# Install dependencies
npm install

# Start development server
npm run dev
# or
npm start
```

The app will be available at `http://localhost:3000`

## Development

### Project Structure
```
├── index.html          # Main HTML file
├── app.js              # Core application logic
├── questions.js        # Assessment questions and labels
├── analysis.js         # Analysis data for results
├── styles.css          # Styling and CSS variables
├── package.json        # Project configuration
├── vercel.json         # Vercel deployment config
└── netlify.toml        # Netlify deployment config
```

### Customization

#### Questions and Labels
- Edit dimension labels in `questions.js` → `window.QUESTIONS.labels`
- Update questions in `questions.js` → `window.QUESTIONS.pages`
- Modify analysis content in `analysis.js` → `window.ANALYSIS`

#### Styling
- Colors and themes: Edit CSS variables in `styles.css` `:root` section
- Layout: Modify classes and structure in `styles.css`

#### Assessment Logic
- Rating scale: Currently 0-5, modify in `app.js` `renderAssessment()` function
- Number of questions per page: Change array length in `createInitialState()`
- Number of pages: Update the `pages` array length

## Deployment

### Vercel (Recommended)
1. Push your code to GitHub
2. Connect your repository to [Vercel](https://vercel.com)
3. Deploy automatically with the included `vercel.json` configuration

### Netlify
1. Push your code to GitHub
2. Connect your repository to [Netlify](https://netlify.com)
3. Deploy automatically with the included `netlify.toml` configuration

### GitHub Pages
1. Push your code to GitHub
2. Enable GitHub Pages in repository settings
3. Select source branch (usually `main`)

### Manual Deployment
Upload all files to any static hosting service:
- AWS S3 + CloudFront
- Google Cloud Storage
- Azure Static Web Apps
- Any web server

## Data & Privacy

- **Local Storage Only**: All assessment data is stored locally in the user's browser
- **No Server Required**: Fully client-side application
- **Export Options**: Users can download their results as PNG or CSV
- **Reset Functionality**: Users can restart the assessment anytime

## Browser Support

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## Technical Details

- **Framework**: Vanilla JavaScript (no dependencies)
- **Charts**: Chart.js 4 (loaded via CDN)
- **Styling**: Modern CSS with custom properties
- **Storage**: localStorage API
- **Responsive**: CSS Grid and Flexbox

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

MIT License - see LICENSE file for details

## Support

For questions or issues, please open an issue on GitHub or contact the maintainer.
