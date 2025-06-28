# Deployment Guide

## Replit Deployment (Recommended)

Mentora is optimized for Replit's deployment platform with zero-configuration setup.

### Steps
1. **Import Repository**
   - Go to [Replit](https://replit.com)
   - Click "Create Repl" → "Import from GitHub"
   - Enter your repository URL

2. **Configure Secrets**
   - In your Repl, go to the "Secrets" tab
   - Add: `VITE_GEMINI_API_KEY` with your Google Gemini API key
   - Add: `SESSION_SECRET` with a random string

3. **Deploy**
   - Click the "Deploy" button in your Repl
   - Your app will be live at `https://your-repl-name.your-username.repl.co`

### Features
- Automatic HTTPS
- Custom domain support
- Health checks
- Auto-scaling
- Zero-downtime deployments

## Manual Deployment

### Prerequisites
- Node.js 18+
- PostgreSQL (optional)
- Process manager (PM2 recommended)

### Build and Deploy
```bash
# Clone and install
git clone https://github.com/yourusername/mentora.git
cd mentora
npm install

# Set environment variables
cp .env.example .env
# Edit .env with your values

# Build the application
npm run build

# Start with PM2
npm install -g pm2
pm2 start dist/index.js --name mentora

# Or start directly
npm start
```

### Environment Variables
```env
# Required
VITE_GEMINI_API_KEY=your_gemini_api_key
NODE_ENV=production
SESSION_SECRET=your_session_secret

# Optional
DATABASE_URL=postgresql://user:pass@host:port/db
PORT=5000
```

## Platform-Specific Guides

### Vercel
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel

# Set environment variables in Vercel dashboard
```

### Netlify
```bash
# Build command: npm run build
# Publish directory: dist
# Set environment variables in Netlify dashboard
```

### Railway
```bash
# Connect GitHub repository
# Set environment variables
# Deploy automatically on push
```

### DigitalOcean App Platform
1. Connect GitHub repository
2. Set build command: `npm run build`
3. Set run command: `npm start`
4. Configure environment variables

## Database Setup

### PostgreSQL (Production)
```bash
# Create database
createdb mentora_production

# Set DATABASE_URL
export DATABASE_URL="postgresql://user:password@localhost:5432/mentora_production"

# Push schema
npm run db:push
```

### Memory Storage (Development)
No additional setup required - uses in-memory storage by default.

## Health Checks

The application provides health check endpoints:

- `GET /health` - Basic health check
- `GET /api/health` - API health check

Example response:
```json
{
  "status": "ok",
  "timestamp": "2025-01-01T00:00:00.000Z",
  "uptime": 3600
}
```

## Monitoring

### Logs
```bash
# View logs (PM2)
pm2 logs mentora

# View logs (Docker)
docker logs mentora

# View logs (Railway/Vercel)
# Check platform dashboard
```

### Performance
- Monitor response times
- Track API usage (Gemini)
- Monitor memory usage
- Check error rates

## Security

### Environment Variables
- Never commit `.env` files
- Use platform-specific secret management
- Rotate API keys regularly
- Use strong session secrets

### HTTPS
- Always use HTTPS in production
- Replit provides automatic HTTPS
- Configure SSL certificates for manual deployments

### Rate Limiting
The application includes basic rate limiting for AI endpoints.

## Scaling

### Horizontal Scaling
- Application is stateless (except session storage)
- Can run multiple instances behind load balancer
- Use external session store (Redis) for multiple instances

### Database Scaling
- PostgreSQL supports read replicas
- Consider connection pooling for high traffic
- Monitor query performance

## Troubleshooting

### Common Issues

**Build fails:**
- Check Node.js version (18+ required)
- Verify all dependencies install correctly
- Check TypeScript compilation

**App won't start:**
- Verify environment variables
- Check port availability
- Review application logs

**AI features not working:**
- Verify Gemini API key
- Check API quotas/limits
- Review network connectivity

**Database connection issues:**
- Verify DATABASE_URL format
- Check database server status
- Review connection permissions

### Debug Mode
```bash
# Enable debug logging
NODE_ENV=development npm start

# Or set debug flag
DEBUG=* npm start
```

## Performance Optimization

### Frontend
- Static assets are cached
- Code splitting enabled
- Lazy loading for components

### Backend
- Response compression enabled
- Static file serving optimized
- Database query optimization

### CDN (Optional)
Consider using a CDN for static assets in high-traffic scenarios.

## Backup Strategy

### Database Backups
```bash
# PostgreSQL backup
pg_dump $DATABASE_URL > backup.sql

# Restore
psql $DATABASE_URL < backup.sql
```

### Application Backups
- Source code in Git
- Environment variables documented
- Deployment configuration saved

## Support

For deployment issues:
- Check [GitHub Issues](https://github.com/yourusername/mentora/issues)
- Review platform-specific documentation
- Contact platform support for infrastructure issues