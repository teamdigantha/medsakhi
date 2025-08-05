# Medsakhi - Revolutionizing Clinical Trials with AI, Trust, and Compassion

Medsakhi is a comprehensive clinical trial management platform designed to connect patients, clinicians, sponsors, CROs, and public health officials in India. The platform leverages AI-powered matching, blockchain transparency, and compassionate patient support to revolutionize clinical trial management.

## 🚀 Features

### Core Platform Features
- **AI-Powered Patient-Trial Matching**: Intelligent matching based on EMR data and trial criteria
- **Blockchain Integration**: Transparent and auditable trial data with smart contracts
- **Mitra Support System**: 24/7 AI companion for patient guidance and support
- **Digital Wallet**: Seamless travel reimbursements and compensation management
- **Real-time Analytics**: Comprehensive dashboards for all stakeholders
- **National Trial Registry**: Centralized registry for public health officials

### Role-Based Dashboards

#### 🧬 Patient Dashboard
- View eligible trials based on medical conditions
- Join trials with one-click enrollment
- Mitra AI support for guidance and questions
- Digital wallet for travel reimbursements
- Progress tracking through trial stages
- Real-time notifications and updates

#### 👨‍⚕️ Clinician Dashboard
- Manage patient enrollment requests
- View eligible patients for trials
- Trial enrollment forms and management
- Calendar view of trial schedules
- Patient messaging and communication
- Progress monitoring and reporting

#### 💼 Sponsor Dashboard
- Real-time recruitment metrics and analytics
- Trial progress monitoring
- Site and clinician management
- Blockchain transaction tracking
- Protocol upload and management
- Comprehensive reporting tools

#### 🔬 CRO Dashboard
- Operational metrics and data quality
- Site performance monitoring
- Trial data management
- Compliance tracking
- Blockchain integration
- Quality assurance tools

#### 🌍 Public Health Dashboard
- National trial registry overview
- Regional analytics and trends
- Disease distribution analysis
- State-wise trial monitoring
- Public health reporting
- Regulatory compliance tracking

#### ⚙️ Admin Dashboard
- User management and role assignment
- Trial creation and management
- System logs and activity monitoring
- Platform settings and configuration
- Security and access control

## 🛠️ Tech Stack

- **Frontend**: React.js 18.2.0
- **Styling**: TailwindCSS 3.3.0
- **Routing**: React Router DOM 6.3.0
- **Icons**: Lucide React 0.263.1
- **Charts**: Recharts 2.7.2
- **Animations**: Framer Motion 10.16.4
- **Lottie**: Lottie React 2.4.0
- **Fonts**: Inter, Nunito (Google Fonts)

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd medsakhi
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the development server**
   ```bash
   npm start
   ```

4. **Open your browser**
   Navigate to `http://localhost:3000`

## 🏗️ Project Structure

```
medsakhi/
├── public/
│   └── index.html
├── src/
│   ├── components/
│   │   ├── Navbar.js
│   │   ├── Sidebar.js
│   │   └── ProtectedRoute.js
│   ├── contexts/
│   │   ├── AuthContext.js
│   │   └── ThemeContext.js
│   ├── data/
│   │   └── mockData.js
│   ├── pages/
│   │   ├── HomePage.js
│   │   ├── AuthPage.js
│   │   ├── PatientDashboard.js
│   │   ├── ClinicianDashboard.js
│   │   ├── SponsorDashboard.js
│   │   ├── CRODashboard.js
│   │   ├── PublicHealthDashboard.js
│   │   ├── TrialRegistry.js
│   │   └── AdminPage.js
│   ├── App.js
│   ├── index.js
│   └── index.css
├── package.json
├── tailwind.config.js
├── postcss.config.js
└── README.md
```

## 🎨 Design System

