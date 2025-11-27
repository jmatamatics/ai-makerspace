# 🧠 AI Mental Coach - Frontend

A beautiful, modern Next.js frontend for your AI-powered mental coaching application! This app connects to a FastAPI backend and provides a sleek chat interface for users to interact with their supportive AI coach.

## 🎨 Features

- 💬 **Real-time Chat Interface** - Beautiful, responsive chat UI
- 🎭 **Message History** - Keep track of your conversation
- ⚡ **Fast & Modern** - Built with Next.js 14 and React 18
- 📱 **Responsive Design** - Works great on desktop, tablet, and mobile
- 🌈 **Beautiful Gradients** - Eye-catching purple gradient theme
- ♿ **Accessible** - Built with accessibility in mind

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ installed on your machine
- The FastAPI backend running on `http://localhost:8000` (see `/api` folder)

### Installation

1. **Install dependencies:**

```bash
cd frontend
npm install
```

2. **Run the development server:**

```bash
npm run dev
```

3. **Open your browser:**

Navigate to [http://localhost:3000](http://localhost:3000)

You should see your AI Mental Coach app! 🎉

## 🛠️ Available Scripts

- `npm run dev` - Start the development server on port 3000
- `npm run build` - Build the production-ready app
- `npm start` - Start the production server (run `build` first)
- `npm run lint` - Run ESLint to check for code issues

## 📦 Tech Stack

- **Next.js 14** - React framework with App Router
- **React 18** - UI library
- **TypeScript** - Type safety
- **CSS** - Custom styling with gradients and animations

## 🔗 API Integration

The frontend connects to your FastAPI backend via the `/api/chat` endpoint. The connection is proxied through Next.js configuration to avoid CORS issues during development.

**Backend URL (development):** `http://localhost:8000/api/chat`

Make sure your backend is running before starting the frontend!

## 🎨 Customization

Want to customize the look and feel? Check out:

- `app/globals.css` - Global styles, colors, and theme
- `app/page.tsx` - Main chat interface component
- `app/layout.tsx` - Root layout and metadata

Feel free to change the gradient colors, fonts, or layout to match your style! 💅

## 📝 Project Structure

```
frontend/
├── app/
│   ├── globals.css      # Global styles
│   ├── layout.tsx       # Root layout
│   └── page.tsx         # Main chat page
├── public/              # Static assets
├── next.config.js       # Next.js configuration
├── package.json         # Dependencies
├── tsconfig.json        # TypeScript config
└── README.md           # This file!
```

## 🐛 Troubleshooting

### "Failed to get response" error

Make sure your FastAPI backend is running:

```bash
cd ..
uv run uvicorn api.index:app --reload
```

### Port 3000 already in use

Kill the process on port 3000:

```bash
lsof -ti:3000 | xargs kill -9
```

Or run Next.js on a different port:

```bash
npm run dev -- -p 3001
```

## 🚀 Deploying to Vercel

This app is ready to deploy to Vercel!

1. Push your code to GitHub
2. Import your repository on [vercel.com](https://vercel.com)
3. Set the root directory to `frontend`
4. Add your environment variables (if any)
5. Deploy! 🎉

Vercel will automatically detect Next.js and configure everything for you.

## 📚 Learn More

- [Next.js Documentation](https://nextjs.org/docs)
- [React Documentation](https://react.dev)
- [TypeScript Documentation](https://www.typescriptlang.org/docs)
- [Vercel Deployment](https://vercel.com/docs)

## 💡 Built with AI

This frontend was created following AI Maker Space's Beyond-ChatGPT course guidelines. Special shoutout to the power of AI-assisted development! 🤖✨

---

Made with ❤️ and ☕ by [Your Name]
