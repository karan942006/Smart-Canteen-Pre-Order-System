# 🍽️ Smart Canteen Pre-Order System

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Georgia&size=30&duration=3000&pause=1000&color=2F6F4F&center=true&vCenter=true&width=900&lines=Smart+Canteen+Pre-Order+System;Android+App+Using+Java+%26+Firebase;Real-Time+Order+Tracking;Student+%26+Admin+Dashboard;Built+with+Android+Studio" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Android-green?style=for-the-badge&logo=android"/>
  <img src="https://img.shields.io/badge/Language-Java-orange?style=for-the-badge&logo=java"/>
  <img src="https://img.shields.io/badge/Firebase-Realtime%20Database-yellow?style=for-the-badge&logo=firebase"/>
  <img src="https://img.shields.io/badge/Auth-Firebase%20Authentication-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/UI-Material%20Design-success?style=for-the-badge"/>
</p>

---

## 🚀 Overview

**Smart Canteen Pre-Order System** is a complete Android application developed using **Java**, **Firebase Authentication**, and **Firebase Realtime Database**.

The system allows students to browse food items, add products to cart, make demo payments, receive digital bills, and track order progress in real time. Canteen staff can manage food items, update order status, and monitor revenue through an admin dashboard.

---

## ✨ Key Features

### 👨‍🎓 Student Module

✅ Email & Password Authentication

✅ Student Registration

✅ Browse Food Menu

✅ Search Food Items

✅ Category Filtering

✅ Cart Management

✅ Demo Payment Gateway

✅ Auto Generated Token Number

✅ Digital Receipt / Bill

✅ Order Tracking

✅ Real-Time Status Updates

✅ Order History

✅ Logout Functionality

---

### 👨‍🍳 Admin Module

✅ Secure Admin Login

✅ Dashboard Analytics

✅ Revenue Monitoring

✅ Order Management

✅ Food Inventory Management

✅ Enable / Disable Food Items

✅ Delete Menu Items

✅ Update Food Prices

✅ Real-Time Order Updates

✅ Student Statistics

---

## 📱 Application Flow

```text
Authentication
      │
      ▼
 Student Dashboard
      │
      ├── Menu
      │     ├── Search
      │     ├── Filter
      │     └── Add to Cart
      │
      ├── Cart Bottom Sheet
      │
      ├── Payment Screen
      │
      ├── Bill Generation
      │
      └── Order Tracking

Admin Login
      │
      ▼
 Admin Dashboard
      │
      ├── Manage Orders
      ├── Update Status
      ├── Manage Foods
      └── Revenue Analytics
```

---

## 🎨 Design System

| Element     | Color   |
| ----------- | ------- |
| Slate       | #1f2b27 |
| Green       | #2f6f4f |
| Light Green | #4f9d74 |
| Amber       | #f2a93b |
| Cream       | #fbf6ec |
| Paper       | #fffdf7 |
| Border      | #d8cfb8 |
| Error       | #d9534f |
| Text        | #2a2a2a |

### Typography

```text
Headings   → Georgia
Body       → Segoe UI
Receipt    → Courier New
```

---

## 🛠 Firebase Database Structure

```json
students
 └── uid
      ├── name
      ├── email
      └── mobile

foods
 └── foodId
      ├── name
      ├── category
      ├── price
      ├── availability
      └── emoji

orders
 └── orderId
      ├── studentId
      ├── studentName
      ├── date
      ├── totalAmount
      ├── status
      ├── tokenNumber
      ├── paymentMethod
      ├── paymentId
      └── items[]
```

---

## 🍔 Default Food Menu

| Item            | Category  | Price |
| --------------- | --------- | ----- |
| 🥪 Veg Sandwich | Snacks    | ₹40   |
| 🥞 Masala Dosa  | Breakfast | ₹50   |
| 🍛 Veg Biryani  | Lunch     | ₹90   |
| 🌮 Paneer Roll  | Snacks    | ₹60   |
| 🥤 Cold Coffee  | Beverages | ₹35   |
| 🥟 Samosa (2pc) | Snacks    | ₹20   |
| 🍱 Veg Thali    | Lunch     | ₹100  |
| ☕ Masala Chai   | Beverages | ₹15   |

---

## 🔐 Demo Admin Login

```text
Email    : admin@canteen.edu
Password : admin123
```

---

## 📦 Order Status Workflow

```text
Pending
   │
   ▼
Accepted
   │
   ▼
Preparing
   │
   ▼
Ready
   │
   ▼
Delivered
```

Real-time synchronization ensures that student order status updates instantly whenever the admin changes the order stage.

---

## 📂 Project Structure

```text
📦 SmartCanteen
│
├── activities
│   ├── AuthActivity
│   ├── StudentMainActivity
│   └── AdminMainActivity
│
├── fragments
│   ├── MenuFragment
│   ├── MyOrdersFragment
│   ├── DashboardFragment
│   ├── ManageOrdersFragment
│   └── ManageFoodsFragment
│
├── bottomsheets
│   ├── CartBottomSheet
│   └── PaymentBottomSheet
│
├── dialogs
│   └── BillDialog
│
├── models
│   ├── Student
│   ├── Food
│   ├── Order
│   ├── OrderItem
│   └── CartItem
│
├── adapters
│   ├── FoodAdapter
│   ├── CartAdapter
│   ├── OrderAdapter
│   ├── AdminOrderAdapter
│   └── AdminFoodAdapter
│
├── firebase
│   └── FirebaseHelper
│
└── res
    ├── layouts
    ├── drawable
    ├── values
    └── anim
```

---

## ⚡ Dependencies

```gradle
implementation platform('com.google.firebase:firebase-bom:latest')

implementation 'com.google.firebase:firebase-auth'
implementation 'com.google.firebase:firebase-database'

implementation 'com.google.android.material:material:latest'
implementation 'androidx.recyclerview:recyclerview:latest'
implementation 'androidx.cardview:cardview:latest'
implementation 'androidx.constraintlayout:constraintlayout:latest'
```

---

## 🎬 UI Animations

✨ Fade-Up Card Animation

✨ Pulsing Logo Badge

✨ Cart Badge Counter

✨ Animated Progress Tracker

✨ Bottom Sheet Slide-Up

✨ Bill Success Pop Animation

✨ Real-Time Dashboard Refresh

---

## 📸 Screens Included

### Student Side

* Login & Registration
* Menu Screen
* Search & Filter
* Cart Bottom Sheet
* Payment Bottom Sheet
* Digital Receipt
* My Orders Tracking

### Admin Side

* Dashboard Analytics
* Manage Orders
* Update Order Status
* Manage Food Menu

---

## 🔥 Why This Project?

This project demonstrates:

* Android Development using Java
* Firebase Authentication
* Firebase Realtime Database
* Material Design UI
* RecyclerView & Adapters
* Bottom Sheets
* Real-Time Data Synchronization
* CRUD Operations
* Clean Architecture
* College-Level Industry Project

---

## ⭐ Future Enhancements

* Razorpay Integration
* QR Code Token System
* Push Notifications
* AI Food Recommendations
* Inventory Prediction
* Firebase Cloud Messaging
* Admin Reports Export (PDF)

---

## 👨‍💻 Developer

**Karan Lingayat**

Android Developer • Firebase Developer • Cybersecurity Enthusiast

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Georgia&size=22&duration=2500&pause=1000&color=F2A93B&center=true&vCenter=true&width=700&lines=Thank+You+For+Visiting!;Star+⭐+the+Repository;Happy+Coding+🚀" />
</p>
