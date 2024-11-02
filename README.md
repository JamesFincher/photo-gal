# Photosphere - Beautiful Photo Gallery

A modern, feature-rich photo gallery application built with Next.js, Clerk Authentication, and UploadThing for seamless photo management.

## Features

- 🔐 Secure authentication with Clerk
- 📸 Photo uploads with UploadThing
- 🎨 Beautiful UI with Tailwind CSS
- 🌓 Dark/Light mode support
- 📱 Fully responsive design
- ✨ Smooth animations with Framer Motion
- 🖼️ Album organization
- 📝 Photo descriptions and comments

## Prerequisites

Before you begin, ensure you have the following installed:
- Node.js 16.x or later
- npm or yarn

## Environment Variables

Create a `.env.local` file in the root directory with the following variables:

```env
# Clerk Authentication
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_test_your-publishable-key
CLERK_SECRET_KEY=sk_test_your-secret-key
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# UploadThing (for photo uploads)
UPLOADTHING_SECRET=sk_live_your-uploadthing-secret
UPLOADTHING_APP_ID=your-uploadthing-app-id
```

## Setup Instructions

1. Clone the repository:
```bash
git clone <repository-url>
cd photosphere
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
   - Create a new project on [Clerk Dashboard](https://dashboard.clerk.dev)
   - Create a new project on [UploadThing Dashboard](https://uploadthing.com)
   - Copy the required keys to your `.env.local` file

4. Run the development server:
```bash
npm run dev
```

5. Open [http://localhost:3000](http://localhost:3000) in your browser

## Project Structure

```
photosphere/
├── app/                    # Next.js app directory
│   ├── albums/            # Album management pages
│   ├── upload/            # Photo upload page
│   ├── layout.tsx         # Root layout
│   └── page.tsx           # Homepage
├── components/            # Reusable components
│   ├── ui/               # UI components
│   └── ...               # Feature components
├── lib/                  # Utility functions
├── public/               # Static assets
└── styles/              # Global styles
```

## Authentication Setup

1. Go to [Clerk Dashboard](https://dashboard.clerk.dev)
2. Create a new application
3. Copy the Publishable Key and Secret Key
4. Add them to your `.env.local` file

## Upload Setup

1. Create an account on [UploadThing](https://uploadthing.com)
2. Create a new project
3. Copy the API keys
4. Add them to your `.env.local` file

## Development

- Run development server: `npm run dev`
- Build for production: `npm run build`
- Start production server: `npm run start`
- Run linter: `npm run lint`

## Contributing

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/amazing-feature`
3. Commit your changes: `git commit -m 'Add amazing feature'`
4. Push to the branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.