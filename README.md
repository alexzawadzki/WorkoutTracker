# Workout Tracker

A beautiful, interactive workout tracking application designed for a 4-week fitness challenge. Built with vanilla JavaScript and Firebase for real-time progress syncing across devices.

## Features

- **4-Week Progressive Program**: Structured workout plan with increasing difficulty each week
- **Real-Time Sync**: Firebase integration allows progress tracking across multiple devices
- **Interactive Checkboxes**: Mark individual exercises as complete
- **Progress Tracking**: Visual progress bar and statistics dashboard
- **Streak Counter**: Track your workout consistency
- **Partner Workouts**: Special workouts designed for two people
- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Offline Support**: LocalStorage fallback when Firebase is unavailable

## Live Demo

Visit the app at: `https://alexzawadzki.github.io/WorkoutTracker/`

## Technologies Used

- HTML5
- CSS3 (Gradient backgrounds, Flexbox, Grid)
- Vanilla JavaScript
- Firebase Firestore (Real-time database)
- GitHub Pages (Hosting)
- GitHub Actions (CI/CD)

## Workout Structure

### Week 1: Foundation
- Full Body Circuit
- Cardio Mix
- Core & Flexibility
- Lower Body Blast
- Partner Workout

### Week 2: Building Strength
- Upgraded circuits with increased reps and new exercises
- Longer workout durations
- Introduction of burpees and V-ups

### Week 3: Intensification
- Tabata training introduction
- 4-5 rounds per workout
- Advanced core exercises
- Jump variations added

### Week 4: Peak Performance
- "12 Days of Fitness" challenge
- Holiday-themed workouts
- Maximum effort final challenge
- Celebration and progress photos

## Progress Tracking

The app tracks:
- **Days Completed**: Total workout days finished
- **Overall Progress**: Percentage of entire program completed
- **Current Streak**: Consecutive days with completed workouts
- **Exercise-Level Detail**: Individual exercise completion within each workout

## Firebase Configuration

The app uses Firebase Firestore to sync progress between devices. Data is stored in:
- Collection: `workoutProgress`
- Document: `alexAndKarolina`

If Firebase is unavailable, the app automatically falls back to browser LocalStorage.

## Local Development

1. Clone the repository:
```bash
git clone https://github.com/alexzawadzki/WorkoutTracker.git
cd WorkoutTracker
```

2. Open `index.html` in your browser:
```bash
open index.html
```

Or use a local server:
```bash
python -m http.server 8000
# Visit http://localhost:8000
```

## Deployment

The app automatically deploys to GitHub Pages when changes are pushed to the `main` branch via GitHub Actions.

### Deployment Workflow
1. Push changes to `main` branch
2. GitHub Actions workflow triggers
3. Static files are uploaded to GitHub Pages
4. Site is live at the GitHub Pages URL

## Reset Progress

Click the "Reset All Progress" button to clear all workout data. This will:
- Clear Firebase data
- Clear LocalStorage
- Reset all checkboxes and statistics

**Warning**: This action cannot be undone.

## Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge

## License

This project is open source and available for personal use.

## Credits

Created for Alex & Karolina's Workout Challenge 🎉
