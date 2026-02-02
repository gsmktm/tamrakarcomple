# Tamrakar Complex - Tech News Magazine

A modern tech news and review website built with Next.js, Prisma, and Tailwind CSS.

## Features

- 📰 **Content Management**: News, Reviews, Guides, Editorials
- 🏪 **Product Catalog**: Brands, products, specifications
- 📊 **Price Tracking**: Multi-region price monitoring
- ⭐ **Review System**: Ratings, pros/cons, verdicts
- 🔍 **Advanced Search**: Full-text search across all content
- 📱 **Responsive Design**: Mobile-optimized interface
- 🎨 **Modern UI**: Clean, professional tech news design

## Tech Stack

- **Frontend**: Next.js 14 (App Router)
- **Styling**: Tailwind CSS
- **Database**: SQLite with Prisma ORM
- **Authentication**: JWT-based admin system
- **Deployment**: Vercel/Netlify ready

## Quick Start

1. **Install dependencies**
   ```bash
   npm install
   ```

2. **Set up environment variables**
   ```bash
   cp .env.example .env
   # Edit .env with your configuration
   ```

3. **Set up database**
   ```bash
   npx prisma migrate dev
   npx prisma db:seed
   ```

4. **Start development server**
   ```bash
   npm run dev
   ```

5. **Open [http://localhost:3000](http://localhost:3000)**

## Admin Access

- URL: `/admin`
- Email: `admin@tamrakarcomplex.com`
- Password: `admin123`

## Project Structure

```
src/
├── app/                    # Next.js App Router pages
│   ├── (site)/           # Public pages
│   │   ├── news/          # News listing
│   │   ├── reviews/       # Reviews listing
│   │   ├── guides/        # Buying guides
│   │   └── search/        # Search page
│   ├── admin/            # Admin panel
│   └── api/              # API routes
├── components/           # Reusable React components
├── lib/                 # Utilities and configurations
└── prisma/              # Database schema and migrations
```

## Deployment

### Vercel (Recommended)

1. Push your code to GitHub
2. Connect your repository to Vercel
3. Set environment variables in Vercel dashboard:
   ```
   DATABASE_URL=your_database_url
   JWT_SECRET=your_jwt_secret
   ADMIN_EMAIL=your_admin_email
   ADMIN_PASSWORD=your_admin_password
   ```
4. Deploy!

### Netlify

1. Build the application:
   ```bash
   npm run build
   ```

2. Deploy the `out` folder to Netlify
3. Set environment variables in Netlify dashboard

### Traditional Hosting

1. Build the application:
   ```bash
   npm run build
   npm start
   ```

2. Upload to your hosting provider

## Environment Variables

```env
DATABASE_URL="file:./dev.db"
JWT_SECRET="your-secret-key-change-this-in-production"
ADMIN_EMAIL="admin@tamrakarcomplex.com"
ADMIN_PASSWORD="admin123"
```

## Database

The application uses SQLite for development. For production, consider:

- **PostgreSQL** (recommended for scaling)
- **MySQL** 
- **PlanetScale** (serverless PostgreSQL)

To switch databases, update the `provider` in `prisma/schema.prisma` and update the `DATABASE_URL`.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

MIT License - see LICENSE file for details.
