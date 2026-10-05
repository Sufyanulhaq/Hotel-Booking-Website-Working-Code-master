Hotel Booking Website
=====================

An early full stack project (2023): a hotel booking site in plain PHP and MySQL, with an admin panel to run it. Kept here to show where I started; my current work is in the newer repositories on my profile.

What it does
------------

**For guests**

* Search hotels and browse rooms, room types, photo galleries and packages
* Book a room and pay online through Instamojo
* Request a refund, book a cab, send an enquiry and join the newsletter
* Read and leave reviews

**For the admin** (`backend/`)

* Add, edit and remove hotels, rooms, room galleries, packages and cabs
* Manage the home page slider, highlights section and footer
* See bookings, enquiries and newsletter sign ups

Built with
----------

PHP, MySQL, JavaScript, jQuery, Bootstrap and the Instamojo PHP client.

Run it
------

1. Create a MySQL database and import `hotel.sql`.
2. Set the database details in `connect.php` and `backend/connect.php`.
3. Set your Instamojo keys as environment variables (`INSTAMOJO_API_KEY` and `INSTAMOJO_AUTH_TOKEN`). Use sandbox keys for testing.
4. Serve the folder with PHP, for example `php -S localhost:8000`.

What I would do differently today
---------------------------------

This was written before I used frameworks and tests. Today I would use prepared statements for every query, keep secrets out of the code from the start, check payments with the provider's webhook instead of trusting the return page, and add automated tests. My recent projects do all of these.
