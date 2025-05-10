# Samrat Singh Rajput Portfolio Website

## Overview
This repository contains the source code for the personal portfolio website of **Samrat Singh Rajput**, a social media influencer and YouTuber from Lucknow, India. The website showcases his work as a content creator through *Samrat Rajput Creation* and his entrepreneurial venture, *Samrat Royal Collection*. It features sections for his biography, journey, ventures, galleries, videos, testimonials, and contact information, designed to engage fans and potential collaborators.

The website is built as a single-page application with a modern, responsive design, incorporating interactive elements like a rating system, review form, contact form, and an AI-powered chatbot, all integrated with Firebase for real-time data storage.

## Features
- **Responsive Design**: Optimized for desktops, tablets, and mobile devices with Tailwind CSS-inspired utility classes.
- **Interactive Elements**:
  - **Star Rating System**: Allows users to rate Samrat’s content, with real-time average rating updates.
  - **Review System**: Users can submit reviews, stored in Firebase and displayed in a modal.
  - **Contact Form**: Enables users to send messages, saved to Firebase for collaboration inquiries.
  - **AI Chatbot**: Provides contextual responses about Samrat’s work, guiding users to relevant sections.
- **Gallery Sections**:
  - **Vertical Gallery**: Displays images with a height of 16rem (responsive to 12rem on mobile).
  - **Horizontal Gallery**: Showcases images with consistent sizing and error handling for failed loads.
- **Social Media Integration**: Links to Samrat’s YouTube, Instagram, and Facebook profiles with animated icons.
- **Video Showcase**: Embeds featured YouTube videos in a responsive grid.
- **Smooth Scrolling Navigation**: Enhances user experience with seamless transitions between sections.
- **SEO Optimization**: Includes meta tags and structured data (JSON-LD) for better search engine visibility.
- **Firebase Integration**: Stores ratings, reviews, contact messages, and chatbot interactions in real-time.

## Technologies Used
- **HTML5**: Structure of the single-page application.
- **CSS3**: Custom styles with utility classes inspired by Tailwind CSS, including animations and responsive design.
- **JavaScript (ES6)**: Handles interactivity, DOM manipulation, and Firebase integration.
- **Firebase**:
  - Realtime Database for storing ratings, reviews, contact messages, and chatbot interactions.
  - Firebase SDK (v9.22.0) for client-side integration.
- **External Libraries**:
  - Firebase JavaScript SDK for database operations.
- **Assets**:
  - Images hosted in the `images/` directory.
  - Placeholder images from `via.placeholder.com` for error handling.

## Prerequisites
To run this project locally, ensure you have:
- A modern web browser (e.g., Chrome, Firefox, Edge).
- A Firebase project set up with the Realtime Database enabled.
- Node.js (optional, for local development with a server).
- A text editor (e.g., VS Code) for code modifications.

## Setup Instructions
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/akrappdeveloper/SamratSinghRajput.git
   cd SamratSinghRajput
   ```

2. **Set Up Firebase**:
   - Create a Firebase project at [console.firebase.google.com](https://console.firebase.google.com).
   - Enable the Realtime Database and set up rules for read/write access (e.g., allow authenticated or public access for testing).
   - Copy your Firebase configuration object (e.g., `apiKey`, `databaseURL`, etc.) from the Firebase console.
   - Update the `firebaseConfig` object in the `<script>` section of `index.html` with your Firebase credentials:
     ```javascript
     const firebaseConfig = {
         apiKey: "YOUR_API_KEY",
         authDomain: "YOUR_AUTH_DOMAIN",
         databaseURL: "YOUR_DATABASE_URL",
         projectId: "YOUR_PROJECT_ID",
         storageBucket: "YOUR_STORAGE_BUCKET",
         messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
         appId: "YOUR_APP_ID",
         measurementId: "YOUR_MEASUREMENT_ID"
     };
     ```

3. **Serve the Website**:
   - Option 1: Open `index.html` directly in a browser (note: Firebase features may require a server due to CORS).
   - Option 2: Use a local server for full functionality:
     ```bash
     npm install -g http-server
     http-server .
     ```
     Access the site at `http://localhost:8080`.

4. **Verify Firebase Integration**:
   - Ensure the Firebase Realtime Database is receiving data (e.g., ratings, reviews, contact messages) by submitting test inputs via the website.
   - Check the Firebase console for stored data under the `ratings`, `reviews`, `contacts`, and `chatbotInteractions` nodes.

## Usage
- **Navigation**: Use the top navigation bar to jump to sections (`Home`, `About`, `Journey`, `Ventures`, `Gallery`, `Contact`).
- **Rating and Reviews**:
  - Click the star rating system to rate Samrat’s content (1–5 stars).
  - Submit a review via the form below the rating section.
  - View all reviews by clicking “Show All Reviews” in the modal.
- **Contact Form**: Open the contact modal from the “Contact” section, fill in your details, and submit a message.
- **Chatbot**: Click the chatbot button (bottom-right corner) to ask questions about Samrat’s work. The AI responds with links to relevant sections.
- **Galleries**: Browse the vertical and horizontal galleries to view images. Fallback placeholders display if images fail to load.
- **Social Media**: Click the YouTube, Instagram, or Facebook icons to visit Samrat’s profiles.
- **Videos**: Watch embedded YouTube videos in the “Featured Videos” section.

## Project Structure
```plaintext
SamratSinghRajput/
├── images/                  # Image assets for profile, galleries, and logo
│   ├── profile.jpg
│   ├── IMG-20250510-WA0002.jpg
│   └── ...
├── index.html              # Main HTML file with embedded CSS and JavaScript
└── README.md               # This file
```

## Contributing
Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Make changes and commit (`git commit -m "Add your feature"`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request with a detailed description of your changes.

Please ensure your code follows:
- Consistent formatting (use Prettier or similar).
- Clear commit messages.
- Compatibility with existing Firebase integration and responsive design.

## Issues
If you encounter bugs or have feature requests:
- Open an issue in the GitHub repository.
- Provide details like browser version, steps to reproduce, and screenshots if applicable.

## Deployment
The website is deployed via GitHub Pages at:  
[https://akrappdeveloper.github.io/SamratSinghRajput/](https://akrappdeveloper.github.io/SamratSinghRajput/)

To deploy updates:
1. Push changes to the `main` branch.
2. Ensure GitHub Pages is configured to serve from the `main` branch root.
3. Verify the updated site at the above URL.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact
For inquiries or collaboration opportunities:
- **Website Owner**: Samrat Singh Rajput
  - Email: Use the contact form on the website.
  - Social Media: [YouTube](https://youtube.com/@samratrajputcreation), [Instagram](https://www.instagram.com/samrat_kushwaha_rajput), [Facebook](https://www.facebook.com/samrat.kushwaha.7798)
- **Developer**: AKR Industry
  - Email: [contact@akrindustry.com](mailto:contact@akrindustry.com)
  - GitHub: [akrappdeveloper](https://github.com/akrappdeveloper)

---

*Made with ❤️ by AKR Industry for Samrat Singh Rajput*
