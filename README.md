# BlogCraft - Modern Blog Platform

A modern, SEO-optimized blog platform with user authentication, content management, and commenting system. Built with React, Express.js, PostgreSQL, and deployed on Replit.

![BlogCraft Screenshot](https://images.unsplash.com/photo-1486312338219-ce68d2c6f44d?ixlib=rb-4.0.3&auto=format&fit=crop&w=1200&h=600)

## ✨ Features

### 🚀 Core Functionality
- **Modern Blog Platform**: Clean, responsive design optimized for readability
- **User Authentication**: Secure authentication powered by Replit Auth
- **Content Management**: Full CRUD operations for blog posts
- **Commenting System**: Threaded comments with moderation capabilities
- **Search Functionality**: Real-time search across posts and categories
- **Category System**: Organize posts with custom categories
- **SEO Optimized**: Meta tags, structured data, and performance optimization

### 📱 User Experience
- **Responsive Design**: Mobile-first approach, works on all devices
- **Fast Loading**: Optimized assets and efficient data loading
- **Interactive UI**: Smooth animations and transitions
- **Dark Mode Ready**: Built-in dark mode support
- **Accessibility**: WCAG compliant with proper focus management

### 🛠 Technical Features
- **Single-File Architecture**: Standalone deployment for easy hosting
- **PostgreSQL Database**: Robust data storage with relations
- **Real-time Updates**: Live comment updates and post statistics
- **Image Support**: Featured images and media handling
- **Performance Monitoring**: Built-in analytics and view tracking

## 🏗 Architecture

### Frontend
- **React 18**: Modern React with hooks and functional components
- **TypeScript**: Full type safety and better developer experience
- **Tailwind CSS**: Utility-first CSS framework for rapid styling
- **Wouter**: Lightweight routing solution
- **TanStack Query**: Data fetching and state management
- **Shadcn/UI**: Beautiful, accessible component library

### Backend
- **Express.js**: Fast, minimal web framework
- **PostgreSQL**: Reliable relational database
- **Drizzle ORM**: Type-safe database operations
- **Replit Auth**: Secure authentication system
- **Zod**: Runtime type validation

### Infrastructure
- **Replit**: Cloud-based development and hosting
- **Database**: PostgreSQL with connection pooling
- **CDN**: Image optimization via Unsplash
- **Fonts**: Google Fonts for typography

## 🚀 Getting Started

### Prerequisites
- Node.js 18+ and npm
- PostgreSQL database
- Replit account (for authentication)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/duskdeveloper/blog-website.git
   cd blogcraft
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   Create a `.env` file with:
   ```env
   DATABASE_URL=your_postgresql_connection_string
   SESSION_SECRET=your_secure_session_secret
   REPLIT_DOMAINS=your-domain.com
   REPL_ID=your_replit_app_id
   ```

4. **Initialize the database**
   ```bash
   npm run db:push
   ```

5. **Start development server**
   ```bash
   npm run dev
   ```

Visit `http://localhost:5000` to see your blog in action!

### Production Deployment

1. **Build the application**
   ```bash
   npm run build
   ```

2. **Start production server**
   ```bash
   npm start
   ```

## 📖 Usage Guide

### For Writers
1. **Sign up/Login**: Use Replit authentication to access the platform
2. **Create Posts**: Navigate to Dashboard → New Post
3. **Manage Content**: Edit, delete, or publish drafts from the dashboard
4. **Engage**: Respond to comments and build your community

### For Readers
1. **Browse Posts**: Discover content on the homepage
2. **Search**: Use the search function to find specific topics
3. **Comment**: Join discussions with threaded comments
4. **Share**: Share posts via social media or direct links

### For Administrators
1. **User Management**: Monitor user activity and moderate content
2. **Category Management**: Create and organize post categories
3. **Analytics**: Track post views, engagement, and user growth
4. **Moderation**: Approve/disapprove comments and manage spam

## 🔧 Configuration

### Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `DATABASE_URL` | PostgreSQL connection string | ✅ |
| `SESSION_SECRET` | Secret key for session encryption | ✅ |
| `REPLIT_DOMAINS` | Comma-separated list of allowed domains | ✅ |
| `REPL_ID` | Replit application ID for OAuth | ✅ |
| `ISSUER_URL` | OAuth issuer URL (default: Replit) | ❌ |
| `NODE_ENV` | Environment mode (development/production) | ❌ |

### Customization

#### Colors and Theming
Edit `client/src/index.css` to customize the color scheme:

```css
:root {
  --primary: hsl(217.2 91.2% 59.8%); /* Primary blue */
  --background: hsl(0 0% 100%); /* White background */
  /* ... other color variables */
}
