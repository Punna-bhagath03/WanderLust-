# TripTales - Airbnb Replica

TripTales is a full-stack web application designed to mimic the core functionality of Airbnb. It allows users to sign up, log in, create and manage listings, and leave reviews. Built with Node.js, Express.js, and MongoDB, this project showcases user authentication, session management, image uploads, and access control.

---

## 📋 Features

### User Authentication
- **Sign Up**: New users can create an account by providing their details.
- **Login**: Existing users can log into their accounts securely.
- **Logout**: Users can log out of their accounts with a single click.

### Listing Management
- **Create Listings**: Logged-in users can create Airbnb-like property listings by providing accommodation details and uploading images.
- **Edit Listings**: Owners can edit their listings, including the ability to replace the listing image (preview of current image provided).
- **Delete Listings**: Owners can delete their listings from the platform.
- **Access Control**: Only the owner of a listing can edit or delete it. Other users cannot alter the listing.

### Reviews and Ratings
- **Write Reviews**: Any user can leave a review and rate a listing with a star rating.
- **View Reviews**: Everyone can see reviews and ratings associated with a particular listing.

---

## 🛠️ Tech Stack
- **Backend**: Node.js, Express.js
- **Database**: MongoDB (Mongoose for Object Data Modeling)
- **Image Upload**: Cloudinary (via Multer for handling file uploads)
- **Authentication**: Passport.js with Passport-Local for handling user authentication
- **Session Management**: Express-session with MongoDB session store
- **Validation**: Joi (for input validation)
- **Environment Variables**: dotenv (for managing environment variables)
- **Frontend**: EJS (Embedded JavaScript templates)

---

## 📂 Project Directory Structure
.
├── public/                 # Static assets such as CSS, images, and JavaScript files
├── views/                  # EJS template files for the frontend
├── models/                 # MongoDB models (User, Listing, Review)
├── routes/                 # Route handlers for API and page rendering
├── middlewares/            # Custom middleware (authentication, validation, etc.)
├── uploads/                # Temporary storage for uploaded files (images)
├── app.js                  # Main server file for the backend
├── .env                    # Environment configuration
├── package.json            # Project dependencies and metadata
└── README.md               # Project documentation (this file)

---

## 📦 Installation and Setup

### Prerequisites

Ensure the following are installed on your local machine:
- **Node.js** (LTS version recommended)
- **MongoDB** (local or cloud instance)
- **Git** (for cloning the repository)

### Step-by-Step Installation

```bash
1. Clone the repository:
   git clone https://github.com/your-username/TripTales.git
   cd TripTales

2. Install Backend Dependencies:
   From the root directory, run:
   npm install

3. Set Up Environment Variables:
   Create a `.env` file in the root of the project and configure the following variables:
   CLOUDINARY_CLOUD_NAME=your-cloudinary-cloud-name
   CLOUDINARY_API_KEY=your-cloudinary-api-key
   CLOUDINARY_API_SECRET=your-cloudinary-api-secret
   MONGO_URI=your-mongodb-uri
   SESSION_SECRET=your-session-secret

4. Start the Application:
   Run the application with Node.js:
   node app.js

🚀 Deployment

TripTales is live on Render for easy access and testing. You can view the deployed version here:

TripTales Deployed on Render-https://triptaless-1.onrender.com/listings
<hr>
🖥️ How to Use
	1.	Access the Application:
	•	Run the project locally by visiting http://localhost:3000 after following the installation steps.
	•	Alternatively, use the deployed version on Render.
	2.	Sign Up / Log In:
	•	New users can sign up and create an account.
	•	Registered users can log in and manage their profiles and listings.
	3.	Create a Listing:
	•	After logging in, users can create listings by adding details such as property type, location, and uploading images.
	4.	Manage Listings:
	•	Owners can edit and delete their own listings. Only the creator of the listing can perform these actions.
	5.	Leave Reviews:
	•	Users can leave star ratings and reviews for any listing to help others make informed decisions.
	6.	Image Management:
	•	While editing a listing, the current image is displayed as a low-resolution preview. Users can replace the image with a new one.
<hr>
🔄 Contributing

We welcome contributions! If you would like to improve the project, feel free to fork the repository, submit issues, or create pull requests. Please follow the code of conduct and guidelines for contributing.
