# Portfolio Website - Vercel Deployment

A modern, responsive portfolio website built with Next.js, React, and TypeScript.

## Features

- 🎨 Modern UI with Framer Motion animations
- 🌙 Dark/Light theme support
- 💬 AI-powered chatbot using Google Gemini
- 📱 Fully responsive design
- ⚡ Optimized performance

## Tech Stack

- **Framework**: Next.js 16
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **Animations**: Framer Motion
- **UI Components**: Radix UI, shadcn/ui
- **AI**: Google Generative AI (Gemini)

## Local Development

1. Install dependencies:
```bash
npm install
```

2. Create a `.env.local` file and add your environment variables:
```
GEMINI_API_KEY=your_gemini_api_key_here
```

3. Run the development server:
```bash
npm run dev
```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

## Deployment on Vercel

### Prerequisites
- A GitHub account
- A Vercel account (free tier available)
- Google Gemini API key

### Quick Deploy

The easiest way to deploy is using the Vercel CLI or through the Vercel Dashboard.

#### Option 1: Deploy via Vercel Dashboard (Recommended)

1. **Push to GitHub**
   - Create a new repository on GitHub
   - Push this project to your repository

2. **Deploy on Vercel**
   - Go to [vercel.com](https://vercel.com)
   - Click "Add New..." → "Project"
   - Import your GitHub repository
   - Vercel will auto-detect Next.js settings
   - Add environment variable: `GEMINI_API_KEY` with your API key
   - Click "Deploy"

3. **Your site will be live in seconds!**

#### Option 2: Deploy via Vercel CLI

1. Install Vercel CLI:
```bash
npm i -g vercel
```

2. Deploy:
```bash
vercel
```

3. Follow the prompts and add your `GEMINI_API_KEY` when asked.

### Environment Variables

Add these in Vercel Dashboard → Project Settings → Environment Variables:

| Variable | Description | Required |
|----------|-------------|----------|
| `GEMINI_API_KEY` | Google Gemini API key for chatbot | Yes |

**Note**: Vercel automatically sets `NODE_ENV` and `PORT`, so you don't need to configure them.

### Build Settings (Auto-detected by Vercel)

- **Framework Preset**: Next.js
- **Build Command**: `next build` (auto-detected)
- **Output Directory**: `.next` (auto-detected)
- **Install Command**: `npm install` (auto-detected)

## Project Structure

```
portfolio-render/
├── app/              # Next.js app directory
│   ├── api/         # API routes
│   └── ...
├── components/      # React components
│   ├── sections/    # Page sections
│   ├── ui/         # UI components
│   └── ...
├── data/           # Data files
├── lib/            # Utility functions
├── public/         # Static assets
└── vercel.json     # Vercel configuration
```

## Custom Domain

1. Go to your project in Vercel Dashboard
2. Click "Settings" → "Domains"
3. Add your custom domain
4. Follow DNS configuration instructions

## Updating Your Site

1. Make changes to your code
2. Commit and push to GitHub:
```bash
git add .
git commit -m "Your update message"
git push
```
3. Vercel will automatically detect changes and redeploy

## Troubleshooting

### Build Fails
- Check build logs in Vercel Dashboard
- Ensure all dependencies are in `package.json`
- Verify Node.js version (>=20.9.0)

### Chatbot Not Working
- Verify `GEMINI_API_KEY` is set in Vercel environment variables
- Check API key is valid and has credits
- Review function logs in Vercel Dashboard

### Environment Variables Not Working
- Make sure variables are added in Vercel Dashboard
- Redeploy after adding new environment variables
- Check variable names match exactly (case-sensitive)

## Support

- Vercel Documentation: [vercel.com/docs](https://vercel.com/docs)
- Next.js Documentation: [nextjs.org/docs](https://nextjs.org/docs)
- Vercel Support: [vercel.com/support](https://vercel.com/support)

## License

Private project - All rights reserved

