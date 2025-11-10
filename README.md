# Collaborative Canvas

A real-time collaborative drawing web application built with Vanilla JavaScript, HTML5 Canvas, Node.js, and Socket.io.

## Setup Instructions

To get the project up and running on your local machine, follow these steps:

1.  **Clone the repository:**

    ```bash
    git clone <repository-url>
    cd collaborative-canvas
    ```

2.  **Install dependencies:**

    ```bash
    npm install
    ```

3.  **Start the development server:**

    ```bash
    npm start
    # Or for development with hot-reloading:
    # npm run dev
    ```

    The server will typically run on `http://localhost:3000`.

## Features

1. **Drawing Tools**:
   - Circle brush for smooth, natural strokes
   - Square brush for geometric and pixel-art style
   - Eraser tool with adjustable size
   - Color picker for unlimited colors
   - Adjustable stroke width

2. **Collaboration**:
   - Real-time multi-user drawing
   - Room-based collaboration system
   - Live cursor tracking
   - User presence indicators
   - Per-user color assignment

3. **Canvas Operations**:
   - Global undo/redo system
   - Drawing state persistence
   - Canvas clearing
   - Save/Load functionality

4. **Performance Features**:
   - FPS counter
   - Latency monitoring
   - Throttled updates
   - Optimized stroke rendering
   - Coordinate normalization

## Testing Multi-User Mode

1. Start the server using `npm start`
2. Open `http://localhost:3000` in your browser
3. Test with multiple users by:
   - Opening multiple browser windows
   - Using different browsers
   - Using incognito/private windows
   - Connecting from different devices on the same network
   
In multi-user mode, you'll see:
- Real-time drawing updates
- Other users' cursors
- Live user list updates
- Synchronized undo/redo
- Unique color per user

## Known Issues or Limitations

1. **Performance**:
   - Large drawings with many strokes may experience lag
   - Frame rate drops with complex strokes or many users
   - High network latency can affect real-time updates

2. **Drawing Synchronization**:
   - Brief disconnections may cause temporary state inconsistency
   - Long disconnections require page refresh
   - Simultaneous drawing in the same area may have visual artifacts

3. **Browser Compatibility**:
   - Pressure sensitivity only works on supported devices/browsers
   - Touch events may behave differently across browsers
   - Some mobile browsers may have rendering differences

4. **Data Persistence**:
   - Drawings are stored in server memory
   - Server restart clears all drawings
   - No automatic saving/backup mechanism

5. **Room Management**:
   - Room list is not persisted across server restarts
   - No password protection for rooms
   - Limited room discovery features

## Deployment

### Live Demo
You can try the application at: [https://collaborative-canvas-dz130nkda-raunakbansods-projects.vercel.app]([https://collaborative-canvas-dz130nkda-raunakbansods-projects.vercel.app](https://collaborative-canvas-es8u6rz4b-raunakbansods-projects.vercel.app/))

### Deployment Instructions

The application can be deployed to various platforms. Here are instructions for common platforms:

#### Vercel Deployment
1. Fork this repository
2. Import your fork to Vercel
3. Set the following:
   - Build Command: `npm install`
   - Output Directory: `client`
   - Install Command: `npm install`
   - Start Command: `npm start`

#### Heroku Deployment
1. Create a new Heroku app
2. Connect your GitHub repository
3. Add the following buildpacks:
   - heroku/nodejs
4. Set environment variables:
   - `NODE_ENV=production`
   - `PORT=process.env.PORT`
5. Deploy the main branch


## Time Spent on Development

Approximately 10-12 hours were spent on the initial development of this application, covering the setup, core drawing functionality, real-time synchronization, user management, undo/redo system, basic conflict resolution, canvas persistence, and performance metrics. This estimate includes time for planning, coding, and debugging.

## Repository Access and Submission

### GitHub Repository
The project is available at: [GitHub Repository Link](https://github.com/RaunakBansod/Collaborative-Canvas)
- For private repositories, please add the following users as collaborators:
  - @reviewer1
  - @reviewer2

### Submission Package
1. **GitHub Repository**
   - Complete source code
   - Documentation (README.md, ARCHITECTURE.md)
   - Commit history showing development progress

2. **Live Demo**
   - Deployed version accessible at [Demo URL]
   - Tested and verified working with multiple users


