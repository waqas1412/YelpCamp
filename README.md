# 🏕️ YelpCamp

[![Node.js](https://img.shields.io/badge/Node.js-18.x-green.svg)](https://nodejs.org/)
[![Express](https://img.shields.io/badge/Express-4.18.1-blue.svg)](https://expressjs.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-6.6.2-green.svg)](https://www.mongodb.com/)
[![EJS](https://img.shields.io/badge/EJS-3.1.8-orange.svg)](https://ejs.co/)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-5.2.1-purple.svg)](https://getbootstrap.com/)
[![License](https://img.shields.io/badge/License-ISC-blue.svg)](LICENSE)

> A full-stack web application for discovering and reviewing campgrounds, built with Node.js, Express, and MongoDB.

## 📋 Table of Contents

- [✨ Features](#-features)
- [🛠️ Tech Stack](#️-tech-stack)
- [🚀 Getting Started](#-getting-started)
- [📁 Project Structure](#-project-structure)
- [🔧 API Endpoints](#-api-endpoints)
- [🎨 Screenshots](#-screenshots)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

## ✨ Features

- **🏕️ Campground Management**: Create, read, update, and delete campground listings
- **⭐ Review System**: Add and manage reviews with ratings (1-5 stars)
- **🔍 Data Validation**: Server-side validation using Joi schemas
- **💾 Database Integration**: MongoDB with Mongoose ODM
- **🎨 Modern UI**: Responsive design with Bootstrap 5
- **⚡ Error Handling**: Custom error handling with ExpressError class
- **🔄 Flash Messages**: User feedback with connect-flash
- **📱 Responsive Design**: Mobile-friendly interface
- **🔒 Form Validation**: Client-side form validation with Bootstrap

## 🛠️ Tech Stack

### Backend
- **Node.js** - JavaScript runtime environment
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB object modeling tool
- **Joi** - Data validation library
- **EJS** - Templating engine
- **Express Session** - Session middleware
- **Connect Flash** - Flash message middleware

### Frontend
- **Bootstrap 5** - CSS framework for responsive design
- **EJS Templates** - Server-side templating
- **Custom JavaScript** - Form validation and interactivity

### Development Tools
- **Method Override** - HTTP method override middleware
- **EJS Mate** - Layout support for EJS

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- MongoDB (running locally or cloud instance)
- npm or yarn package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/yelpcamp.git
   cd yelpcamp
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up MongoDB**
   - Ensure MongoDB is running on `mongodb://127.0.0.1:27017/yelp-camp`
   - Or update the connection string in `app.js`

4. **Seed the database (optional)**
   ```bash
   node seeds/index.js
   ```

5. **Start the application**
   ```bash
   node app.js
   ```

6. **Open your browser**
   Navigate to `http://localhost:3000`

## 📁 Project Structure

```
YelpCamp/
├── app.js                 # Main application entry point
├── package.json           # Project dependencies and scripts
├── models/                # Database models
│   ├── campground.js      # Campground model with reviews
│   └── review.js          # Review model
├── routes/                # Express routes
│   ├── campground.js      # Campground CRUD operations
│   └── reviews.js         # Review operations
├── views/                 # EJS templates
│   ├── layouts/           # Layout templates
│   ├── partials/          # Reusable components
│   └── campgrounds/       # Campground-specific views
├── public/                # Static assets
│   └── javascripts/       # Client-side JavaScript
├── utils/                 # Utility functions
│   ├── catchAsync.js      # Async error handler
│   └── ExpressError.js    # Custom error class
├── seeds/                 # Database seeding
│   ├── index.js           # Main seed script
│   ├── cities.js          # City data
│   └── seedHelpers.js     # Seed helper functions
└── schemas.js             # Joi validation schemas
```

## 🔧 API Endpoints

### Campgrounds
- `GET /campgrounds` - Display all campgrounds
- `GET /campgrounds/new` - Show create campground form
- `POST /campgrounds` - Create new campground
- `GET /campgrounds/:id` - Show specific campground
- `GET /campgrounds/:id/edit` - Show edit campground form
- `PUT /campgrounds/:id` - Update campground
- `DELETE /campgrounds/:id` - Delete campground

### Reviews
- `POST /campgrounds/:id/reviews` - Add review to campground
- `DELETE /campgrounds/:id/reviews/:reviewId` - Delete review

## 🎨 Screenshots

> *Screenshots will be added here once the application is running*

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the ISC License - see the [LICENSE](LICENSE) file for details.

---

<div align="center">

**Made with ❤️ using Node.js, Express, and MongoDB**

[![GitHub stars](https://img.shields.io/github/stars/yourusername/yelpcamp?style=social)](https://github.com/yourusername/yelpcamp/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/yourusername/yelpcamp?style=social)](https://github.com/yourusername/yelpcamp/network)
[![GitHub issues](https://img.shields.io/github/issues/yourusername/yelpcamp)](https://github.com/yourusername/yelpcamp/issues)

</div>
