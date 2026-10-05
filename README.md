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
Home Page:-
<img width="1920" height="908" alt="Screenshot (81)" src="https://github.com/user-attachments/assets/ef81ef0c-879d-4c9d-ae8e-2595b9a11d51" />

Customer Registration:-
<img width="1920" height="842" alt="Screenshot (82)" src="https://github.com/user-attachments/assets/cdc7689a-21c7-4a6d-be50-4baf1005fe1c" />

Customer Login:-
<img width="1920" height="766" alt="Screenshot (83)" src="https://github.com/user-attachments/assets/a1a34546-7f06-42a9-972c-f108933805f5" />

Packages:-
<img width="1920" height="872" alt="Screenshot (85)" src="https://github.com/user-attachments/assets/f1a35c8e-9ca9-4aba-883b-aed2ddab14e1" />

Packages Details:- 
<img width="1920" height="895" alt="Screenshot (86)" src="https://github.com/user-attachments/assets/a3515523-2047-4872-bf11-91851bacc2c0" />

Appointment Booking:-
<img width="1920" height="896" alt="Screenshot (87)" src="https://github.com/user-attachments/assets/42273d8a-43de-48dc-995a-cae192e77ec0" />

Razorpay Payment:-
<img width="1920" height="885" alt="Screenshot (93)" src="https://github.com/user-attachments/assets/3015b5ed-a7fa-4018-9249-b840a0ef1df3" />

Admin Dashboard:-
<img width="1920" height="903" alt="Screenshot (88)" src="https://github.com/user-attachments/assets/dd2c547e-8b86-4971-b465-0d463be77342" />

Package Management:-
<img width="1920" height="891" alt="Screenshot (91)" src="https://github.com/user-attachments/assets/69140d90-7be7-4e0a-b80c-eb78b83e4d77" />
<img width="1920" height="860" alt="Screenshot (92)" src="https://github.com/user-attachments/assets/c23c1b14-c7e1-46f6-aa26-7db9c190918f" />

Appointment Management:-
<img width="1920" height="897" alt="Screenshot (89)" src="https://github.com/user-attachments/assets/b6ad8726-31d5-40e2-a40f-04174b0a8a0d" />

Gallery:-
<img width="1920" height="880" alt="Screenshot (90)" src="https://github.com/user-attachments/assets/63d6ef75-db7d-4702-b059-b41628a52e53" />


## Live Demo

**Live Demo:**  
https://gmrllabs.pythonanywhere.com/

## GitHub Repository

**GitHub Repository:**  
https://github.com/RaveenaLaiju/gmrllab.git
