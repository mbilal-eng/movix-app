# 🎬 Movix - Movie & TV Show Discovery App

A modern, responsive web application for discovering movies and TV shows using The Movie Database (TMDB) API. Built with React, Redux Toolkit, and Vite for optimal performance and user experience.

## 🌟 Live Preview

**🔗 [View Live Demo](https://movix-eta.vercel.app/)**

![Movix Screenshot](screenshot.png)

## ✨ Features

### 🎯 Core Functionality
- **Movie & TV Show Discovery**: Browse trending, popular, and top-rated content
- **Advanced Search**: Search for movies and TV shows with real-time results
- **Detailed Information**: Comprehensive movie/TV show details including cast, crew, ratings, and trailers
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Infinite Scroll**: Seamless browsing with infinite scroll pagination
- **Video Integration**: Watch trailers and clips directly in the app

### 🎨 User Interface
- **Hero Banner**: Dynamic background with featured content
- **Carousel Components**: Smooth scrolling content sections
- **Interactive Cards**: Hover effects and detailed movie cards
- **Genre Filtering**: Filter content by genres
- **Rating Display**: Visual rating indicators with circular progress bars
- **Lazy Loading**: Optimized image loading for better performance

### 🔧 Technical Features
- **State Management**: Redux Toolkit for efficient state management
- **API Integration**: Seamless TMDB API integration
- **Custom Hooks**: Reusable data fetching hooks
- **Error Handling**: Comprehensive error handling and loading states
- **Performance Optimization**: Lazy loading, image optimization, and code splitting

## 🛠️ Tech Stack

### Frontend
- **React 18** - Modern React with hooks and functional components
- **Redux Toolkit** - State management and data caching
- **React Router DOM** - Client-side routing
- **Axios** - HTTP client for API requests
- **Sass/SCSS** - CSS preprocessing for maintainable styles

### UI/UX Libraries
- **React Icons** - Comprehensive icon library
- **React Circular Progressbar** - Rating visualization
- **React Lazy Load Image Component** - Optimized image loading
- **React Infinite Scroll Component** - Infinite scroll functionality
- **React Player** - Video playback capabilities
- **React Select** - Enhanced select components

### Development Tools
- **Vite** - Fast build tool and development server
- **ESLint** - Code linting and formatting
- **Sass** - CSS preprocessing

## 🚀 Getting Started

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn package manager
- TMDB API key

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/movix.git
   cd movix
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Environment Setup**
   Create a `.env` file in the root directory:
   ```env
   VITE_APP_TMDB_TOKEN=your_tmdb_api_token_here
   ```

4. **Get TMDB API Key**
   - Visit [TMDB API](https://www.themoviedb.org/settings/api)
   - Create an account and request an API key
   - Add your API key to the `.env` file

5. **Start the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

6. **Open your browser**
   Navigate to `http://localhost:5173`

## 📁 Project Structure

```
movix/
├── public/
│   └── movix-logo.png
├── src/
│   ├── assets/                 # Static assets
│   ├── components/            # Reusable UI components
│   │   ├── carousel/          # Carousel components
│   │   ├── circleRating/      # Rating display
│   │   ├── contentWrapper/    # Layout wrapper
│   │   ├── footer/            # Footer component
│   │   ├── genres/            # Genre filtering
│   │   ├── header/            # Navigation header
│   │   ├── lazyLoadImage/     # Optimized image loading
│   │   ├── movieCard/         # Movie/TV show cards
│   │   ├── spinner/           # Loading indicators
│   │   ├── switchTabs/        # Tab switching
│   │   └── videoPopup/        # Video modal
│   ├── hooks/                 # Custom React hooks
│   │   └── useFetch.jsx       # Data fetching hook
│   ├── pages/                 # Page components
│   │   ├── 404/              # 404 error page
│   │   ├── details/          # Movie/TV show details
│   │   ├── explore/          # Browse by category
│   │   ├── home/             # Homepage
│   │   └── searchResult/     # Search results
│   ├── store/                # Redux store
│   │   ├── homeSlice.js      # Home state management
│   │   └── store.js          # Store configuration
│   ├── utils/                # Utility functions
│   │   └── api.js            # API configuration
│   ├── App.jsx               # Main app component
│   ├── main.jsx              # App entry point
│   └── index.scss            # Global styles
├── package.json
├── vite.config.js
└── README.md
```

## 🎯 Key Components

### 🏠 Home Page
- **Hero Banner**: Featured content with search functionality
- **Trending Section**: Currently trending movies and TV shows
- **Popular Section**: Most popular content
- **Top Rated Section**: Highest rated content

### 🔍 Search & Discovery
- **Global Search**: Search across movies and TV shows
- **Advanced Filtering**: Filter by genre, year, rating
- **Search Results**: Paginated search results with infinite scroll

### 📱 Details Page
- **Movie/TV Show Information**: Comprehensive details
- **Cast & Crew**: Actor and crew information
- **Trailers & Videos**: Embedded video content
- **Similar Content**: Recommendations based on current content
- **Reviews & Ratings**: User reviews and ratings

### 🎨 UI Components
- **Responsive Header**: Navigation with mobile menu
- **Interactive Cards**: Hover effects and smooth transitions
- **Loading States**: Skeleton loaders and spinners
- **Error Handling**: User-friendly error messages

## 🔧 API Integration

The app integrates with The Movie Database (TMDB) API to fetch:

- **Movie Data**: Popular, trending, top-rated movies
- **TV Show Data**: Popular, trending, top-rated TV shows
- **Search Results**: Real-time search functionality
- **Details**: Comprehensive movie/TV show information
- **Cast & Crew**: Actor and crew details
- **Videos**: Trailers and clips
- **Images**: Posters, backdrops, and profile images

## 🎨 Design Features

- **Modern UI**: Clean, contemporary design
- **Responsive Layout**: Mobile-first approach
- **Smooth Animations**: CSS transitions and hover effects
- **Dark Theme**: Eye-friendly dark color scheme
- **Typography**: Readable fonts and proper hierarchy
- **Accessibility**: WCAG compliant design

## 🚀 Performance Optimizations

- **Lazy Loading**: Images and components load on demand
- **Code Splitting**: Route-based code splitting
- **Caching**: Redux state caching for API responses
- **Image Optimization**: Optimized image sizes and formats
- **Bundle Optimization**: Vite's optimized build process

## 📱 Responsive Design

The app is fully responsive and optimized for:
- **Desktop**: Full-featured experience
- **Tablet**: Touch-optimized interface
- **Mobile**: Mobile-first design with touch gestures

## 🔒 Environment Variables

Create a `.env` file with the following variables:

```env
VITE_APP_TMDB_TOKEN=your_tmdb_api_token_here
```

## 📦 Build & Deployment

### Build for Production
```bash
npm run build
```

### Preview Production Build
```bash
npm run preview
```

### Deploy to Vercel
1. Connect your GitHub repository to Vercel
2. Add environment variables in Vercel dashboard
3. Deploy automatically on push to main branch

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [The Movie Database (TMDB)](https://www.themoviedb.org/) for providing the API
- [React](https://reactjs.org/) for the amazing framework
- [Vite](https://vitejs.dev/) for the fast build tool
- [Redux Toolkit](https://redux-toolkit.js.org/) for state management

## 📞 Support

If you have any questions or need help, please:
- Open an issue on GitHub
- Contact the maintainers
- Check the documentation

---

**Made with ❤️ by Muhammad Bilal**
