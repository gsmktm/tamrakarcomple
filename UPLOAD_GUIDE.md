# 📁 FILES TO UPLOAD TO GITHUB

## ✅ Essential Files (Must Upload):

### Core Project Files:
- ✅ `package.json` - Dependencies and scripts
- ✅ `package-lock.json` - Lock file for exact versions
- ✅ `next.config.js` - Next.js configuration
- ✅ `tsconfig.json` - TypeScript configuration
- ✅ `tailwind.config.ts` - Tailwind CSS config
- ✅ `postcss.config.js` - PostCSS config
- ✅ `next-env.d.ts` - Next.js types

### Source Code:
- ✅ `src/` folder (entire folder)
  - `app/` - All pages and API routes
  - `components/` - React components
  - `lib/` - Utilities and Prisma client

### Database:
- ✅ `prisma/` folder (entire folder)
  - `schema.prisma` - Database schema
  - `migrations/` - Database migrations
  - `seed.ts` - Seed data

### Configuration:
- ✅ `vercel.json` - Vercel deployment config
- ✅ `netlify.toml` - Netlify config (optional)
- ✅ `.env.example` - Environment variables template
- ✅ `.gitignore` - Git ignore rules

### Documentation:
- ✅ `README.md` - Project documentation
- ✅ `DEPLOYMENT.md` - Deployment guide

## ❌ DO NOT Upload:

- `node_modules/` - (Too large, will be installed)
- `.next/` - (Build folder, will be generated)
- `.env` - (Contains secrets)
- `.DS_Store` - (Mac system file)
- `dev.db` - (Database file, will be created)

## 🚀 Quick Upload Steps:

### 1. Create GitHub Repository
1. Go to [github.com](https://github.com)
2. Click "New repository"
3. Name: `tamrakarcomplex`
4. Public or Private (your choice)
5. Click "Create repository"

### 2. Upload Files
1. Click "uploading an existing file"
2. Drag and drop ALL the ✅ files listed above
3. Make sure to include hidden files like `.gitignore`
4. Commit changes: "Deploy Tamrakar Complex tech news website"
5. Click "Commit changes"

### 3. Verify Upload
Check that these folders are uploaded:
- `src/` (with all subfolders)
- `prisma/` (with schema and migrations)
- Root configuration files

## 📋 Upload Checklist:

### Required Files:
- [ ] `package.json`
- [ ] `package-lock.json`
- [ ] `next.config.js`
- [ ] `vercel.json`
- [ ] `.env.example`
- [ ] `.gitignore`
- [ ] `README.md`
- [ ] `src/` folder
- [ ] `prisma/` folder

### Optional Files:
- [ ] `netlify.toml`
- [ ] `tailwind.config.ts`
- [ ] `tsconfig.json`
- [ ] `postcss.config.js`

### Exclude Files:
- [ ] `node_modules/` ❌
- [ ] `.next/` ❌
- [ ] `.env` ❌
- [ ] `.DS_Store` ❌
- [ ] `dev.db` ❌

## 🎯 After Upload:

1. **Go to Vercel**
   - Visit [vercel.com](https://vercel.com)
   - Import your repository
   - Set environment variables
   - Deploy!

2. **Environment Variables Needed:**
   ```
   DATABASE_URL=your_database_url
   JWT_SECRET=your_very_secure_secret_key
   ADMIN_EMAIL=admin@tamrakarcomplex.com
   ADMIN_PASSWORD=your_secure_admin_password
   ```

## ⚡ **Ready to Upload!**

Select all the ✅ files above and upload them to your new GitHub repository. Your Tamrakar Complex will be live in minutes!
