Topic:
Event Planning: Create a tool for organizing and promoting community events.
Problem 1: No Volunteer or Staff Coordination Features

Most event tools focus on attendee registration and promotion, but they lack features for managing internal teams — such as assigning volunteers, tracking staff availability, and handling last-minute changes, which leads to confusion, missed tasks, and poor coordination. (Eventbrite, 2023; Meetup, 2023)
Requirement 1: The system should allow organizers to manage volunteer/staff roles clearly.
Assumptions with Validation
Assumption 1:
Organizers want to assign internal roles like registration.
•	Validation:
o	Interview 3–5 community organizers about their planning process. (Lucas, 2014).
o	Review tools like Eventbrite and Meetup that don't provide internal staff planning features. (Eventbrite, 2023; Meetup, 2023)
Follow-Up Questions:
•	What are your most common internal roles?
•	Do you prefer assigning them digitally or on paper?
Assumption 2:
Organizers currently use spreadsheets or informal tools to manage roles.
•	Validation:
o	Ask for examples (Google Sheets, paper lists, etc.) during interviews(Google Sheets Templates, n.d.).
o	Review shared planning templates on nonprofit forums or VolunteerMatch blogs(VolunteerMatch, n.d.).
Follow-Up Questions:
•	What’s missing from the tools you use now?
•	Would a built-in role assignment tool simplify your process?
Preliminary Tasks
•	Build a role assignment table (columns: name, role, shift time, contact).
o	Create an editable table with sample data and test with organizers.
•	Add ability to edit/update roles in real-time.
o	Implement an "Edit" and "Save" button for each row entry.
•	Test with sample roles: greeter, tech support, cleanup crew.
o	Assign at least 3 sample roles in a test run and get user feedback.
Metrics for Success
•	At least 3 unique roles can be added and assigned.
•	Organizers can edit/update/delete role assignments.
•	Pilot testers confirm it is easier than using spreadsheets.
 Outcome
Organizers can assign tasks with clarity, reducing confusion and ensuring everyone knows their responsibilities.
Requirement 2: The system should show each volunteer/staff member their own schedule.
Assumptions with Validation
Assumption 1:
Volunteers need personalized views showing only their assigned tasks.
•	Validation:
o	Compare Eventbrite’s generic event view with a prototype dashboard(Eventbrite, 2023).
o	Ask volunteers from local events how they currently get task info (e.g., SMS, email chains).
Follow-Up Questions:
•	Do you often get confused about where and when you need to help?
•	Would a dashboard or printed handout help?
Assumption 2:
Volunteers often access information on mobile, not desktops.
•	Validation:
o	Survey event volunteers on preferred device usage.
o	Test mobile responsiveness of existing sites like VolunteerMatch (VolunteerMatch, n.d.).
Follow-Up Questions:
•	Do you check your schedule while on the move?
•	Would reminders via email/SMS help reduce no-shows?

Preliminary Tasks
•	Create a responsive “My Tasks” dashboard view.
o	Design a mobile-friendly layout and test it on 3 different screen sizes.
•	Add toggle for mobile vs. desktop layouts.
o	Implement a responsive toggle using CSS media queries.
•	Optionally allow volunteers to request reminders.
o	Add a checkbox in the dashboard for opting into email/SMS alerts.
 Metrics for Success
•	100% of volunteers can access and view their personal schedule.
•	Dashboard passes usability testing on mobile and desktop.
•	At least 80% report improved clarity on their responsibilities.
Outcome
Volunteers stay informed, improving attendance and reducing operational chaos.
Requirement 3: The system should help organizers track volunteer availability.
Assumptions with Validation
Assumption 1:
Organizers want to match volunteers based on their availability.
•	Validation:
o	Test availability fields in volunteer sign-up forms.
o	Compare with platforms like Eventbrite, which lack built-in availability collection(Eventbrite, 2023).
Follow-Up Questions:
•	How do you currently track availability—do you ask, call, or assume?
•	Would a “filter by free volunteers” feature help?
Assumption 2:
Volunteers sometimes cancel last-minute, so organizers want automatic alerts or reassignment.
•	Validation:
o	Interview organizers about dropout frequency and how they adjust.
o	Review best practices on VolunteerMatch for managing changes (VolunteerMatch, n.d.).
Follow-Up Questions:
•	Would automatic notifications help when a shift becomes unassigned?
•	Should the system suggest backups from available volunteers?
Preliminary Tasks
•	Add availability input to sign-up forms.
o	Include a multi-select field for days and time blocks.
•	Create filtering logic for matching based on time slots.
o	Build a filter that shows only volunteers available for selected roles.
•	Develop an alert or “auto-fill with backup” feature.	
o	Send an email alert and show a suggested replacement from available pool.
Metrics for Success
•	At least 80% of volunteers fill out their availability.
•	Fewer than 10% of shifts go unfilled due to dropouts.
•	Alerts are triggered for all unfilled shifts within 15 minutes.
Outcome
Organizers can confidently assign roles knowing volunteers are available and replacements are ready in case of cancellations.
