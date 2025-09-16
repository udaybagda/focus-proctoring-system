# Deployment Configuration

## Environment Variables Required

Create these environment variables in your deployment platform:

```env
# Server Configuration
PORT=3000
NODE_ENV=production

# MongoDB Configuration
MONGODB_URI=mongodb+srv://username:password@cluster.mongodb.net/video_proctoring

# Session Configuration
SESSION_SECRET=your_super_secret_key_here_change_this_in_production

# File Upload Configuration
MAX_FILE_SIZE=100MB
UPLOAD_PATH=./uploads
```

## Platform-Specific Notes

### Railway
- Automatically detects Node.js projects
- Supports MongoDB Atlas integration
- Free tier available with limitations

### Render
- Requires Procfile or package.json start script
- Supports MongoDB Atlas
- Free tier with sleep after inactivity

### Vercel
- Best for frontend deployment
- Use with Railway for backend
- Excellent for static sites
