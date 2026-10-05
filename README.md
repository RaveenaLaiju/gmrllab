# GMRL Laboratory Management System

## Overview

GMRL Laboratory Management System is a Django-based web application designed to manage laboratory services, branches, packages, customer appointments, enquiries, orders, and administrative operations.

The system provides separate functionality for **Customers and Admins**, allowing customers to register, browse laboratory packages and branches, book appointments, make online payments, manage their profiles, and view their orders. Administrators can manage branches, packages, appointments, enquiries, contacts, orders, and gallery content through an administrative dashboard.

## Features

- Customer registration and login
- Secure logout and password reset
- Customer profile creation and updating
- Laboratory branch management
- Laboratory package/test management
- Subpackage/content management
- Branch-wise package browsing
- Appointment booking
- Appointment filtering by branch and date
- Customer enquiries
- Contact-us management
- Customer testimonials
- Gallery management
- Customer order history
- Admin dashboard with order and package statistics
- Branch-wise and package-wise order filtering
- Branch-wise enquiry and contact filtering
- Online payment processing
- Razorpay payment verification and status management
- Payment success/failure handling

## User Roles

### Customer
- Register and log in
- Browse laboratory branches and packages
- View package details
- Book appointments
- Make online payments
- View previous orders
- Create and update profile information
- Submit enquiries and testimonials

### Admin
- Manage laboratory branches
- Add, update and delete packages
- Manage package sub-content
- Manage branch timings
- View and filter appointments
- View customer enquiries
- View customer contact messages
- View customer orders
- Manage gallery images
- Monitor package, branch and order statistics

## Technology Stack

- **Backend:** Python, Django
- **Frontend:** HTML, CSS, Bootstrap
- **Database:** SQLite
- **Authentication:** Django Authentication
- **Payment Gateway:** Razorpay
- **Email:** Django Email Backend
- **ORM:** Django ORM

## Database

The application uses a relational database through Django ORM.

Key database entities include:

- User
- Profile
- Branch
- Branch Time
- Package
- Subpackage
- Order
- Appointment
- Contact
- Enquiry
- Testimonial
- Gallery

The models use Django relationships such as **ForeignKey** to connect packages with branches, orders with customers/packages/branches, and appointments/enquiries/contacts with branches.

## Payment Integration

The system integrates **Razorpay** for online package payments.

The payment workflow includes:

1. Customer selects a laboratory package.
2. A Razorpay order is created.
3. The order is stored in the database.
4. Razorpay processes the payment.
5. The callback receives the payment details.
6. The Razorpay signature is verified.
7. The order status is updated as **Success** or **Failure**.

The implementation stores the Razorpay order ID, payment ID, signature ID and payment status for each order.

## Screenshots
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/8c0fa48f-395c-4815-a605-a92ee42328ac" />



## Live Demo

**Live Demo:**  
https://gmrllabs.pythonanywhere.com/

## GitHub Repository

**GitHub Repository:**  
https://github.com/RaveenaLaiju/gmrllab.git
