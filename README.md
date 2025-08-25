## imagify Screenshots

![Home Page](./client/public/home.png)

🖼️ AI Text-to-Image Generator (MERN + SaaS)

A Full Stack AI SaaS Application built with MongoDB, Express, React, and Node.js (MERN) that allows users to generate AI-powered images from text prompts.
The app includes user authentication, credit system, payment integration, and image generation using ClipDrop API.

🚀 Features

🔐 User Authentication – Sign up, log in, and manage user accounts (stored in MongoDB).

🖼️ AI Text-to-Image Generation – Generate high-quality images using ClipDrop API.

🎟️ Credit System – Each image generation consumes credits.

💳 Payment Gateway Integration – Users can purchase credits online securely.

📦 MERN Stack – Built with MongoDB, Express.js, React.js, and Node.js.

⚡ REST API Backend – Handles authentication, payments, and image requests.

🖥️ Responsive UI – Clean and modern frontend built with React.

🛠️ Tech Stack

Frontend: React.js, TailwindCSS

Backend: Node.js, Express.js

Database: MongoDB (Mongoose ODM)

Authentication: JWT (JSON Web Tokens)

Payments: Stripe (or your integrated gateway)

AI API: ClipDrop API

Deployment: Vercel (frontend) + Render/Heroku (backend)

📂 Project Structure
├── client/           # React frontend
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── context/
│   │   └── utils/
│   └── package.json
│

├── server/           # Node.js backend
│   ├── config/       # DB & environment configs
│   ├── controllers/  # Auth, Payment, Image generation
│   ├── models/       # MongoDB models (User, Transactions)
│   ├── routes/       # Express routes
│   ├── server.js     # Entry point
│   └── package.json
│

├── .gitignore
├── README.md
└── package.json

⚙️ Installation & Setup

1️⃣ Clone Repository
git clone https://github.com/your-username/ai-text-to-image-saas.git
cd ai-text-to-image-saas

2️⃣ Install Dependencies
# Install backend dependencies
cd server
npm install

# Install frontend dependencies
cd ../client
npm install

3️⃣ Setup Environment Variables
Create .env file in the server/ folder:

MONGO_URI=your_mongodb_connection_string

JWT_SECRET=your_jwt_secret

CLIPDROP_API_KEY=your_clipdrop_api_key

STRIPE_SECRET_KEY=your_stripe_secret_key

STRIPE_PUBLIC_KEY=your_stripe_public_key

4️⃣ Run the App
# Run backend
cd server
npm run dev

# Run frontend (new terminal)
cd client
npm start

🧪 API Endpoints
Authentication

POST /api/auth/register → Register new user

POST /api/auth/login → Login user

Credits & Payments

POST /api/payment/create-checkout-session → Purchase credits

GET /api/user/credits → Fetch user credits

AI Image Generation

POST /api/image/generate → Generate image using text prompt

📌 Deployment

Frontend (React): Vercel / Netlify

Backend (Express): Render / Railway / Heroku

Database: MongoDB Atlas

🤝 Contributing

Contributions are welcome!

Fork the repo

Create a feature branch

Commit changes

Open a Pull Request 🚀

📜 License

This project is licensed under the MIT License.

💡 Future Improvements

Add social login (Google, GitHub)

Support image history & downloads

Implement subscription-based billing

Enhance prompt-to-image quality with more AI APIs
