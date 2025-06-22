# Discord Server Admin Dashboard

A modern, responsive Discord server administration dashboard built with Next.js 14 and Tailwind CSS. This dashboard provides a comprehensive interface for managing Discord server members, roles, and messages with a beautiful dark/light theme toggle.

![Dashboard Preview](https://via.placeholder.com/800x400/6366f1/ffffff?text=Discord+Server+Dashboard)

##  Features

###  Dashboard Overview

- Real-time server statistics (members, online users, roles, messages)
- Interactive member growth chart
- Recent activity feed
- Server performance metrics

###  Member Management

- Searchable and filterable member list
- Pagination for large member counts
- Role-based filtering
- Add new members (mock functionality)
- Sort by join date or username
- Online/offline status indicators

### Role Management

- Visual role hierarchy display
- Toggle role visibility
- Inline role name editing
- Permission overview
- Role-based color coding
- Member count per role

###  Message Management

- Cross-channel message viewing
- Search functionality
- Channel-based filtering
- Message deletion (mock)
- Timestamp and user information
- Channel activity statistics

###  Design & UX

- **Dark/Light Mode**: Persistent theme toggle with localStorage
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile
- **Accessibility**: ARIA labels, keyboard navigation, proper contrast
- **Smooth Animations**: Hover effects and transitions
- **Custom Components**: Built from scratch without UI libraries

##  Tech Stack

- **Framework**: Next.js 14 (App Router)
- **Styling**: Tailwind CSS
- **Icons**: Lucide React
- **State Management**: React Context API + useReducer
- **Language**: TypeScript
- **Deployment Ready**: Vercel/Netlify compatible

##  Getting Started

### Prerequisites

- Node.js 18+ installed
- npm, yarn, or pnpm package manager

### Installation

1. **Clone the repository**

   ```bash
   git clone <repository-url>
   cd dis-dashboard
   ```

2. **Install dependencies**

   ```bash
   npm install
   # or
   yarn install
   # or
   pnpm install
   ```

3. **Run the development server**

   ```bash
   npm run dev
   # or
   yarn dev
   # or
   pnpm dev
   ```

4. **Open in browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

##  Project Structure

```
src/
├── app/                    # Next.js 14 App Router
│   ├── globals.css        # Global styles and theme
│   ├── layout.tsx         # Root layout with providers
│   └── page.tsx           # Main page component
├── components/            # React components
│   ├── pages/            # Page components
│   │   ├── Dashboard.tsx # Main dashboard with stats
│   │   ├── Members.tsx   # Member management
│   │   ├── Roles.tsx     # Role management
│   │   └── Messages.tsx  # Message management
│   ├── DashboardLayout.tsx # Main layout wrapper
│   ├── Navbar.tsx        # Top navigation bar
│   └── Sidebar.tsx       # Left navigation sidebar
├── context/              # React Context for state
│   └── DashboardContext.tsx # Global state management
├── data/                 # Mock data
│   └── mockData.ts       # Sample Discord server data
├── types/                # TypeScript definitions
│   └── index.ts          # Type definitions
└── utils/                # Utility functions
    └── dashboard.ts      # Helper functions

## 🚀 Deployment

### Vercel 

1. Push code to GitHub repository
2. Connect repository to Vercel
3. Deploy automatically on push.
## 📄 License

This project is open source and available under the [MIT License](LICENSE).


