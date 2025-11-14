# Piciclot Tracker - Personal Spending Tracker

A modern web application for tracking personal expenses, managing budgets, and visualizing spending patterns.

## 🎯 Project Overview

Piciclot Tracker is a full-stack web application designed to help users monitor their spending habits, set budgets, and gain insights through interactive charts and visualizations. The application features a clean, gradient interface with comprehensive user management and data visualization capabilities.

## ✨ Features

### Authentication & User Management
- **User Registration** - Create new accounts with email verification
- **Email Activation** - Account activation via email token
- **Secure Login** - Password-protected user authentication
- **Password Recovery** - Forgot password functionality
- **Profile Management** - Update personal information and passwords

### Dashboard & Analytics
- **Interactive Charts** - Visualize spending with:
  - Pie Chart - Category breakdown
  - Bar Chart - Spending comparisons
  - Line Chart - Spending trends over time
- **Budget Setting** - Set and track monthly/weekly budgets
- **Spending Overview** - Comprehensive view of all transactions
- **Real-time Updates** - Live data synchronization

### User Settings
- **Personal Information Management**
  - Full name
  - Birthday
  - Gender
  - Email
  - Password
- **Payment Information** (Future feature)
  - Payment methods
  - Billing address
  - Billing dates

## 🛠️ Technology Stack

### Frontend
- **React.js** - UI framework
- **React Router DOM** - Client-side routing
- **Axios** - HTTP client for API requests
- **React Toastify** - Toast notifications
- **Material Design Icons** - Icon library (MdVisibility, MdVisibilityOff)
- **CSS3** - Styling with gradients and animations

### Styling
- Custom CSS with gradient backgrounds
- Responsive design
- Google Fonts (Karla, Nunito, Montserrat, Roboto)
- Font Awesome icons

## 📁 Project Structure

```
spending-tracker/
├── components/
│   ├── Forgot/
│   │   └── Forgot.js
│   ├── Navbar/
│   │   └── Navbar.js
│   ├── Profile/
│   │   └── Profile.js
│   ├── Sidebar/
│   │   └── Sidebar.js
│   └── Input/
│       └── Input.js
├── pages/
│   ├── Signin.js
│   ├── Signup.js
│   ├── Charts.js
│   ├── Saver.js
│   └── Overview.js
├── layouts/
│   ├── AuthLayout.js
│   ├── ActivateLayout.js
│   └── ProfileLayout.js
├── styles/
│   ├── AuthLayout.css
│   ├── ProfileLayout.css
│   ├── settings.css
│   └── index.css
├── images/
│   └── landing1.png
└── README.md
```

## 🚀 Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Backend API server running (for authentication and data storage)

### Installation

1. **Clone the repository**
```bash
git clone <repository-url>
cd spending-tracker
```

2. **Install dependencies**
```bash
npm install
```

Required packages:
```bash
npm install react react-dom react-router-dom axios react-toastify
npm install react-icons
```

3. **Configure API endpoint**
Ensure your axios base URL points to your backend API (usually configured in a separate config file or environment variable)

4. **Start the development server**
```bash
npm start
```

The application will open at `http://localhost:3000`

## 📱 Application Pages

### Landing Page (`/`)
- Clean landing page with navigation
- Toggle between Sign In and Sign Up forms
- Forgot Password functionality
- Gradient background with hero image
- Navigation sections: Home, About, Services, Contact

### Account Activation (`/activate/:activation_token`)
- Email verification page
- Automatic token validation
- Success/error notifications
- Redirect to sign in

### Profile/Dashboard (`/profile`)
- Main dashboard with spending overview
- Interactive charts and visualizations
- Budget management tools
- Quick access to all features

### Settings
- Tabbed interface with:
  - Personal Information tab
  - Payment Information tab
- Update profile details
- Password management
- Go back navigation

## 🎨 Design Features

### Color Scheme
- Primary Gradient: `linear-gradient(to right, #2ed573, #f9ca24)`
- Accent Green: `#7ed386`, `#10ac84`
- Text: White on gradient backgrounds
- Cards: White with shadow effects

