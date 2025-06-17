Event Guest List Manager
A browser-based tool for managing event guests
Version: 1.0 — June 2025
By: Angel Lucy

Description
The Event Guest List Manager allows users to manage a simple guest list directly from their browser. Users can type a guest's name into an input field and submit the form to see that name appear in a list on the page. Each guest entry includes controls for managing RSVP status, editing names, categorizing guests, and removing them from the list.

This app was built as part of a coding challenge to practice DOM manipulation, form handling, and user interaction with vanilla JavaScript.

Problem Statement
The Event Guest List Manager solves the challenge of managing and organizing event guest lists dynamically on a webpage without the need for a database, spreadsheet, or page reload. More specifically, it addresses these challenges:

✅ Dynamic Data Entry
Users can add guest names seamlessly without refreshing the page. Each guest’s information is temporarily stored in the DOM, streamlining input and interaction.

🚫 Guest Capacity Control
Prevents overbooking by enforcing a maximum guest limit (e.g., 10 guests), helping organizers keep their event manageable.

🎨 Category Assignment
Guests can be classified into categories such as Friend, Family, or Colleague, with distinct background colors to visually differentiate each category for better organization.

🔁 Live Interactivity
Users can toggle RSVP status with a single click, edit guest names in-place, and remove guests easily — all without page reloads.

⏱️ Timestamp Logging
Each guest entry includes a timestamp indicating when they were added, useful for record keeping and providing real-time UI feedback.

Setup/Installation Requirements
To run this application locally:

Clone the repository:

bash
Copy
Edit
git clone https://github.com/Angellucy460/Code-Challenge-2.git
Open the project folder in Visual Studio Code.

Install and use the Live Server extension:

Right-click on index.html and choose "Open with Live Server".

Your browser will open automatically (usually at http://127.0.0.1:5500/).

How It Works Behind the Scenes
When a user submits a guest’s name:

Page Load Listener
The script waits for the full DOM to load before accessing elements like the form and guest list.

Form Submission Handling
The form’s default behavior is intercepted with event.preventDefault() to prevent a page reload.

Guest Input Validation

Empty names are ignored.

Guest limit is capped at 10. If exceeded, an alert appears.

Dynamic Element Creation
An <li> is created with the following:

A <span> for the guest’s name

A <select> for category (with background color styling)

RSVP toggle (adds a strikethrough for “Attending”)

Edit button (renames the guest)

Remove button (deletes guest and updates count)

Timestamp showing when the guest was added

DOM Injection
The new list item is added to the DOM via guestList.appendChild(...), the total count is updated, and the form resets for the next input.

Features
Add guest names dynamically

Limit guest list to 10 people

Edit names via prompt

Mark guests as attending

Categorize guests (with color-coded dropdown)

Remove guests with one click

Timestamp showing when the guest was added

Known Bugs
There are currently no known bugs. The application functions as expected.

Technologies Used
HTML for page structure

CSS for styling

JavaScript for dynamic interaction, DOM manipulation, and form validation

Support and Contact
For feedback, questions, or issues, feel free to reach out:
📧 angelliona38@gmail.com
📞 +254 790781575
💻 GitHub: https://github.com/Angellucy460/Code-Challenge-2
Contributions welcome — feel free to fork and submit pull requests!

License
MIT License
Copyright (c) 2025
Angel Lucy

