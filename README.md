# alx-airbnb-database
This is for my Alx pro back-end dev course
Team roles ;
Backend Developer-Builds and maintains the server-side logic of web or mobile applications.
Database Administrator-Designs, implements, and maintains database systems.
Business Analyst-Gathers and analyzes business needs and requirements.
Product Manager-Defines the vision and strategy for a product.
Technology Stack;
Django-to build secure, scalable, and maintainable web applications quickly.
PostgreSQL-to store, manage, and query structured data.
GraphQL-to request only the data they need.
Python-For high-performance API framework.
Database Design;
Users,
id: Unique identifier for each user

name: Full name of the user

email: User’s unique email address

password: Encrypted password for login

role: Indicates whether the user is a host or guest
 Properties,
 id: Unique identifier for each property

title: Property name/title

location: City and country

price_per_night: Cost of staying per night

host_id: Refers to the user who owns the property
Bookings,
id: Unique identifier for each booking

user_id: Refers to the guest who made the booking

property_id: Refers to the booked property

start_date: Start of the stay

end_date: End of the stay
Reviews,
id: Unique identifier for each review

user_id: Refers to the user who wrote the review

property_id: Refers to the reviewed property

rating: Score given by the user 

comment: Text feedback
Payments,
id: Unique identifier for the payment

booking_id: Refers to the related booking

amount: Total payment amount

payment_date: When the payment was made

status: Payment status
Relationships,
A review is for one property
A booking is made by one user for one property
A property can have multiple bookings
A property belongs to one user
A user can own multiple properties
A user can leave multiple reviews
Feature Breakdown;
User Management- allows users to sign up, log in, manage profiles, and define roles
Property Management- allows hosts to add, update, and manage property listings
Booking System-allows guests to select available dates and reserve properties
Payment System-allows users to make secure payments for bookings using various methods
Search and Filter Functionality-enables users to search for properties based on location, price, dates, and more
Property Image Gallery-allows hosts to upload multiple images per listing, and guests to view them in a gallery layout
