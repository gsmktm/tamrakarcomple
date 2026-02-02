# 🚀 Vercel Deployment Instructions for Tamrakar Complex

## Step 1: Push to GitHub
First, let's get your code to GitHub so Vercel can access it.

```bash
# Initialize git repository (if not already done)
git init
git add .
git commit -m "Deploy Tamrakar Complex tech news website"

# Create a new repository on GitHub first, then:
git remote add origin https://github.com/YOUR_USERNAME/tamrakarcomplex.git
git branch -M main
git push -u origin main
```

## Step 2: Deploy on Vercel

### Option A: Using Vercel CLI (Fastest)
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy to production
vercel --prod
```

### Option B: Using Vercel Dashboard
1. Go to [vercel.com](https://vercel.com)
2. Click "New Project"
3. Import your GitHub repository
4. Vercel will automatically detect it's a Next.js app

## Step 3: Set Environment Variables
In Vercel dashboard, add these environment variables:

```
DATABASE_URL=your_production_database_url
JWT_SECRET=your_very_secure_random_secret_key
ADMIN_EMAIL=admin@tamrakarcomplex.com
ADMIN_PASSWORD=your_secure_admin_password
```

## Database Options

### Option 1: Use Vercel Postgres (Recommended)
1. In Vercel dashboard, go to Storage
2. Create a new Postgres database
3. Copy the connection string
4. Use it for `DATABASE_URL`

### Option 2: External PostgreSQL
1. Create PostgreSQL database (Railway, Supabase, etc.)
2. Get connection string
3. Add to environment variables

### Option 3: Keep SQLite (Not recommended for production)
- Use the existing SQLite file
- Limited scalability

## Step 4: Deploy and Test
1. Click "Deploy" in Vercel
2. Wait for deployment to complete
3. Visit your new URL
4. Test all features:
   - Homepage loads
   - Admin panel works (`/admin`)
   - News, Reviews, Guides pages
   - Search functionality

## Production Setup Checklist

After deployment:
- [ ] Update admin credentials in production
- [ ] Test all pages load correctly
- [ ] Verify database connections
- [ ] Test content creation in admin
- [ ] Check mobile responsiveness
- [ ] Set up custom domain (optional)

## Troubleshooting

### Build Errors
- Check environment variables are set correctly
- Ensure database connection is valid
- Verify all dependencies are installed

### Database Issues
- Run `npx prisma migrate deploy` if needed
- Check database URL format
- Ensure database is accessible

### Performance Issues
- Enable Vercel Analytics
- Check bundle size in Vercel dashboard
- Optimize images if needed

## Success! 🎉

Once deployed, your Tamrakar Complex site will be live at:
`https://your-project-name.vercel.app`

You'll have a fully functional tech news website with:
- Modern responsive design
- Complete admin panel
- News, reviews, and guides sections
- Search functionality
- Newsletter signup
- Professional tech news features

Ready to deploy? Start with Step 1!
