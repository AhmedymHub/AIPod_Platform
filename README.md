#AI Podcast Platform
Overview
The AI Podcast Platform is a web application that enables users to create podcasts effortlessly using AI technology. Users can select from various AI-generated voices, input a text prompt, and have the platform generate a high-quality podcast. Additionally, the platform provides automatic podcast thumbnail generation and seamless playback, making it a one-stop solution for podcast creators.

Features
AI Voice Selection: Choose from multiple AI-generated voices for your podcast.
Text-to-Audio Conversion: Enter a text prompt, and the AI generates the podcast in real-time.
Automatic Thumbnail Generation: Generate podcast thumbnails automatically using AI image generation.
Seamless Playback: Listen to generated podcasts with an integrated audio player.
Podcast Publishing: Easily submit and publish podcasts on the platform.
Tech Stack
Frontend: Next.js, TypeScript, SCSS, JSX
Backend: Convex API
AI Integration: OpenAI for text-to-audio conversion
File Upload: Cloudinary (for podcast and image uploads)
Authentication: Clerk
Styling: TailwindCSS, Shadcn
Payments: Stripe (for premium features)
Storage: MongoDB (for data storage)
Installation
Prerequisites
Before you begin, ensure you have met the following requirements:

Node.js (v16 or later)
MongoDB
Convex CLI
Stripe API Keys
Clerk API Keys
Cloudinary Account
Steps to Install
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/ai-podcast-platform.git
Navigate to the project directory:

bash
Copy code
cd ai-podcast-platform
Install dependencies:

bash
Copy code
npm install
Set up environment variables:

Create a .env.local file and add the following keys:

bash
Copy code
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
NEXT_PUBLIC_STRIPE_PUBLIC_KEY=your_stripe_public_key
NEXT_PUBLIC_CLERK_FRONTEND_API=your_clerk_api_key
CONVEX_DEPLOYMENT_URL=your_convex_deployment_url
Run the application:

bash
Copy code
npm run dev
Access the app at http://localhost:3000.

Usage
Create a new podcast by entering the podcast title and description.
Select your preferred AI voice from the list of available options.
Provide a text prompt for the AI to convert into a podcast.
Optionally generate a thumbnail image for your podcast.
Click "Submit & Publish Podcast" to complete the process.
Listen to your podcast directly within the platform.
Folder Structure
bash
Copy code
.
├── components      # Reusable UI components
├── pages           # Next.js page components
├── public          # Static files (images, etc.)
├── styles          # SCSS and CSS files
├── hooks           # Custom React hooks
├── utils           # Utility functions
├── convex          # Convex server logic
├── types           # TypeScript interfaces and types
└── README.md       # Project documentation
API Endpoints
/api/generateAudio: Generates podcast audio using the selected AI voice and text prompt.
/api/upload: Uploads generated audio and thumbnail images to Cloudinary.
Contributing
Contributions are welcome! To contribute:

Fork the repository.
Create a new feature branch: git checkout -b feature-name.
Make your changes.
Commit your changes: git commit -m 'Add some feature'.
Push to the branch: git push origin feature-name.
Submit a pull request.
License
This project is licensed under the MIT License - see the LICENSE file for details.
