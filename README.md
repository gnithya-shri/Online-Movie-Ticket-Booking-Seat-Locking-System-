# 🎬 Online Movie Ticket Booking & Seat Locking System

A full-stack web application that simulates a real-world movie ticket booking platform. It features a **concurrent seat locking mechanism** to prevent double bookings and ensure a seamless user experience.

---

## 📌 Project Overview

This application allows users to browse movies, select show timings, and book seats through an interactive interface. 

The **core highlight** of this project is the seat locking system, which temporarily reserves selected seats to avoid conflicts when multiple users attempt to book the same seat simultaneously.

## 🚀 Features

- 🎥 **Browse Movies:** View current listings and show timings.
- 🪑 **Interactive UI:** Dynamic seat selection interface.
- 🔒 **Seat Locking:** Temporary reservation system to prevent race conditions.
- ✅ **Workflow:** Integrated booking confirmation process.
- 👤 **Auth:** User registration and login system.
- 🛠️ **Admin Panel:** Full CRUD for movies, shows, and seat management.
- 📊 **Analytics:** Dashboard featuring data visualization for booking insights.

## 🛠️ Tech Stack

- **Backend:** Python, Django Framework
- **Database:** SQL (Relational Database)
- **Frontend:** HTML5, CSS3, JavaScript
- **Charts:** Chart.js

---

## ⚙️ How It Works

1. **Selection:** User selects a movie and preferred showtime.
2. **Locking:** Once a seat is clicked, it is marked as `LOCKED` in the SQL database.
3. **Timer:** A timeout mechanism releases the seats if the booking isn't finished within a set time.
4. **Consistency:** Locked seats are invisible or unselectable for other concurrent users.
5. **Finalization:** Seats transition from `LOCKED` to `BOOKED` only after successful confirmation.

---
![App Preview](Screenshot%202026-03-15%20200515.png)

## 📂 Project Structure

```text
project/
│── booking/          # Seat selection & locking logic  
│── movies/           # Movie & show management  
│── users/            # Authentication system  
│── templates/        # HTML files  
│── static/           # CSS, JS, assets  
└── manage.py         # Django entry point