### Color Palette
- **Primary**: Blue (#0ea5e9) - Trust and reliability
- **Success**: Green (#22c55e) - Positive actions and status
- **Warning**: Orange (#f59e0b) - Caution and pending states
- **Error**: Red (#ef4444) - Errors and critical actions
- **Secondary**: Gray (#64748b) - Text and borders

### Typography
- **Primary Font**: Inter - Clean and modern
- **Secondary Font**: Nunito - Friendly and approachable

### Components
- **Cards**: Rounded corners with subtle shadows
- **Buttons**: Primary and secondary variants with hover states
- **Status Badges**: Color-coded for different states
- **Forms**: Clean input fields with focus states
- **Navigation**: Responsive sidebar and navbar

## 🔐 Authentication & Authorization

The platform uses role-based access control with the following user types:

- **Patient** (`/patient`) - Trial discovery and participation
- **Clinician** (`/clinician`) - Patient and trial management
- **Sponsor** (`/sponsor`) - Trial oversight and metrics
- **CRO** (`/cro`) - Operational management
- **Public Health** (`/public-health`) - National registry access
- **Admin** (`/admin`) - Platform administration

## 📊 Mock Data

The application includes comprehensive mock data for:

- **Trials**: 3 sample trials with detailed information
- **Patients**: 3 sample patients with EMR data
- **Clinicians**: 3 sample clinicians with specializations
- **Metrics**: Recruitment and operational metrics
- **Blockchain**: Sample transaction data
- **Chat**: Mitra support conversation history
- **Wallet**: Transaction history and balances

## 🚀 Demo Credentials

For testing purposes, use these demo credentials:

- **Email**: `demo@medsakhi.com`
- **Password**: `demo123`

## 🎯 Key Features Implementation

### AI-Powered Matching
- Patient eligibility assessment based on trial criteria
- EMR data integration for intelligent matching
- Real-time recommendations and notifications

### Blockchain Integration
- Smart contract addresses for each trial
- Transaction history and verification
- Transparent data audit trail

### Mitra Support System
- AI chatbot for patient guidance
- Real-time conversation interface
- Contextual responses and support

### Digital Wallet
- Travel reimbursement tracking
- Transaction history and status
- Balance management and notifications

### Analytics & Reporting
- Interactive charts and visualizations
- Real-time metrics and KPIs
- Exportable reports and data

## 🔧 Customization

### Adding New Trials
Edit `src/data/mockData.js` to add new trial data:

```javascript
{
  id: 'TRIAL004',
  title: 'Your Trial Title',
  sponsor: 'Your Sponsor',
  phase: 'Phase II',
  status: 'active',
  // ... other properties
}
```

### Modifying User Roles
Update the role definitions in `src/components/Sidebar.js`:

```javascript
case 'new-role':
  return [
    { name: 'Dashboard', icon: Home, path: '/new-role' },
    // ... other menu items
  ];
```

### Styling Customization
Modify `tailwind.config.js` to customize colors, fonts, and other design tokens.

## 📱 Responsive Design

The application is fully responsive and optimized for:
- **Desktop**: Full dashboard experience
- **Tablet**: Adapted layouts with touch-friendly interactions
- **Mobile**: Mobile-first design with collapsible navigation

## 🔒 Security Features

- **Protected Routes**: Role-based access control
- **Authentication**: Session management with localStorage
- **Input Validation**: Form validation and sanitization
- **CSRF Protection**: Token-based request validation

## 🚀 Deployment

### Build for Production
```bash
npm run build
```

### Environment Variables
Create a `.env` file for production configuration:

```env
REACT_APP_API_URL=your-api-url
REACT_APP_BLOCKCHAIN_NETWORK=ethereum
REACT_APP_ANALYTICS_ID=your-analytics-id
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Design Inspiration**: Notion, Stripe Dashboard, Apple Health
- **Icons**: Lucide React
- **Charts**: Recharts
- **Animations**: Framer Motion
- **Fonts**: Google Fonts (Inter, Nunito)

## 📞 Support

For support and questions:
- **Email**: support@trialsaathi.com
- **Documentation**: [docs.trialsaathi.com](https://docs.trialsaathi.com)
- **Issues**: [GitHub Issues](https://github.com/trialsaathi/issues)

---

**TrialSaathi** - Revolutionizing Clinical Trials with AI, Trust, and Compassion 🧬 