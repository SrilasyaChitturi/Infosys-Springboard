# Infosys-Springboard
# Milestone 4 – Admin Dashboard, Analytics & User Management

## Description
In this milestone, the Streamlit NLP platform was enhanced with a powerful **Admin Management System, Activity Tracking, Analytics Dashboard, Feedback System, and User Profile Management**.

The system now provides administrators with complete control over users, system logs, and platform analytics. Additionally, users can manage their personal profiles and submit feedback to improve the platform. Data visualization tools and WordCloud generation were integrated to analyze usage patterns and user feedback effectively.

---

## Features Implemented

### Admin User Management
The platform now includes a dedicated **Admin Dashboard** that allows administrators to manage user accounts and control access to the system.

- Promote normal users to **Admin role**
- **Lock or unlock** user accounts
- **Delete users** from the system
- Maintain **secure role-based access control**
- View and manage all registered users

---

### System Activity & Logs
To monitor system usage and ensure transparency, the application now tracks user activity and system operations.

- Track **active users currently using the platform**
- Maintain **system activity logs**
- Monitor **which features each user uses**
- Display **activity insights in the Admin dashboard**
- Store logs securely in the database

---

### Analytics & Data Visualization
An analytics dashboard was added to provide insights into platform usage through interactive charts.

- Visual charts for **AI model usage**
- Charts for **language usage statistics**
- Charts for **most frequently used features**
- Interactive **Admin analytics dashboard**
- Built using **Plotly for real-time visualization**

---

### Feedback System & WordCloud
A feedback system was introduced to collect insights from users and visualize common suggestions.

- **User feedback submission form**
- Store feedback data in the database
- **Admin feedback management panel**
- Generate **WordCloud visualization** from user feedback
- Helps identify **common issues and suggestions**

---

### User Profile Dashboard
Users now have a dedicated profile section where they can manage their personal information.

- **Update email address**
- **Change password securely**
- **Upload or update profile avatar (Display Picture)**
- Improved **UI/UX for profile management**
- Personalized user settings dashboard

---

### Security Enhancements
To ensure platform security, the system maintains strict authentication and account protection mechanisms.

- Secure **OTP-based authentication**
- Password encryption using **bcrypt**
- **Account lock mechanism** for suspicious activity
- Role-based **Admin access control**

---

### Improved UI/UX
The application interface was improved to make dashboards and user interactions more intuitive.

- Enhanced **Admin dashboard layout**
- Interactive **analytics and charts**
- Organized **user profile section**
- Better **visual feedback and navigation**

---

## Technologies Used

- **Python**
- **Streamlit**
- **Flask**
- **JWT Authentication**
- **Plotly (for analytics charts)**
- **WordCloud**
- **SQLite / Database management**
- **Docker**
- **Ngrok**

---

## How to Run

1. Install dependencies 
2. Run the application  

3. Open the local URL displayed in the terminal.

4. Login as **Admin** to access the **Admin Dashboard**.
## Screenshots
<img width="1353" height="625" alt="Screenshot 2026-03-07 195902" src="https://github.com/user-attachments/assets/ae3b7445-fa77-4c8b-9021-bc604c2924ac" />
<img width="1350" height="570" alt="Screenshot 2026-03-12 234505" src="https://github.com/user-attachments/assets/7cbefd86-52dd-4a9c-a8db-90a48c7c4cf8" />
<img width="1345" height="562" alt="Screenshot 2026-03-12 234540" src="https://github.com/user-attachments/assets/528d04b4-c611-4570-a404-d587138df419" />
<img width="1338" height="626" alt="Screenshot 2026-03-12 233334" src="https://github.com/user-attachments/assets/2c3593b7-e39b-4909-9a41-3ed7309ca911" />
<img width="1339" height="624" alt="Screenshot 2026-03-12 233347" src="https://github.com/user-attachments/assets/e0ace25a-eeeb-49f3-a25b-d1142bbdeca0" />
<img width="1346" height="618" alt="Screenshot 2026-03-12 233802" src="https://github.com/user-attachments/assets/fae147fa-aa8b-41f1-8571-0a18f5621c3f" />
<img width="1341" height="616" alt="Screenshot 2026-03-12 233818" src="https://github.com/user-attachments/assets/e215da17-0f84-4bf9-a3f9-491153db9c34" />
<img width="1329" height="624" alt="Screenshot 2026-03-12 233908" src="https://github.com/user-attachments/assets/f2ffb31c-a097-453d-9c78-fe66a93cd080" />
<img width="1326" height="617" alt="Screenshot 2026-03-12 233921" src="https://github.com/user-attachments/assets/2e312428-fedd-416a-bec7-9549929303d1" />
<img width="1335" height="619" alt="Screenshot 2026-03-12 233957" src="https://github.com/user-attachments/assets/2270d0b9-5940-4387-b920-77a8394f4b5b" />
<img width="1340" height="619" alt="Screenshot 2026-03-12 234013" src="https://github.com/user-attachments/assets/7236b400-a3ba-4cc1-ac6e-a33046bd286b" />
<img width="1328" height="619" alt="Screenshot 2026-03-12 234026" src="https://github.com/user-attachments/assets/dd2514af-8624-4b00-87d6-3fb619ad43b9" />
<img width="1337" height="622" alt="Screenshot 2026-03-12 234049" src="https://github.com/user-attachments/assets/f7376e02-444a-4011-b123-44d73209cf1d" />
<img width="1332" height="615" alt="Screenshot 2026-03-12 234113" src="https://github.com/user-attachments/assets/389ab07b-dfd1-4175-81d0-f928c56ced03" />
<img width="1339" height="608" alt="Screenshot 2026-03-12 234130" src="https://github.com/user-attachments/assets/a54cea84-663f-416c-aa39-6c270198e0a1" />
<img width="1353" height="619" alt="Screenshot 2026-03-12 234206" src="https://github.com/user-attachments/assets/572d19e1-2731-40ac-ae7f-bc36cf25ce6f" />
<img width="1333" height="609" alt="Screenshot 2026-03-12 234216" src="https://github.com/user-attachments/assets/509c7d0a-a826-4636-8bb6-214e94925561" />
<img width="1337" height="622" alt="Screenshot 2026-03-12 234243" src="https://github.com/user-attachments/assets/3c465ee4-4736-4ed9-9d04-99787fd61e3b" />
<img width="1335" height="613" alt="Screenshot 2026-03-12 234326" src="https://github.com/user-attachments/assets/5875bd42-b0ba-43bb-8fd6-c745ebdbbd0f" />
<img width="1325" height="610" alt="Screenshot 2026-03-12 234337" src="https://github.com/user-attachments/assets/302c518f-ce46-4b89-b8e5-6a391bc9750a" />
<img width="1337" height="609" alt="Screenshot 2026-03-12 234348" src="https://github.com/user-attachments/assets/c1b6cadc-4ce0-4a1a-8ca4-451792726ab5" />
<img width="1335" height="612" alt="Screenshot 2026-03-12 234400" src="https://github.com/user-attachments/assets/91f33991-b238-4bd7-88a9-459812d78f8c" />
<img width="1321" height="610" alt="Screenshot 2026-03-12 234414" src="https://github.com/user-attachments/assets/e71287ec-3a82-4e7b-9595-3850efc012e7" />
<img width="1334" height="617" alt="Screenshot 2026-03-12 234429" src="https://github.com/user-attachments/assets/77254e2b-ad4f-442b-979d-113f17d9db30" />
<img width="1336" height="618" alt="Screenshot 2026-03-12 234440" src="https://github.com/user-attachments/assets/7551ede3-b624-43e6-a142-68aa93aa0c4d" />





