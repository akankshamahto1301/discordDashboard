# Discord Server Admin Dashboard

A modern, responsive Discord server administration dashboard built with Next.js 14 and Tailwind CSS. This dashboard provides a comprehensive interface for managing Discord server members, roles, and messages with a beautiful dark/light theme toggle.

![Dashboard Preview](https://via.placeholder.com/800x400/6366f1/ffffff?text=Discord+Server+Dashboard)

## ✨ Features

### 📊 Dashboard Overview

- Real-time server statistics (members, online users, roles, messages)
- Interactive member growth chart
- Recent activity feed
- Server performance metrics

### 👥 Member Management

- Searchable and filterable member list
- Pagination for large member counts
- Role-based filtering
- Add new members (mock functionality)
- Sort by join date or username
- Online/offline status indicators

### 🛡️ Role Management

- Visual role hierarchy display
- Toggle role visibility
- Inline role name editing
- Permission overview
- Role-based color coding
- Member count per role

### 💬 Message Management

- Cross-channel message viewing
- Search functionality
- Channel-based filtering
- Message deletion (mock)
- Timestamp and user information
- Channel activity statistics

### 🎨 Design & UX

- **Dark/Light Mode**: Persistent theme toggle with localStorage
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile
- **Accessibility**: ARIA labels, keyboard navigation, proper contrast
- **Smooth Animations**: Hover effects and transitions
- **Custom Components**: Built from scratch without UI libraries

## 🛠️ Tech Stack

- **Framework**: Next.js 14 (App Router)
- **Styling**: Tailwind CSS
- **Icons**: Lucide React
- **State Management**: React Context API + useReducer
- **Language**: TypeScript
- **Deployment Ready**: Vercel/Netlify compatible

## 🚀 Getting Started

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

## 📁 Project Structure

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
```

## 🎯 Key Features Explained

### State Management

The application uses React Context API with useReducer for global state management, providing:

- Centralized state for users, roles, messages, and UI preferences
- Type-safe actions and state updates
- Persistent dark mode preference in localStorage

### Mock Data & Interactions

All functionality is frontend-only with realistic mock data:

- **8 sample users** with different roles and online status
- **6 role types** with permissions and color coding
- **5 sample messages** across different channels
- **Interactive features** like adding users, editing roles, deleting messages

### Responsive Design

- **Mobile-first approach** with collapsible sidebar
- **Breakpoint coverage**: sm (640px), md (768px), lg (1024px)
- **Touch-friendly**: Proper button sizes and spacing
- **Flexible layouts**: Grid and flexbox for optimal spacing

### Accessibility Features

- **ARIA labels** on all interactive elements
- **Keyboard navigation** support
- **Screen reader** friendly structure
- **High contrast** color schemes
- **Focus indicators** for all focusable elements

## 🎨 Design Philosophy

### Custom Component Approach

- **No UI libraries**: All components built from scratch
- **Tailwind-first**: Utility classes for consistent styling
- **Component reusability**: Modular design patterns
- **Design system**: Consistent spacing, colors, and typography

### Color Scheme

- **Light Mode**: Clean whites and grays with indigo accents
- **Dark Mode**: Rich darks with proper contrast ratios
- **Role Colors**: Distinct color coding for different user roles
- **Status Indicators**: Green for online, gray for offline

## 📱 Browser Compatibility

- **Modern browsers**: Chrome 90+, Firefox 88+, Safari 14+, Edge 90+
- **Mobile browsers**: iOS Safari, Chrome Mobile, Samsung Internet
- **Progressive enhancement**: Graceful degradation for older browsers

## 🔧 Development

### Available Scripts

```bash
# Development server with Turbopack
npm run dev

# Production build
npm run build

# Start production server
npm run start

# Run ESLint
npm run lint
```

### Customization

1. **Mock Data**: Edit `src/data/mockData.ts` to customize server data
2. **Styling**: Modify Tailwind classes or add custom CSS
3. **Features**: Add new pages by creating components and updating the router
4. **Theming**: Adjust color schemes in the Tailwind configuration

## 📝 Implementation Notes

### Why This Approach?

1. **Educational Value**: Demonstrates modern React patterns and best practices
2. **Customization**: Full control over design and functionality
3. **Performance**: Minimal dependencies and optimized bundle size
4. **Maintainability**: Clear separation of concerns and modular architecture

### Mock vs Real Implementation

This dashboard showcases frontend capabilities without backend complexity:

- **Real Discord Integration**: Would require Discord OAuth and Bot API
- **Database**: Would need user authentication and data persistence
- **Real-time Updates**: Would implement WebSocket connections
- **File Uploads**: Would handle avatar and file management

## 🚀 Deployment

### Vercel (Recommended)

1. Push code to GitHub repository
2. Connect repository to Vercel
3. Deploy automatically on push

### Netlify

1. Build the project: `npm run build`
2. Deploy the `out` folder to Netlify

### Other Platforms

The project builds to static files and can be deployed anywhere that serves static content.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit changes: `git commit -m 'Add amazing feature'`
4. Push to branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- **Next.js Team**: For the excellent React framework
- **Tailwind CSS**: For the utility-first CSS framework
- **Lucide**: For the beautiful icon set
- **Unsplash**: For placeholder avatar images

---

**Built with ❤️ for Discord Server Management**

For questions or support, please open an issue in the GitHub repository.
