🎬 Online Movie Ticket Booking & Seat Locking System

A full-stack web application that simulates a real-world movie ticket booking platform with a concurrent seat locking mechanism to prevent double bookings and ensure a smooth user experience.

📌 Project Overview

This application is built using the Django framework and allows users to browse movies, select show timings, and book seats through an interactive interface.

The core highlight of this project is the seat locking system, which temporarily reserves selected seats to avoid conflicts when multiple users attempt to book the same seat simultaneously.

🚀 Features
🎥 Browse movies and show timings
🪑 Interactive seat selection interface
🔄 Real-time seat availability handling
🔒 Temporary seat locking system
✅ Booking confirmation workflow
👤 User authentication (login/register)
🛠️ Admin panel to manage movies and shows
📊 Dashboard with basic analytics (charts & insights)
🛠️ Tech Stack
Python
Django Framework
MySQL Database
HTML
CSS
JavaScript
Chart.js
⚙️ How It Works
User registers and logs into the system
Movies and show timings are fetched from the database
User selects a movie and preferred show
Available seats are displayed dynamically
Selected seats are temporarily locked
User proceeds with booking confirmation
Seats are marked as booked after confirmation
If not completed, locked seats are automatically released
🔒 Seat Locking Mechanism
Seats are marked as LOCKED when selected by a user
Locked seats cannot be accessed by other users
A timeout mechanism releases seats if booking is not completed
Prevents race conditions and ensures data consistency
📂 Project Structure
project/
│── booking/              # Seat selection & locking logic  
│── movies/               # Movie & show management  
│── users/                # Authentication system  
│── templates/            # HTML files  
│── static/               # CSS, JS, assets  
│── mysql  
│── manage.py  
💡 Key Learning Outcomes
Implemented real-world concurrency handling (seat locking)
Built a complete full-stack Django application
Designed an interactive and user-friendly UI
Understood database consistency and conflict management
Developed admin dashboards with data visualization
⚠️ Limitations
SQLite is not ideal for high concurrency environments
Seat locking depends on server-side timing
No payment gateway integration (simulation only)
📸 Application Preview
<p align="center"> <img src="your-screenshot.png" width="700"> </p>
▶️ Run Locally
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
🌟 Future Improvements
💳 Payment gateway integration (Razorpay / Stripe)
🔔 Email & SMS notifications
⚡ Redis-based seat locking for scalability
📱 Improved mobile responsiveness
🌍 Multi-theatre support
💼 Final Note

This project goes beyond basic CRUD operations by addressing a critical real-world issue — handling simultaneous seat booking requests efficiently.
