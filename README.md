# Video Carousel Application

A responsive, accessible video carousel built with React and TypeScript, featuring smooth navigation, custom controls, and pixel-perfect design implementation.

## Overview

This application implements a sophisticated video carousel component that displays multiple videos with seamless navigation and interactive controls. Built to exact Figma specifications with comprehensive accessibility support and mobile optimization.

## Features

### Core Functionality
- **Auto-Play**: First video starts automatically on page load
- **Infinite Scrolling**: Seamless navigation without endpoints
- **Smart Navigation**: Multiple input methods (arrows, keyboard, mouse wheel, touch)
- **Active Video Focus**: Only current video is interactive with visual indication
- **Custom Controls**: Play/pause/mute buttons using SVG background images
- **Fallback System**: Multiple video sources for maximum reliability

### User Experience
- **Responsive Design**: Works perfectly across all device sizes
- **Touch Optimized**: Mobile-friendly with proper touch event handling
- **Keyboard Navigation**: Full keyboard accessibility (←, →, Space, M, Home, End)
- **Visual Feedback**: Clear indication of active video and control states
- **Loading States**: Smooth loading animations and error handling

### Technical Excellence
- **TypeScript**: Full type safety throughout the application
- **Performance Optimized**: Efficient rendering and memory management
- **Accessibility**: WCAG compliant with screen reader support
- **Browser Compatible**: Works across all modern browsers
- **Clean Architecture**: Modular components with separation of concerns

## Quick Start

### Prerequisites
- Node.js 18.0.0 or higher
- npm 8.0.0 or higher

### Installation
```bash
# Clone the repository
git clone <repository-url>
cd carousel-app

# Install dependencies
npm install

# Start development server
npm run dev
```

### Available Scripts
```bash
npm run dev      # Start development server
npm run build    # Build for production
npm run preview  # Preview production build
npm run lint     # Run ESLint
```

### Project Structure
```
src/
├── components/          # React components
│   ├── Carousel/        # Main carousel component
│   ├── VideoPlayer/     # Video player with custom controls
│   └── NavigationArrows/ # Navigation arrow buttons
├── styles/              # Global styles and fonts
├── types/               # TypeScript type definitions
├── utils/               # Utility functions
├── App.tsx             # Main application component
└── main.tsx            # Application entry point
```

### Component Hierarchy
```
App
└── Carousel
    ├── NavigationArrows (in header)
    └── VideoPlayer[] (array of video players)
```


### Layout Specifications (Figma Compliant)
- **Container**: 1440px × 732px
- **Padding**: 40px 80px 80px 80px
- **Video Cards**: 300px × 532px
- **Gap**: 32px between elements

### Typography
- **Primary Font**: Haffer XH (headers, UI elements)


### Navigation Methods
1. **Header Arrows**: Click left/right arrows in carousel header
2. **Keyboard Shortcuts**:
   - `←` / `→`: Navigate between videos
   - `Space`: Play/pause active video
   - `M`: Mute/unmute active video
   - `Home`: Jump to first video
   - `End`: Jump to last video
3. **Mouse Wheel**: Scroll up/down to navigate
4. **Touch Gestures**: Swipe left/right on mobile
5. **Click to Focus**: Click any video to make it active

### Video Controls
- **Play/Pause**: Circular button with play/pause icon
- **Mute/Unmute**: Circular button with sound on/off icon
- **Progress Bar**: Seek through video timeline
- **Time Display**: Current time / total duration

## Mobile Optimization

### Touch Handling
- **Swipe Navigation**: Natural left/right swipe gestures
- **Touch Isolation**: Control buttons don't trigger carousel navigation
- **Proper Touch Targets**: Minimum 44px touch targets
- **Gesture Support**: Standard mobile interaction patterns

### Responsive Breakpoints
- **Desktop**: 1200px+ (full Figma layout)
- **Tablet**: 768px - 1199px (adapted layout)
- **Mobile**: < 768px (mobile-optimized layout)


### Keyboard Navigation
- Full keyboard support for all interactions
- Logical tab order and focus management
- Clear focus indicators

### Screen Reader Support
- Semantic HTML structure
- ARIA labels and descriptions
- Live region announcements
- Proper heading hierarchy

### Visual Accessibility
- High contrast mode support
- Reduced motion preferences
- Color-independent information
- Clear visual feedback

## Technical Implementation

### State Management
- **Carousel State**: Current index, transition status
- **Video State**: Playback status, loading states, error handling
- **Touch State**: Touch tracking for gesture recognition

### Performance Optimizations
- **Lazy Loading**: Videos load metadata only when needed
- **Debounced Events**: Optimized scroll and resize handlers
- **Memory Management**: Proper cleanup of event listeners
- **Efficient Rendering**: Minimized re-renders with React hooks

### Error Handling
- **Fallback Sources**: Multiple video sources per item
- **Graceful Degradation**: Continues working if some videos fail
- **User Feedback**: Clear error states with retry options
- **Console Logging**: Detailed error information for debugging



## Dependencies

### Development Dependencies
- **TypeScript**: 5.8.3 - Type safety
- **Vite**: 7.1.6 - Build tool
- **ESLint**: 9.35.0 - Code linting

## Key Features Implemented

### Requirements Met
- [x] Auto-play first video on page load
- [x] Left/right arrow navigation with infinite scrolling
- [x] Only active video is interactive
- [x] Visual indication of focused video
- [x] Fully responsive design
- [x] Pixel-perfect Figma implementation
- [x] Clean, maintainable React + TypeScript code

### Bonus Features
- [x] Multiple navigation methods (keyboard, mouse wheel, touch)
- [x] Custom video controls with SVG icons
- [x] Fallback video sources for reliability
- [x] Loading states and error handling
- [x] Mobile-optimized touch interactions
- [x] Comprehensive accessibility support
- [x] Performance optimizations
- [x] Browser compatibility

## Deployment

### Build for Production
```bash
npm run build
```

