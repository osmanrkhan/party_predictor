# Poisson Party Predictor

A real-time party attendance predictor that uses the Poisson distribution to estimate how many guests will show up to your event. Built with React and featuring dynamic visualizations.

![Poisson Party Predictor Screenshot](/api/placeholder/800/400)

## Features

- Real-time attendance prediction using Poisson distribution
- Dynamic visualization of current and expected guests
- Animated guest visualization with "ghost" predictions
- Live probability distribution charts
- Adaptive predictions based on actual arrival rates
- Encouraging status messages based on party performance
- Dark mode interface inspired by modern event platforms

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/poisson-party-predictor
cd poisson-party-predictor
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

## Usage

1. Set your initial party parameters:
   - Expected total number of guests (0-1000)
   - Party duration (60-360 minutes)

2. Click "Start Party" to begin tracking

3. As guests arrive:
   - Click "Guest Arrived!" to log each arrival
   - Adjust elapsed time manually as needed
   - Watch the predictions update in real-time

4. Monitor your party's performance:
   - View current and predicted guest counts
   - Check arrival rates and trends
   - See encouraging status messages
   - Visualize probability distributions

## Technical Details

### Dependencies

- React
- Recharts (for charts)
- Lucide React (for icons)
- Tailwind CSS (for styling)

### Key Components

- `RealtimePoissonParty`: Main component
- Canvas-based guest visualization
- Real-time probability distribution charts
- Dynamic status messaging system

### Statistical Implementation

The predictor uses:
- Poisson distribution for arrival probability
- Bayesian updating based on actual arrivals
- Blended rate calculation combining expected and actual rates
- Dynamic maximum value calculation for distribution display

### Customization

You can modify:
- Prediction parameters in `getPredictedRemaining()`
- Visual styles in the Tailwind classes
- Status message thresholds in `getStatusMessage()`
- Animation parameters in the canvas rendering loop

## License

MIT License - feel free to use and modify for your own projects.

## Acknowledgments

- My neurotic friends
- Claude
