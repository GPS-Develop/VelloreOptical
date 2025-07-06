# Vellore Optical

A modern, professional website for Vellore Optical - an eyewear store located in Vaughan, Ontario. Features include virtual try-on technology, online appointment booking, and comprehensive eyewear information.

## 🌟 Features

- **Virtual Try-On**: AI-powered face tracking using MediaPipe for real-time eyewear fitting
- **Online Appointment Booking**: Integrated Calendly scheduling system
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Insurance Information**: Direct billing support with major insurance providers
- **Eyewear Tips**: Educational content about eyewear care and selection
- **Contact Integration**: WhatsApp button and Instagram social links

## 🚀 Live Demo

Visit the live site: [https://velloreoptical.com](https://velloreoptical.com)

## 📱 Screenshots

*Virtual Try-On Experience*
- Real-time face tracking and frame overlay
- Multiple frame options with custom scaling
- Photo capture functionality

*Store Information*
- Interactive Google Maps integration
- Business hours and contact details
- Insurance provider logos

## 🛠️ Built With

- **Framework**: [Next.js 15](https://nextjs.org/) with App Router
- **Styling**: [Tailwind CSS 4](https://tailwindcss.com/)
- **AI/ML**: [MediaPipe Tasks Vision](https://developers.google.com/mediapipe) for face landmarks
- **Typography**: [Geist Font](https://vercel.com/font) by Vercel
- **Email**: [Nodemailer](https://nodemailer.com/) for appointment notifications
- **Scheduling**: [Calendly](https://calendly.com/) integration
- **Language**: TypeScript for type safety

## 🏗️ Project Structure

```
src/
├── app/
│   ├── api/
│   │   └── book-appointment/     # Email notification API
│   ├── components/
│   │   ├── BookingCalendar.tsx   # Calendly integration
│   │   ├── NavBar.tsx           # Navigation component
│   │   ├── VirtualTryOn.tsx     # AI-powered try-on feature
│   │   └── WhatsAppButton.tsx   # Contact button
│   ├── book-appointment/        # Appointment booking page
│   ├── eyewear-tips/           # Educational content
│   ├── virtual-try-on/         # Virtual try-on page
│   ├── globals.css             # Global styles
│   ├── layout.tsx              # Root layout
│   └── page.tsx                # Homepage
├── public/
│   ├── frames/                 # Eyewear frame images
│   ├── models/                 # AI model files
│   └── ...                     # Other static assets
└── ...
```

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ 
- npm or yarn
- Git

### Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/vellore-optical.git
cd vellore-optical
```

2. Install dependencies
```bash
npm install
# or
yarn install
```

3. Set up environment variables
```bash
cp .env.example .env.local
```

Add your environment variables:
```env
GMAIL_USER=your-email@gmail.com
GMAIL_PASS=your-app-password
GMAIL_TO=appointments@velloreoptical.com
```

4. Run the development server
```bash
npm run dev
# or
yarn dev
```

5. Open [http://localhost:3000](http://localhost:3000) in your browser

## 📧 Email Configuration

For appointment notifications to work, you'll need to:

1. Create a Gmail App Password:
   - Go to Google Account settings
   - Enable 2-factor authentication
   - Generate an App Password for "Mail"

2. Update environment variables with your credentials

## 🎨 Customization

### Adding New Frames

1. Add frame images to `public/frames/`
2. Update the `frames` array in `src/app/components/VirtualTryOn.tsx`:

```typescript
const frames = [
  {
    id: 'new-frame',
    name: 'New Frame Style',
    imageUrl: '/frames/new-frame.png',
    scaleFactor: 1.5, // Optional: adjust fit
  },
  // ... other frames
];
```

### Customizing Store Information

Update store details in `src/app/page.tsx`:
- Address and contact information
- Business hours
- Google Maps embed URL
- Insurance provider logos

## 🔧 Available Scripts

```bash
# Development
npm run dev          # Start development server
npm run build        # Build for production
npm run start        # Start production server
npm run lint         # Run ESLint

# Additional scripts
npm run type-check   # Run TypeScript compiler
npm run analyze      # Analyze bundle size
```

## 🌐 Deployment

### Vercel (Recommended)

1. Connect your GitHub repository to Vercel
2. Add environment variables in Vercel dashboard
3. Deploy automatically on every push to main

### Other Platforms

The app can be deployed to any platform that supports Next.js:
- Netlify
- Railway
- DigitalOcean App Platform
- AWS Amplify

## 📊 Performance

- **Lighthouse Score**: 95+ across all metrics
- **Core Web Vitals**: Optimized for LCP, FID, and CLS
- **Mobile Optimized**: Responsive design with touch interactions
- **SEO Ready**: Meta tags, structured data, and sitemap

## 🔒 Security

- Input validation on all forms
- HTTPS enforcement
- Secure environment variable handling
- CSP headers for XSS protection

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Contact

**Vellore Optical**
- Address: 10385 Weston Rd, Vaughan, ON L4H 3T4
- Phone: (365) 418-7055
- Instagram: [@velloreoptical](https://www.instagram.com/velloreoptical/)
- Website: [velloreoptical.com](https://velloreoptical.com)

## 🙏 Acknowledgments

- [MediaPipe](https://developers.google.com/mediapipe) for face detection technology
- [Vercel](https://vercel.com) for hosting and font optimization
- [Tailwind CSS](https://tailwindcss.com) for styling framework
- [Next.js](https://nextjs.org) for the React framework

---

*Built with ❤️ for the Vellore Optical community*