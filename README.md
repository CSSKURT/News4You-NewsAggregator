# 📚 News Aggregator for The Future Business Teachers' Organization
## Powered by Mapúa & FBTO

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

### User Authentication
- **User Registration:**
  - **Endpoint:** `POST /api.php?action=register`
  - **Description:** Registers a new user with the following JSON body:
    ```json
    {
      "firstname": "John",
      "lastname": "Doe",
      "email": "john.doe@example.com",
      "gender": "male",
      "birthday": "1990-01-01",
      "password": "yourpassword"
    }
    ```
  - **Functionality:** Creates a new user account and stores user information in the database.

- **User Login:**
  - **Endpoint:** `POST /api.php?action=login`
  - **Description:** Authenticates a user with the following JSON body:
    ```json
    {
      "email": "john.doe@example.com",
      "password": "yourpassword"
    }
    ```
  - **Functionality:** Validates user credentials and returns a session token for authenticated requests.

### User Preferences
- **Set User Preferences:**
  - **Endpoint:** `POST /api.php?action=setPreferences`
  - **Description:** Allows users to specify their news preferences (e.g., topics of interest such as local, international, sports, and entertainment).
  - **Functionality:** Saves user preferences in the database, which will be used to filter news articles.

- **Get User Preferences:**
  - **Endpoint:** `GET /api.php?action=getPreferences`
  - **Description:** Retrieves the current preferences set by the user.
  - **Functionality:** Returns the user's preferences to customize the news feed.

### Personalized News Retrieval
- **Get Personalized News:**
  - **Endpoint:** `GET /api.php?action=getPersonalizedNews`
  - **Description:** Fetches news articles based on the user's preferences.
  - **Functionality:** Queries the News API using the user's specified topics and filters the results to return articles that match their interests. This ensures that users receive content that is relevant to them.

### Article Management
- **Bookmark Articles:**
  - **Endpoint:** `POST /api.php?action=bookmarkArticle`
  - **Description:** Allows users to bookmark articles for later reading.
  - **Functionality:** Saves the article ID to the user's bookmarks in the database.

- **Get Bookmarked Articles:**
  - **Endpoint:** `GET /api.php?action=getBookmarkedArticles`
  - **Description:** Retrieves a list of articles that the user has bookmarked.
  - **Functionality:** Returns the bookmarked articles for easy access.

### Search Functionality
- **Search Articles:**
  - **Endpoint:** `GET /api.php?action=searchArticles`
  - **Description:** Allows users to search for articles based on keywords.
  - **Functionality:** Filters articles from the database or the News API based on the search query, providing users with relevant results.

### User Profile Management
- **Get User Profile:**
  - **Endpoint:** `GET /api.php?action=getUserProfile`
  - **Description:** Retrieves the user's profile information.
  - **Functionality:** Returns user details, including preferences and bookmarked articles.

- **Update User Profile:**
  - **Endpoint:** `PUT /api.php?action=updateUserProfile`
  - **Description:** Allows users to update their profile information.
  - **Functionality:** Updates user details in the database, ensuring that their profile remains current.

### Commenting System
- **Add Comment:**
  - **Endpoint:** `POST /api.php?action=addComment`
  - **Description:** Allows users to add comments to articles.
  - **Functionality:** Saves the comment associated with the article ID in the database.

- **Get Comments:**
  - **Endpoint:** `GET /api.php?action=getComments&id={articleId}`
  - **Description:** Retrieves comments for a specific article.
  - **Functionality:** Returns all comments associated with the specified article ID.

### Notifications
- **Get Notifications:**
  - **Endpoint:** `GET /api.php?action=getNotifications`
  - **Description:** Retrieves notifications for the user, such as new articles or comments on their posts.
  - **Functionality:** Returns a list of notifications to keep users informed about relevant updates.


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
