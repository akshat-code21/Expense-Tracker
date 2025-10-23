# PennyWise - Modern Expense Tracking Application

PennyWise is a comprehensive full-stack expense tracking application built with modern technologies. It features an intuitive React frontend and a robust TypeScript backend, providing users with powerful financial management tools including AI-powered insights, detailed analytics, and smart saving recommendations.

## ✨ Key Features

- 📊 **Interactive Dashboard** - Real-time expense visualization with charts and graphs
- 💳 **Expense Management** - Full CRUD operations for tracking expenses by category
- 🤖 **AI-Powered Insights** - Google Gemini AI integration for personalized financial analysis
- 💡 **Smart Saving Tips** - Intelligent recommendations based on spending patterns
- 📱 **Responsive Design** - Optimized for desktop and mobile devices
- 🔐 **Secure Authentication** - JWT-based user authentication with password hashing
- 🎯 **Budget Planning** - Category-based expense tracking and goal setting

## 🏗️ Architecture

This project follows a modern full-stack architecture:

```
PennyWise/
├── Backend/          # TypeScript/Express API server
└── Frontend/         # React/TypeScript client application
```

## 🛠️ Tech Stack

### Backend
- **Runtime**: Node.js with Express.js
- **Language**: TypeScript
- **Database**: MongoDB with Mongoose ODM
- **Authentication**: JWT tokens with bcrypt password hashing
- **Validation**: Zod schema validation
- **AI Integration**: Google Gemini Pro API
- **Security**: CORS, input validation, error handling

### Frontend
- **Framework**: React 18 with TypeScript
- **Build Tool**: Vite
- **Styling**: Tailwind CSS with Shadcn UI components
- **State Management**: Redux Toolkit
- **Charts**: Recharts for data visualization
- **Forms**: React Hook Form with validation
- **Icons**: Lucide React & Tabler Icons
- **Animations**: Framer Motion

## 🚀 Getting Started

### Prerequisites

- **Node.js** (v16 or higher)
- **MongoDB** (local instance or cloud)
- **Google Gemini API Key** (for AI insights)
- **npm** or **yarn** package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd project
   ```

2. **Set up the Backend**
   ```bash
   cd Backend
   npm install

   # Create environment file
   cp .env.example .env
   # Edit .env with your configuration
   ```

3. **Set up the Frontend**
   ```bash
   cd ../Frontend
   npm install
   ```

### Environment Configuration

Create a `.env` file in the `Backend/` directory with:

```env
MONGO_URL=your_mongodb_connection_string
JWT_SECRET=your_secure_jwt_secret_key
GEMINI_API_KEY=your_google_gemini_api_key
PORT=5000
```

### Running the Application

1. **Start the Backend** (from Backend directory)
   ```bash
   npm run dev
   ```
   The backend will start on `http://localhost:5000`

2. **Start the Frontend** (from Frontend directory)
   ```bash
   npm run dev
   ```
   The frontend will start on `http://localhost:5173`

3. **Access the application**
   Open your browser and navigate to `http://localhost:5173`

## 📁 Project Structure

```
project/
├── Backend/
│   ├── src/
│   │   ├── config/          # Database and app configuration
│   │   ├── middlewares/     # Custom Express middlewares
│   │   ├── models/          # MongoDB schemas
│   │   ├── routes/          # API route handlers
│   │   └── index.ts         # Application entry point
│   ├── dist/                # Compiled JavaScript files
│   ├── package.json
│   └── tsconfig.json
│
└── Frontend/
    ├── src/
    │   ├── components/      # Reusable UI components
    │   │   ├── auth/        # Authentication components
    │   │   ├── dashboard/   # Dashboard-specific components
    │   │   └── ui/          # Base UI components
    │   ├── features/        # Redux slices and state logic
    │   ├── hooks/           # Custom React hooks
    │   ├── lib/             # Utility functions
    │   └── store/           # Redux store configuration
    ├── public/              # Static assets
    └── package.json
```

## 🔌 API Endpoints

### Authentication
- `POST /api/v1/auth/signup` - Register new user
- `POST /api/v1/auth/signin` - User login

### Expenses
- `GET /api/v1/expenses` - Retrieve user expenses
- `POST /api/v1/expenses` - Create new expense
- `PUT /api/v1/expenses/:id` - Update existing expense
- `DELETE /api/v1/expenses/:id` - Delete expense

### Insights
- `GET /api/v1/insights/ai-analysis` - AI-powered expense analysis
- `GET /api/v1/insights/statistics` - Statistical expense breakdowns

## 🎯 Usage Guide

1. **Sign Up/Login** - Create an account or sign in to existing one
2. **Dashboard Overview** - View your financial summary and recent activity
3. **Add Expenses** - Track new expenses with categories and descriptions
4. **View Analytics** - Analyze spending patterns with interactive charts
5. **AI Insights** - Get personalized financial recommendations
6. **Manage Expenses** - Edit or delete existing expense entries

## 🔒 Security Features

- **Password Hashing** - bcrypt for secure password storage
- **JWT Authentication** - Token-based secure API access
- **Input Validation** - Zod schemas for data validation
- **CORS Protection** - Configured cross-origin resource sharing
- **Error Handling** - Comprehensive error management and logging

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines

- Follow TypeScript best practices
- Use ESLint for code linting
- Write meaningful commit messages
- Test your changes thoroughly
- Update documentation as needed

## 📄 License

This project is licensed under the ISC License.

## 🙏 Acknowledgments

- **Previous Version**: Original JavaScript backend by [apurvdugar](https://github.com/apurvdugar/PennyWise)
- **UI Components**: Built with [Shadcn UI](https://ui.shadcn.com/)
- **Icons**: [Lucide React](https://lucide.dev/) and [Tabler Icons](https://tabler.io/icons)
- **Charts**: Powered by [Recharts](https://recharts.org/)

---

**Happy expense tracking with PennyWise! 💰**
