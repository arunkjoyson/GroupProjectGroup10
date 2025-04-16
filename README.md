Here's the exact wording you requested in the correct format for `README.md`:

```markdown
# Group Project - Group 10

### Members:
- Arun Kanjirathingal Joyson (8955136)
- Nithin George Lorance (8989714)

## Topic:
Event Planning: Create a tool for organizing and promoting community events.

## Problem 1: No Volunteer or Staff Coordination Features
Most event tools focus on attendee registration and promotion, but they lack features for managing internal teams — such as assigning volunteers, tracking staff availability, and handling last-minute changes, which leads to confusion, missed tasks, and poor coordination. (Eventbrite, 2023)

### Requirement 1: The system should allow organizers to manage volunteer/staff roles clearly.

#### Assumptions with Validation
- **Assumption 1:**
  - Organizers want to assign internal roles like registration.
  - **Validation:**
    - Interview 3–5 community organizers about their planning process. (Lucas, 2014).
    - Review tools like Eventbrite and Meetup that don't provide internal staff planning features. (Eventbrite, 2023; Meetup, 2023)
  - **Follow-Up Questions:**
    - What are your most common internal roles?
    - Do you prefer assigning them digitally or on paper?

- **Assumption 2:**
  - Organizers currently use spreadsheets or informal tools to manage roles.
  - **Validation:**
    - Ask for examples (Google Sheets, paper lists, etc.) during interviews(Google Sheets Templates, n.d.).
    - Review shared planning templates on nonprofit forums or VolunteerMatch blogs(VolunteerMatch, n.d.).
  - **Follow-Up Questions:**
    - What’s missing from the tools you use now?
    - Would a built-in role assignment tool simplify your process?

#### Preliminary Tasks
- [ ] Build a role assignment table (columns: name, role, shift time, contact).
  - Create an editable table with sample data and test with organizers.
- [ ] Add ability to edit/update roles in real-time.
  - Implement an "Edit" and "Save" button for each row entry.
- [ ] Test with sample roles: greeter, tech support, cleanup crew.
  - Assign at least 3 sample roles in a test run and get user feedback.

#### Metrics for Success
- [ ] At least 3 unique roles can be added and assigned.
- [ ] Organizers can edit/update/delete role assignments.
- [ ] Pilot testers confirm it is easier than using spreadsheets.

#### Outcome
Organizers can assign tasks with clarity, reducing confusion and ensuring everyone knows their responsibilities.

---

### Requirement 2: The system should show each volunteer/staff member their own schedule.

#### Assumptions with Validation
- **Assumption 1:**
  - Volunteers need personalized views showing only their assigned tasks.
  - **Validation:**
    - Compare Eventbrite’s generic event view with a prototype dashboard(Eventbrite, 2023).
    - Ask volunteers from local events how they currently get task info (e.g., SMS, email chains).
  - **Follow-Up Questions:**
    - Do you often get confused about where and when you need to help?
    - Would a dashboard or printed handout help?

- **Assumption 2:**
  - Volunteers often access information on mobile, not desktops.
  - **Validation:**
    - Survey event volunteers on preferred device usage.
    - Test mobile responsiveness of existing sites like VolunteerMatch (VolunteerMatch, n.d.).
  - **Follow-Up Questions:**
    - Do you check your schedule while on the move?
    - Would reminders via email/SMS help reduce no-shows?

#### Preliminary Tasks
- [ ] Create a responsive “My Tasks” dashboard view.
  - Design a mobile-friendly layout and test it on 3 different screen sizes.
- [ ] Add toggle for mobile vs. desktop layouts.
  - Implement a responsive toggle using CSS media queries.
- [ ] Optionally allow volunteers to request reminders.
  - Add a checkbox in the dashboard for opting into email/SMS alerts.

#### Metrics for Success
- [ ] 100% of volunteers can access and view their personal schedule.
- [ ] Dashboard passes usability testing on mobile and desktop.
- [ ] At least 80% report improved clarity on their responsibilities.

#### Outcome
Volunteers stay informed, improving attendance and reducing operational chaos.

---

### Requirement 3: The system should help organizers track volunteer availability.

#### Assumptions with Validation
- **Assumption 1:**
  - Organizers want to match volunteers based on their availability.
  - **Validation:**
    - Test availability fields in volunteer sign-up forms.
    - Compare with platforms like Eventbrite, which lack built-in availability collection(Eventbrite, 2023).
  - **Follow-Up Questions:**
    - How do you currently track availability—do you ask, call, or assume?
    - Would a “filter by free volunteers” feature help?

- **Assumption 2:**
  - Volunteers sometimes cancel last-minute, so organizers want automatic alerts or reassignment.
  - **Validation:**
    - Interview organizers about dropout frequency and how they adjust.
    - Review best practices on VolunteerMatch for managing changes (VolunteerMatch, n.d.).
  - **Follow-Up Questions:**
    - Would automatic notifications help when a shift becomes unassigned?
    - Should the system suggest backups from available volunteers?

#### Preliminary Tasks
- [ ] Add availability input to sign-up forms.
  - Include a multi-select field for days and time blocks.
- [ ] Create filtering logic for matching based on time slots.
  - Build a filter that shows only volunteers available for selected roles.
- [ ] Develop an alert or “auto-fill with backup” feature.	
  - Send an email alert and show a suggested replacement from available pool.

#### Metrics for Success
- [ ] At least 80% of volunteers fill out their availability.
- [ ] Fewer than 10% of shifts go unfilled due to dropouts.
- [ ] Alerts are triggered for all unfilled shifts within 15 minutes.

#### Outcome
Organizers can confidently assign roles knowing volunteers are available and replacements are ready in case of cancellations.

---

## Problem 2: No Support for Physical Promotion
Most marketing tools prioritize digital promotion methods such as email and social media. However, for local community events, traditional outreach methods including flyer distribution, poster placement, and word-of-mouth continue to play a critical role. Current platforms lack features to plan or track physical promotion tasks, resulting in limited visibility, inefficiencies, and missed outreach opportunities. (Lucas, 2014)

### Requirement 4: The system should allow organizers to track physical marketing tasks such as flyer distribution, poster placement, or booth setup.

#### Assumptions with Validation
- **Assumption 1:**
  - Event organizers continue to use physical promotion methods such as flyers and posters.
  - **Validation:**
    - Conduct interviews with local event planners regarding their current promotional strategies(Lucas, 2014).
    - Administer a short survey to determine what percentage of outreach efforts are conducted offline.
  - **Follow-Up Questions:**
    - How often do you use flyers or posters to promote events?
    - Which areas are commonly targeted for physical outreach?

- **Assumption 2:**
  - Organizers need to track which volunteers completed assigned promotional tasks and when.
  - **Validation:**
    - Interview both organizers and volunteers to understand current accountability practices. (VolunteerMatch, n.d.)
    - Prototype a basic task confirmation form that includes options like checkbox, timestamp, or photo upload, and gather user feedback.
  - **Follow-Up Questions:**
    - Do you require visual or written confirmation of completed tasks?
    - Would location-based tracking (e.g., GPS tags) be beneficial?

#### Preliminary Tasks
- [ ] Add a “Physical Promotion Plan” section to the event creation form.
  - Include form fields for task type (e.g., flyer, poster), assigned personnel, and location details.
- [ ] Create a simple task confirmation form for volunteer use.	
  - Implement checkbox functionality and optional file upload to verify task completion.

#### Metrics for Success
- [ ] Organizers are able to assign and complete tracking for at least three physical promotion tasks.
- [ ] Completion status is visible to both the organizer and volunteer.
- [ ] A minimum of 70% of assigned tasks are verified using a timestamp or photo.

#### Outcome
Organizers are able to plan and oversee offline outreach efforts more effectively, resulting in better coverage, higher community visibility, and improved event attendance.

---

### Requirement 5: The system should allow scheduling of physical promotion tasks in advance.

#### Assumptions with Validation
- **Assumption 1:**
  - Organizers require the ability to schedule physical promotion tasks ahead of time.
  - **Validation:**
    - Conduct user interviews to determine if organizers plan outreach based on specific dates or times. (Lucas, 2014)
    - Test calendar-based scheduling during trials to assess improvements in planning efficiency.
  - **Follow-Up Questions:**
    - Do you prefer to schedule all outreach at once, or adjust tasks as needed?
    - Would recurring task options (e.g., weekly poster placements) be useful?

- **Assumption 2:**
  - Certain physical locations are considered high-priority for outreach and should be visually prioritized or mapped.
  - **Validation:**
    - Interview organizers to identify their most frequently used outreach areas.
    - Introduce a map-based tagging feature and monitor adoption rates in early testing.
  - **Follow-Up Questions:**
    - Which locations (e.g., libraries, markets) do you prioritize for flyer/poster placement?
    - Would a visual map interface help with outreach organization?

#### Preliminary Tasks
- [ ] Add scheduling capability to the physical promotion task creation form.
  - Include calendar date and time pickers for each task assignment.
- [ ] Integrate a location tagging map into the promotion planning module.	
  - Implement Google Maps API to allow users to drop pins and label outreach sites.

#### Metrics for Success
- [ ] Organizers successfully schedule a minimum of three physical promotion tasks.
- [ ] Map-based tagging is used for two or more locations per event.
- [ ] Post-task feedback from users confirms improved scheduling and area targeting.

#### Outcome
The planning and execution of physical outreach becomes more structured, allowing organizers to allocate volunteer resources effectively and ensure that high-impact areas are not missed.

---

### Requirement 6: The system should help track the effectiveness of physical promotion.

#### Assumptions with Validation
- **Assumption 1:**
  - Organizers are interested in understanding how many attendees learned about the event through physical promotion.
  - **Validation:**
    - Add a referral question (e.g., “How did you hear about us?”) in the event registration form.
    - Distribute flyers with unique QR codes or promo codes and analyze the resulting engagement data.
  - **Follow-Up Questions:**
    - Are you currently measuring how effective physical promotion is?
    - Would you consider tracking offline engagement via codes or referral questions?

- **Assumption 2:**
  - Data from physical promotion can be used to improve future outreach strategies.
  - **Validation:**
    - Review flyer-related QR code scans and promo code redemptions.
    - Compare offline marketing results against online promotional efforts.
  - **Follow-Up Questions:**
    - Have you ever adjusted your outreach plan based on feedback or attendance data?
    - Would real-world data on physical promotion impact influence your future approach?

#### Preliminary Tasks
- [ ] Add a referral tracking question to the event registration form.
  - Include a dropdown menu listing options like flyer, poster, and word-of-mouth.
- [ ] Generate trackable QR codes for each printed flyer batch.
  - Create URLs with tracking parameters and generate QR codes linked to those URLs.

#### Metrics for Success
- [ ] At least 50% of event registrants respond to the referral source question.
- [ ] QR codes or promo codes are scanned or used a minimum of 25 times per event.
- [ ] Organizers report clearer insights into the impact of their physical outreach strategies.

#### Outcome
Organizers gain actionable data on the effectiveness of their offline promotional campaigns, enabling them to make data-driven improvements in future event planning.

---

### Reference:
- Eventbrite. (2023). How to organize an event. https://www.eventbrite.com/blog/academy/ 
- Google Sheets Templates. (n.d.). Event planning templates. https://docs.google.com/templates 
- Lucas, M. J. (2014). The organizing practices of a community festival. Journal of Organizational Ethnography, 3(2), 275–290. https://doi.org/10.1108/JOE-01-2013-0001
- VolunteerMatch. (n.d.). Blog & best practices for volunteer coordination. https://www.volunteermatch.org/
``` 

This is in the exact format, keeping the structure and content unchanged. Let me know if you need anything else!