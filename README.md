# CRMApp

A responsive, user-friendly frontend for a CRM (Customer Relationship Management) platform. Built with React, Tailwind CSS, and integrated with Google OAuth and dynamic campaign management.

## 🚀 Features

### User Authentication
- Google OAuth login
- Session management and secure storage
- Protected routes based on user authentication

### Dashboard
- Summary cards for Customers, Orders, Campaigns
- Clean, responsive UI
- Quick navigation links

### Customer Module
- Add new customers
- View customer list
- Real-time UI update after insertion

### other Module
- Add orders for customers
- View order history

### Segment Builder
- Dynamic rule builder (field, operator, value)
- Multiple condition support with AND/OR logic
- Audience preview functionality (real-time MongoDB query)
- Save custom segments

### Campaigns
- Create campaign linked to a segment
- AI-assisted message generation
- Send email via nodemailer
- View delivery stats (sent, failed, total)


## 🛠️ Tech Stack

### Frontend
- React 19
- Tailwind CSS
- React Router DOM
- Axios
- Google OAuth
- Toast Notifications (react-hot-toast)
- Charting with Recharts
- Lucide-react + shadcn/ui for UI components


## 💾 Environment Variables

### Frontend
```env
VITE_BACKEND_URL=https://crmapp-backend.onrender.com
```


## 📦 Installation

### Frontend Setup
```bash
# Navigate to frontend directory
cd frontend

# Install dependencies
npm install

# Start the development server
npm run dev

```

## Authentication
- Sign in using Google OAuth on the Landing page
- Google login stores userId, name, and picture in localStorage
- Logout from sidebar clears session and redirects to SignIn


### Campaigns and Segments
- Audience segments support flexible condition building (e.g., totalSpend > 10000 AND visits < 3)
- Preview Audience button queries backend and displays number of matched users
- Campaigns can be created from these segments and sent using nodemailer


### UX Bonus
- Drag-and-drop-like UX for rules
- Responsive design on all screen sizes
- Sidebar and Topbar layout with clear navigation
- Toasts for notifications

### Security
- Auth middleware validation on all protected APIs
- Google OAuth verification token stored securely
- AuthContext used to manage state globally

## 👏 Acknowledgments
- Tailwind CSS
- React

## 📞 Contact
Your Name - haiderzaidi45h@gmail.com

Project Link: [GitHub Repository](https://github.com/haider-zaidi/CRM-frontend)