### Typography
- **Karla** - Main headings and navigation
- **Montserrat** - Section headers
- **Roboto** - Body text and labels
- **Nunito** - Special UI elements

### UI Components
- **Gradient Buttons** - Smooth hover effects
- **Toast Notifications** - Success/error feedback
- **Password Toggle** - Visibility icons for password fields
- **Responsive Navigation** - Fixed navbar with smooth scrolling
- **Card Layouts** - Shadowed cards for forms and content

## 📊 Features Breakdown

### Authentication Flow
1. User registers with email and password
2. Activation email sent with unique token
3. User clicks activation link
4. Account activated and redirected to sign in
5. User logs in with credentials
6. Access to full dashboard

### Budget Management
1. Set monthly/weekly budget target
2. Track expenses against budget
3. Visual indicators for budget status
4. Alerts when approaching/exceeding budget

### Data Visualization
- **Pie Chart**: Category-wise expense breakdown
- **Bar Chart**: Compare spending across periods
- **Line Chart**: Visualize spending trends over time

## 🔐 Security Features

- Password visibility toggle
- Password confirmation on registration
- Secure password fields (type="password")
- Email verification required
- Token-based activation
- Protected routes (requires authentication)

## 🎯 What This Application Does

### User Registration & Authentication
- Users can create accounts with name, email, and password
- Email verification through activation tokens sent to user's email
- Secure login system with password confirmation
- Password recovery through "Forgot Password" functionality
- Profile updates with password change capability

### Expense Tracking
- Record and categorize spending
- View comprehensive spending overview
- Track expenses over time
- Organize by categories

### Budget Management
- Set custom budget goals
- Monitor budget utilization
- Visual budget indicators
- Alerts and notifications for budget thresholds

### Data Visualization
- Multiple chart types for different insights
- Interactive data displays
- Real-time chart updates
- Category-based breakdowns

### Settings Management
- Update personal information
- Manage payment methods (future feature)
- Customize user preferences
- Security settings

## 🔄 User Workflow

1. **Landing** → User visits homepage
2. **Sign Up** → Creates account with email
3. **Email Activation** → Clicks link in email
4. **Sign In** → Logs into account
5. **Dashboard** → Views spending overview and charts
6. **Add Expenses** → Records new transactions
7. **Set Budget** → Defines spending limits
8. **Monitor** → Tracks progress via charts
9. **Settings** → Updates profile as needed

## 📝 Component Details

### Input Component
Reusable input field with:
- Dynamic type (text, password, email)
- Icon support (visibility toggle)
- Change handlers
- Default values
- Disabled state

### Form Handling
- Controlled components with state management
- Form validation
- Submit handlers
- Error handling with toast notifications

### Navigation
- Fixed navbar with smooth scrolling
- Responsive menu
- Active state indicators
- Logo and brand identity

## 🌐 API Endpoints (Expected)

```
POST /activation - Activate user account
POST /signin - User login
POST /signup - User registration
POST /forgot - Password recovery
GET /user - Get user profile
PUT /user - Update user profile
GET /expenses - Fetch user expenses
POST /expenses - Add new expense
GET /budget - Get budget settings
PUT /budget - Update budget
```

## 🚧 Future Enhancements

- [ ] **Expense Categories** - Custom category creation
- [ ] **Export Data** - Download reports as CSV/PDF
- [ ] **Recurring Expenses** - Set up automatic recurring entries
- [ ] **Payment Integration** - Connect bank accounts/cards
- [ ] **Mobile App** - React Native version
- [ ] **Multi-currency** - Support for different currencies
- [ ] **Shared Budgets** - Family/group budget tracking
- [ ] **AI Insights** - Smart spending recommendations
- [ ] **Receipt Scanning** - OCR for receipt capture
- [ ] **Dark Mode** - Theme toggle option

## 🐛 Known Issues

- Payment information section is not fully implemented
- Charts require backend data integration
- Mobile responsiveness needs improvement on some screens
- Settings page navigation needs Redux/Context integration
