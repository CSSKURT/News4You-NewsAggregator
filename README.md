# 📚 News Aggregator for The Future Business Teachers' Organization
## Powered by Mapúan Students & FBTO
Medina, Art Gabriel Luces - Documentation
Pasion, John Carlo - Documentation
Samonte, Adriel Denzel A. - 
Tambagan, Enrick Alfonso D. - Frontend & UI/UX Designer
Taningco, Kurt Andrei C. - Documentation

Client: Nicko Barro (President of Future Business Teachers Organization)

## 🛠️ Introduction
The overwhelming volume of news content across various topics makes it challenging for users to track information relevant to their interests. The **Personalized News Aggregator** aims to help users filter and find news that aligns with their specific preferences, fostering awareness and engagement through a user-curated experience in partnership with the Future Business Teachers' Organization (FBTO).

## 🎯 Objectives
- Develop a user information and database for user login and registration.
- Implement a user preference/filter system to allow users to select their news content preferences.
- Integrate the News API to retrieve articles and apply filtering based on user preferences, utilizing metadata for improved accuracy.
- Ensure the system is updated with real-time news content, displaying timestamps for article updates.
- Implement a filtering system and search bar for enhanced user experience.
- Support multi-platform accessibility using JavaScript, HTML, and PHP.
- Include a bookmarking feature for users to save articles for later reading.
- Create a user-friendly interface for easy navigation and interaction.

## 🌈 Dashboard Personalization Features
Users can put a personalized touch on their dashboard with the following decorative options:
- **Change Dashboard Color:** Users can select their preferred color scheme for the dashboard, allowing for a more personalized and visually appealing experience.
- **Custom Background Images:** Users can upload or select from a gallery of background images to enhance the aesthetic of their dashboard.
- **Font Style Selection:** Users can choose from a variety of font styles for headings and body text to match their personal taste.
- **Widget Arrangement:** Users can rearrange dashboard widgets (e.g., news categories, bookmarks, and notifications) to prioritize the information they find most important.
- **Theme Selection:** Users can choose from predefined themes (e.g., light mode, dark mode, or colorful themes) to suit their mood or preference.
- **Personalized Greetings:** Users can set a custom greeting message that appears on their dashboard, adding a personal touch to their experience.

## 🌍 UN SDGs Addressed
This project addresses 15 of the 17 United Nations Sustainable Development Goals (SDGs) by promoting awareness on various topics, including:
1. No Poverty
2. Zero Hunger
3. Good Health and Well-being
4. Quality Education
5. Gender Equality
6. Clean Water and Sanitation
7. Affordable and Clean Energy
8. Decent Work and Economic Growth
9. Industry, Innovation, and Infrastructure
10. Reduced Inequalities
11. Sustainable Cities and Communities
12. Responsible Consumption and Production
13. Climate Action
14. Peace, Justice, and Strong Institutions
15. Partnerships for the Goals

## 🛠️ Core Functionality
- Uses NewsAPI to fetch news articles.
- Allows users to search for specific topics.
- Supports article sorting (newest first or alphabetically).
- User authentication system with login/registration.
- Ability to save favorite articles.
- User profiles and dashboard.

## ⚙️ Technical Components
- PHP-based backend.
- Bootstrap for frontend styling.
- MySQL database for user management.
- Session-based authentication.
- Responsive design.

## 🛠️ REST API
The project includes a REST API that allows for programmatic access to various functionalities, enabling a personalized news experience for users. The API facilitates user interactions with the news aggregator by allowing them to set preferences, retrieve tailored content, and manage their accounts. Key endpoints include:


### 1. User Authentication and Management
- **User Registration and Login:**
  - **File:** `api.php`
  - **Functionality:** This file handles user registration and login requests. It allows users to create accounts and authenticate themselves using their email and password. Upon successful login, a session is initiated, enabling users to access personalized features.

### 2. Article Management
- **Save Article:**
  - **File:** `save_article.php`
  - **Functionality:** This script allows logged-in users to save articles they find interesting. When a user submits an article to be saved, the script retrieves the user's ID from the session and inserts the article details (title, URL, published date, and description) into the `saved_articles` table in the database. After saving, the user is redirected back to their profile page with a success message.

- **Unsave Article:**
  - **File:** `unsave_article.php`
  - **Functionality:** This script enables users to remove articles from their saved list. It checks if the user is logged in and retrieves their ID. If an article ID is provided, the script deletes the corresponding entry from the `saved_articles` table, allowing users to manage their saved content effectively. A success or error message is displayed based on the outcome.

### 3. News Retrieval
- **Fetch News Articles:**
  - **File:** `news_app.php`
  - **Functionality:** This file is responsible for fetching news articles from the News API based on user-defined topics. Users can input a topic and choose a sorting preference (newest first or alphabetically). The script constructs a request to the News API, retrieves the articles, and displays them on the page. Users can also save articles directly from this interface.


## 🎯 Suggested Adaptation for The Future Business Teachers' Organization

### 📅 Content Focus Redesign
Replace general news with education and nonprofit-focused content sections:
- Educational Events Calendar
- Donation Drive Updates
- Teaching Resources
- Business Education News
- Success Stories
- Volunteer Opportunities

### ✨ New Features to Add
- User Profile Management
- Article Management (CRUD operations)
- Commenting System
- Enhanced Search Functionality
- Event Management
- Notifications

## 📊 Analytics Dashboard
- Donation tracking metrics.
- Event attendance statistics.
- Resource usage analytics.
- Member engagement metrics.
- Impact assessment tools.

## 📝 Implementation Objectives
- **User Information and Database:** Develop the user information and database for users to log in or register their accounts to use the website.
- **User Preference/Filter System:** Implement a user preference/filter system that allows users to select their preferences in terms of news content.
- **News API Integration:** Integrate the News API to retrieve news articles and apply the filtering system based on the chosen preferences of the user. Use metadata for better filtering.
- **Timestamp Updates:** Ensure that the system is updated in terms of news content through the display of timestamps for article updates.
- **Filtering System and Search Bar:** Implement a filtering system and search bar for enhanced user experience.
- **Multi-Platform Accessibility:** Ensure the website supports multi-platform accessibility using JavaScript, HTML, and PHP.
- **Bookmarking Feature:** Implement a bookmarking feature to save articles that users would like to read again.
- **User-Friendly Interface:** Create a user-friendly interface that makes it easy for users to navigate and use the website.

## 🚀 Navigation Guide for Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   ```

2. **Set Up the Environment:**
   - Ensure you have PHP, MySQL, and a web server (like Apache) installed.
   - Use XAMPP or MAMP for a local development environment.

3. **Create the Database:**
   - Import the SQL file to create the necessary tables in your MySQL database.

4. **Configure Database Connection:**
   - Update the `connect.php` file with your database credentials.

5. **Run the Application:**
   - Start your web server and navigate to `http://localhost/your-repo-name/auth/login.php` to access the login page.

6. **Explore Features:**
   - Log in and explore the various features of the application.

## 📞 Support
For any issues or questions, please open an issue in this repository or contact the project maintainer.

---

Thank you for checking out the News Aggregator for The Future Business Teachers' Organization! 🌟
