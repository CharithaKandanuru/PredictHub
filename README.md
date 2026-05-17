# PredictAI Hub

A modern, fully functional, responsive AI-powered prediction analytics web application that works across multiple sectors such as Banking, Shopping/Retail, Healthcare, Education, Insurance, Real Estate, Agriculture, and Business Analytics.

## Features

### 🔐 Authentication System
- Login page with animated UI
- Signup/Register page
- Forgot password page
- JWT-based authentication UI flow
- Social login buttons (Google, GitHub)
- Secure session handling UI
- Remember me option

### 🏠 Home Page
- Attractive hero section with AI-themed design
- Intro about AI prediction platform
- Sector selection cards with icons and animations
- Testimonials section
- AI analytics showcase section
- Feature cards
- Footer with contact, links, and social media

### 📊 Sector-Based Prediction System
Each sector allows:
- Dataset upload (CSV, Excel)
- Manual data entry forms
- Data preprocessing preview
- Feature selection UI
- Prediction trigger button
- Real-time loading animations
- AI confidence score display

**Supported Sectors:**
- Banking (Loan approval, credit risk, fraud detection)
- Retail/Shopping (Customer insights, sales forecasting)
- Healthcare (Disease prediction, patient risk analysis)
- Education (Student performance, dropout risk)
- Insurance (Claim prediction, risk classification)
- Agriculture (Crop yield, weather impact analysis)
- Real Estate (Property valuation, market trends)
- Manufacturing (Quality control, demand forecasting)
- Marketing (Campaign optimization, lead scoring)

### 📈 Advanced Analytics Dashboard
- Sidebar navigation
- Top navbar with search
- User profile section
- Notification center
- Dynamic widgets/cards
- Real-time analytics display
- Pie charts, Bar graphs, Line charts
- Area charts, Heatmaps, Radar charts
- Tables with filters
- Download reports option
- Export PDF/Excel buttons
- AI-generated insights section
- Prediction history
- Sector comparison analytics
- KPI cards
- Accuracy metrics (Precision, Recall, F1 Score)
- Interactive drill-down charts

### 🤖 AI Analysis Page
- Detailed prediction explanation
- Prediction probability
- Confidence percentage
- Important features affecting prediction
- Risk level indicator
- Trend analysis
- Suggested actions/recommendations
- AI explanation cards
- Data visualization panels

### 👨‍💼 Admin Panel
- Manage users
- Manage datasets
- Monitor predictions
- Analytics overview
- Sector usage statistics
- User activity logs
- Subscription plans UI
- System health dashboard

### 🎨 UI/UX Features
- Fully responsive design
- Mobile-friendly
- Modern enterprise SaaS design
- Smooth transitions and animations
- Framer Motion animations
- Recharts visualizations
- Professional icons using Lucide React
- Loading skeletons
- Empty states
- Toast notifications
- Search and filters
- Dynamic theme switching (Dark/Light mode)
- Glassmorphism effects
- Gradients

### 🤖 Smart Features
- AI chatbot assistant
- Dataset validation
- Drag-and-drop file upload
- Real-time prediction updates
- Multi-language support
- Dark/light mode
- Notification system
- Role-based access UI
- Activity tracking
- Recent predictions panel

## Tech Stack

### Frontend
- **React.js** - UI library
- **Vite** - Build tool
- **Tailwind CSS** - Styling
- **Framer Motion** - Animations
- **React Router** - Routing
- **Axios** - HTTP client
- **Recharts** - Charts and graphs
- **Lucide React** - Icons
- **Context API** - State management

## Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd Predict
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and navigate to `http://localhost:3000`

### Build for Production

```bash
npm run build
```

The built files will be in the `dist` directory.

## Project Structure

```
Predict/
├── public/
├── src/
│   ├── components/
│   │   ├── charts/          # Chart components (Pie, Bar, Line, etc.)
│   │   ├── data/            # Data upload components
│   │   ├── layout/          # Layout components (Sidebar, Navbar)
│   │   ├── smart/           # Smart features (AI Chatbot)
│   │   └── ui/              # Reusable UI components
│   ├── context/             # Context providers (Theme, Auth, Notification)
│   ├── lib/                 # Utility functions and constants
│   ├── pages/
│   │   ├── admin/           # Admin panel
│   │   ├── ai-analysis/     # AI analysis page
│   │   ├── analytics/       # Analytics dashboard
│   │   ├── auth/            # Authentication pages
│   │   ├── dashboard/       # Main dashboard
│   │   ├── datasets/        # Datasets management
│   │   ├── sector/          # Sector-specific dashboards
│   │   ├── settings/        # Settings page
│   │   ├── users/           # User management
│   │   └── Home.jsx          # Landing page
│   ├── App.jsx              # Main app component with routing
│   ├── index.css            # Global styles
│   └── main.jsx             # Entry point
├── index.html
├── package.json
├── tailwind.config.js
├── vite.config.js
└── README.md
```

## Usage

### Authentication
1. Navigate to `/login` to sign in
2. Or click "Sign up" to create a new account
3. Use social login buttons for quick access (Google, GitHub)

### Dashboard
1. After login, you'll be redirected to the main dashboard
2. View KPI cards, charts, and recent predictions
3. Navigate to different sections using the sidebar

### Sector Predictions
1. Click on any sector card from the home page or sidebar
2. Upload your dataset or enter data manually
3. Select a prediction model
4. Click "Run Prediction" to get AI-powered insights
5. View detailed analysis in the AI Analysis page

### Admin Panel
1. Navigate to `/admin` (requires admin role)
2. Manage users, datasets, and system settings
3. Monitor system health and activity logs

## Customization

### Adding New Sectors
1. Add sector configuration in `src/lib/utils.js`
2. Create sector-specific prediction models
3. Update sector icons and colors

### Modifying Charts
1. Chart components are in `src/components/charts/`
2. Use Recharts documentation for customization
3. Modify data structures as needed

### Theme Customization
1. Update colors in `tailwind.config.js`
2. Modify glassmorphism effects in `src/index.css`
3. Add custom animations in Tailwind config

## Deployment

### Vercel
```bash
npm install -g vercel
vercel
```

### Netlify
```bash
npm run build
# Upload dist folder to Netlify
```

### Docker
```dockerfile
FROM node:18-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build
EXPOSE 3000
CMD ["npm", "run", "preview"]
```

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License.

## Support

For support, email support@predictai.com or open an issue in the repository.

## Acknowledgments

- Recharts for the charting library
- Framer Motion for animations
- Lucide for beautiful icons
- Tailwind CSS for styling
