✅ Institutional Activity Oversight and Management System (IAOMS) – HITAM

🎯 Objective:
To build a decentralized, secure, and automated digital system for managing Permission Reports / Letters / Circulars, streamlining submission, approval, signature, and tracking between Employees and HITAM Authorities

🧑‍💻 Tech Stack Overview
Layer
Technology
Frontend
React + Tailwind CSS + Shadcn/ui + Vite(with White & Green UI theme)
BackEnd - TypeScript + Node.js
Auth
SuperBase Authentication (Google Sign-In + HITAM ID login + HITAM ID Roll No With Password)
Storage
Google Drive API (report uploads)
Realtime DB
SuperBase Realtime Database 
Notifications
WebSocket API
Email Alerts
SuperBase Cloud Functions + SendGrid + Gmail API (Google Mail)




🤖 AI-Powered Future Enhancements
🧠 Grammar Correction using Google Gemini + Google API before report submission


🧾 AI-Powered Summary of report for reviewer preview


📊 Activity analytics dashboard for management


AI-based templates using Google Gemini + Google API)



Integrated Workflow for All Kinds of Recipient Roles
Technologies Used:
🔑 Google API Key


📁 Google Drive


📊 Google Sheets


📄 Google Docs


📧 Gmail API (Google Mail)


📑 Google Forms


📈 Microsoft Excel


🤖 Google Gemini (via PaLM API)


🔥 SuperBase (Authentication & Database)



1. 📄 Automated Document Generation
Utilize Google Docs templates and Apps Script to dynamically generate:


Letters


Circulars


Reports


Automatically populate content from Google Forms or Sheets.


2. 🤖 AI-Powered Summarization & Drafting
Integrate Google Gemini (PaLM API) to:


Summarize long inputs (e.g., student requests, event details)


Auto-draft circulars or reports from structured form responses


3. 📂 Document Storage & Access Control
Store all documents securely in Google Drive folders.


Use SuperBase Authentication for login and role-based access (Employee/Principal).


Maintain access logs and versioning history.


4. 📬 Automated Notifications
Trigger real-time email alerts via Gmail API for:


Document submission


Approval or rejection


Comments added by approvers







✅ UI & UX Design Requirement for Document Sending System

📄 1. Document Type Selection
Provide a dropdown or multi-select toggle to choose one or more of the following document types:
✅ Letter


✅ Circular


✅ Report



📤 2. Advanced Upload Options (For Principal & Employee)
Allow users to upload files from multiple sources, including:
📁 Google Drive


📊 Google Sheets / Microsoft Excel


📄 Google Docs


📷 Images


📂 Local Uploads


Advanced Upload Options (for Principal & Employee):
Ability to upload Google Forms, Excel sheets, Google Docs, Microsoft Excel,  images, and various file types:
Supported File Formats:
.pdf, .doc, .docx, .xlsx, .xls, .png, .jpg, .jpeg



👥 3. Role-Based Recipient Selection (Multi-Select Dropdown)
Provide a searchable multi-select list of recipients with clear labels and grouped by sender type:

📤 Principal – Authorized Recipients
Mentors/Employees/faculty (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


 Program Department Heads (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


HODs (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)
Registrar


CDC Department Employees


Dean


Chairman


Director (For Information)


Leadership


Controller of Examinations


Asst. Dean IIIC


Head Operations


Librarian


SSG
Registar




📤 Employee – Authorized Recipients
 Program Department Heads (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


HODs (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


Registrar


Principal



🚀 4. Submission Workflow
Once the user selects the document type, uploads the file(s), and selects recipients, clicking Submit should:
✅ Automatically send email notifications to each selected role


✅ Trigger a dashboard alert (in-app notification) for each recipient


✅ Display a confirmation message:


“✅ Document successfully sent and notifications delivered to selected roles.”

 UI/UX interpretation 
✅Approval & Rejection Component (Design)
This component allows reviewers ( To All The recipients) to approve or reject Letters, Circulars, or Reports with a comment 

💡 UI Layout (Horizontal Inline)
[ ✅ Approved ]    [ ❌ Rejected ]     [ 💬 Add Comment Here... ]
     (Green)            (Red)                (Text Field)

Approved Button


Label: Approved


Color: Green (#28a745)


On click: Highlights green, locks comment, and submits with timestamp


Rejected Button


Label: Rejected


Color: Red (#dc3545)


On click: Highlights red, locks comment, and submits with timestamp


Comment Field


Optional but encouraged (especially on rejection)


Input type: Textarea or single-line input


Placeholder: Enter your comment ...



🔁 Workflow Triggered On Action
✅ If Approved: Signature panel opens (if enabled),Sends notification and email + status updated


❌ If Rejected: Sends notification and email + status updated + saves comment reason + marks in red


💬 All actions are saved with:


User role


Date & time


Status (approved/rejected)


comment



Auto-Generate Analytics Dashboard
🎯 Purpose
Visually track:
Number of reports submitted, approved, rejected


Department-wise report activity


Average approval time


Most active users/faculty


Monthly/yearly trends



✅ Universal Search 
🔍 Universal Search Integration
Implement a global search feature that allows users to search across all modules:
🔎 Letters, Circulars, Reports


🧑‍💼 User Names (All Kind of Recipients)


🏢 Departments


📅 Events & Meetings


📂 Document Status (In Progress, Approved, Rejected)


💡 Include:
Tag filters and autocomplete suggestions


Role-based visibility for search results


Real-time updates using Firestore indexing or Supabase full-text search




Sticky Notes Canvas UI – In-Website Short Reminder Notes Module for IAOMS
✅ Purpose:
Allow Recipients and all authorized roles to jot down short personal notes or task reminders directly within the IAOMS website—without needing external apps.

🧩 Key Features:
Sticky Notes Canvas UI


Add, move, edit, or delete sticky notes.


Color-coded notes (📘 blue for tasks, 🟩 green for meeting points, 🟥 red for urgent reminders).


Quick Access Panel


Accessible from dashboard side panel or top navbar.


Click “📝 Notes Canva” to expand/collapse.


Auto-Save & Time Stamp


Notes are auto-saved to the user’s account.


Shows last edited time and creation time.


Rich Text Support


Bold, bullet points, headings, emojis 😊


Link attachments (e.g., Google Doc, Meeting ID, etc.)


Optional Reminder Alerts


Convert any note into a reminder.


Choose date/time for browser push or Gmail alert.


Search & Tag


Add tags to notes (e.g., #meeting, #followup).


Search notes via keywords or tags.


AI Suggestion Mode (Optional)


Gemini or ChatGPT can suggest note titles or extract to-do items from meeting uploads.



👨‍🏫 Example Use Case:
"Create a note after the Principal's meeting:
 📌 'Update student attendance policy doc before Friday review' — #urgent #principal #circular"



✅ Dynamic Dashboards – Role-Based UI Personalization
Display a customized dashboard depending on the role of the logged-in user. After login/signup, the user’s role All Kind of Recipients is retrieved from the database and used to dynamically render relevant components.

🎯 How It Works:
On Successful Login:


Fetch user role from database (users collection/table).


Store it in session or localStorage.


Dashboard Rendering Logic (Frontend Example):


if (role === 'Principal') {
  render(<PrincipalDashboard />);
} else if (role === 'Registrar') {
  render(<RegistrarDashboard />);
} else if (role === 'HOD-CSE') {
  render(<HODDashboard department="CSE" />);
} else {
  render(<EmployeeDashboard />);
}

🧩 UI Per Role 
🟥 Principal Dashboard
✅ View & approve all circulars, reports, and letters


✅ Mass document distribution (to HODs, Program Heads, etc.)


✅ Escalation management (bi-directional routing, auto-escalation)


✅ Role management (assignments, overrides)


✅ View analytics (document stats, delays, trends)


✅ Signature dashboard (multi-recipient digital signature collection)


✅ Meeting scheduling (with approval workflows, smart suggestions)


✅ Receive high-priority alerts during meetings


✅ Access to “Live Meet” requests from employees



🟨 Registrar Dashboard
✅ Workflow routing approvals (between departments)


✅ Counter-approvals and conditional escalation


✅ View circulars pending from HODs/Principal


✅ AI summaries of submitted documents


✅ Role-wise activity logs


✅ Access document lifecycle tracking


✅ Emergency document receipt and signature handling



🟦 HOD Dashboard (EEE, MECH, CSE, ECE, CSM, CSO, CSD, CSC — 1st to 4th Year)
✅ Submit and approve reports, circulars, letters


✅ Re-upload or return rejected files


✅ Calendar view for department events/meetings


✅ Self-reminder notifications (document or meeting follow-ups)


✅ Auto-generated MoM (Minutes of Meeting) for scheduled events


✅ Track approvals by role and status


✅ Access real-time chat for role-based communication



🟩 Program Heads Dashboard (All Branches & Years)
✅ Same as HODs (department-level management)


✅ Focused on academic scheduling and circular approvals


✅ Document upload and tracking


✅ Reminder and task manager integration


✅ Review and signature panel with e-signature or scanned input



🟧 Employees Dashboard
✅ Submit new documents (Letters, Circulars, Reports)


✅ Choose routing: HOD ➝ Program Head ➝ Registrar ➝ Principal


✅ Track submission status (Approved, Rejected, Pending)


✅ Re-submit rejected reports with updated attachments


✅ Smart notes/reminder (Notes Canva) integration


✅ Emergency document submission with direct access


✅ Access to Live Meet scheduling with approvers


✅ AI-generated summaries of submitted reports



✅ Other Shared UI Features for All Roles:
🔍 Universal Search: Search across reports, dates, recipients, and keywords.


🔔 Notification Center: Email + in-app alerts on approvals, rejections, comments.


📊 Role-Based Analytics Dashboard: Submission rate, delay heatmaps, top contributors.


📅 Mini Calendar Widget: Shows upcoming tasks, meetings, and pending approvals.


📝 Notes Canva Panel: Sticky notes, auto-saved, color-coded with reminder options.


📂 Old Document Upload: Archive & refine older circulars with AI formatting.


📥 Multi-format Upload Support: .pdf, .docx, .xlsx, .jpg, Google Docs, Forms.


🤖 AI Support: Drafting, grammar checks, routing recommendations


💾 Where to Store Role Data:
🔐 Session/localStorage: for client-side access


📚 Database (Supabase): for persistent mapping


🎟️ JWT Claims: optionally embed role info inside tokens





✅Feature: Real Time Live Meet In-Person Communication Request
🔹 Purpose:
To allow real-time clarification or discussion before or during the approval/rejection process of Letters, Circulars, or Reports.

📌 For Employees
Employees can request or be invited to a Real Time Live Meet In-Person Communication Request at any stage of the workflow with the following authorized roles:
✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


✅ HODs (All Branches-EEE, MECH, CSE, ECE, CSM, CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


✅ Registrar


✅ Principal


🕒 Options Meeting Scheduler:
Date Picker


Time Slot Selector


Notes/Agenda (Optional field)


Authorized Recipients from the list below can also initiate a Real Time Live Meet In-Person Communication Request to the employee before making a final decision in Between Approved and Rejected Stages.

📌 For Principal
The Principal can also request a Real Time Live Meet In-Person Communication Request at any workflow stage (for better coordination or discussion) with the following roles:
✅Mentors/Employees/faculty (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)
✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)
✅ HODs (All Branches-EEE, MECH, CSE, ECE, CSM, CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)
 ✅ Registrar
 ✅ CDC Department Employees
 ✅ Dean
 ✅ Chairman
 ✅ Director (For Information)
 ✅ Leadership
 ✅ Controller of Examinations
 ✅ Asst. Dean IIIC
 ✅ Head Operations
 ✅ Librarian
 ✅ SSG
 
💬  Real Time Live Meet In-Person Communication Request Triggers:
✅ Optional toggle available on each approval/rejection screen


✅ Live Meet notification sent via email + dashboard alert to the other party


✅ Google Meet / Zoom link auto-generated (if integrated)



🗂️ Document Status Tracking by Role
Use status filters to categorize documents based on approval stages:
🟡 In Progress Approvals


🟠 Pending Documents


🔴 Rejected With Comments


🟢 Approved and Archived


📊 Track Based on Roles & Timelines
Identify which role is currently holding or has acted on the document.


Track how long each document has remained in each status.


Calculate total time taken by each role for approval or rejection.


View per-role metrics like:


Number of documents handled


Average approval/rejection time


Delay trends


✅ This enables better accountability, time management, and workflow optimization.


🔔 Self-Reminder Notification System
For Roles: All Recipients
✅ Purpose:
Allow users to set Self-Reminder Notification System for tasks, meetings, document actions, or follow-ups — all within the system, without waiting for external triggers.

💡 Features & Capabilities
📝 1. Reminder Setup Options
Title/Note Field (e.g., “Submit workshop circular for approval”)


Select Reminder Date & Time


Repeat Option: Daily / Weekly / Monthly / Custom


Priority Tag: 🔴 High, 🟡 Medium, 🟢 Low


Category Selection:


🗂 Document Follow-up


📅 Meeting


⏳ Pending Approval


✏️ Personal Note



🔁 2. Notification Modes
📩 Email Reminder sent via Gmail API


🔔 Dashboard Alert at scheduled time


📲 Optional WhatsApp Notification (via webhook if integrated)



🔄 3. Snooze & Reschedule
Users can snooze reminders (e.g., +10 mins, +1 hr, Tomorrow)


Easily reschedule or edit reminders from the dashboard



🗓️ 4. Integration with Calendar
Auto-sync with Google Calendar for better visibility


Display reminders in the IAOMS mini calendar widget


Option to attach documents or link existing workflows



🔐 5. Confidential & Role-Based
Only visible to the reminder creator


Designed to support internal personal productivity
 (not monitored by admins or other roles)



✅ Sample Use Cases:
User
Reminder
Time
Outcome
Employee
Upload signed circular
3:00 PM
Dashboard + email ping
Principal
Review upcoming project proposals
9:30 AM
Appears in “Today’s Reminders”
HOD-CSE
Prepare the monthly dept. report
July 31
Google Calendar + PDF draft linked



✅ Role-Based Access to Share Documents & Files – IAOMS
All the following authorized roles will have full access to share and collaborate on important institutional documents such as:
📄 Letters
 📃 Circulars
 📑 Reports
 📂 Google Docs
 📊 Google Sheets / Microsoft Excel
 📋 Google Forms
 📷 Images (JPEG, PNG)
 📁 Local Uploads (.pdf, .doc, .docx, .xlsx, .xls)

🎓 Authorized Roles with Share Access
✅ Principal


✅ Registrar


✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM, CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


✅ HODs (All Branches-EEE, MECH, CSE, ECE, CSM, CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


Mentors/Employees/faculty (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


✅ CDC Department Employees


✅ Dean


✅ Chairman


✅ Director (For Information)


✅ Leadership


✅ Controller of Examinations


✅ Asst. Dean IIIC


✅ Head Operations


✅ Librarian


✅ SSG



📤 System Capabilities:
🔄 Upload, View, Share, and Collaborate on documents in real-time


🧾 Access control via SuperBase or OAuth-based role mapping


🔗 Attach files in chat sessions, workflows, meeting scheduler, or dashboard


🧠 Google Gemini integration to auto-format shared documents


🔒 Role-based visibility to protect sensitive documents (e.g., confidential letters or academic reports)




⏳ Document Life Cycle Progress Tracker
Visual timeline indicators:


 Drafted ➝ Sent ➝ Under Review ➝ Approved ➝ Archived



Includes color-coded status bars and timestamp logs.


Boosts transparency and traceability.



📊 Unified Dashboard with Role-Based Widgets
Each user sees a personalized dashboard based on their role:
🔄 Pending Actions (Approve/Reject)


📬 Latest Letters/Circulars/Reports


📊 Document Stats (Daily, Weekly activity)


📅 Upcoming Meetings/Events


✅ Encourages accountability and streamlines navigation.


📈 Reporting & Analytics Panel (For Principal/Management)
Includes charts and KPIs such as:
📂 Number of documents sent/approved (by department, user)


⏱ Average approval/rejection time


📉 Delay or inactivity heatmap (monthly trends)


💬 Most active roles and document types


✅ Drives data-driven decision-making.

✅ Integrated Taskboard for Post-Approval Follow-ups
Automatically convert approved documents into task cards:


Status: 🟢 To Do / 🔵 In Progress / ✅ Done


Example: Circular: “AI Workshop” ➝ Task: Registrar to notify all HoDs


📌 Encourages action-based workflows beyond signatures.

🔥 Real-Time Dashboard Heatmaps
Visualize:


Departments with most pending documents


Active hours per user role


Approval/rejection cycle time


✅ Helps management optimize performance and allocate resources better.
⭐ Bookmark & Archive System
Allow users to:


Bookmark any document to “My Dashboard”


Add to “Starred for Action”


Create folders or personal archives (Private/Public)


✅ Enhances personalized tracking.


✅ Role-Based Document Routing System
📤 Principal — Authorized to Send To:
The Principal can send Letters, Circulars, or Reports and request signatures from the following authorized recipients:
Mentors/Employees/faculty (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


Program Heads  (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


HODs  (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


Registrar


CDC Department Employees


Dean


Chairman


Director (for information)


Leadership


Controller of Examinations


Asst. Dean IIIC


Head Operations


Librarian


SSG




📤 Employee — Authorized to Send To:
An Employee can send Letters, Circulars, or Reports and request signatures from:
Program Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


HODs  (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


Registrar


Principal



✅ UI & UX Design Requirement: Emergency Document Sending System
🔴 Emergency Send Button Feature
For critical or time-sensitive situations, provide a clearly labeled "Emergency Send" button. Upon activation, the system will:
Bypass standard approval flow


Immediately open a recipient selection interface


Allow Employees to send documents directly to any of the following authorized recipients:



📜 Authorized Recipients List (Emergency Access)
 ✅Mentors/Employees/faculty (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)
 ✅Program Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)
 ✅HODs  (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)
 ✅ Registrar
 ✅ CDC Department Employees
 ✅ Dean
 ✅ Chairman
 ✅ Director (For Information)
 ✅ Leadership
 ✅ Controller of Examinations
 ✅ Asst. Dean IIIC
 ✅ Head Operations
 ✅ Librarian
 ✅ SSG
 ✅ Principal

🧩 User Interface Behavior
Show a multi-select dropdown or checkbox list of the above roles.


Allow uploading of documents in common formats: .pdf, .doc, .xlsx, .png, .jpg, etc.


Trigger instant email + dashboard notification to selected recipients.


Highlight the document tag as “⚠️ Emergency Document”.







✅ Email & Dashboard Notification Flow

🔔 At Document Submission
When a Letter, Circular, or Report is submitted, the system will immediately:
📤 2. Advanced Upload Options (for Principal & Employee):
Allow file uploads from multiple sources:
📁 Google Drive


📊 Google Sheets / Microsoft Excel


📄 Google Docs


📷 Images (scanned documents or photos)


📂 Local Device Uploads


Supported File Formats:
 .pdf, .doc, .docx, .xlsx, .xls, .png, .jpg, .jpeg
📬 Triggered Actions:
📩 Instant Email Alert to all selected recipients with file and sender details.


📲 Dashboard Notification for each recipient:


 “You have received a new document for review and approval.”




✅ If Approved
When a recipient clicks “Approve”, optionally adding comments:
📩 Email Notification is sent to:


The original sender


All relevant roles/approvers


“Your document has been approved by [Role/Name] on [Date/Time].”



🟢 Dashboard Update on the sender’s screen:


Status: Approved


Approver’s name, date, and optional comments included.



❌ If Rejected
When a recipient clicks “Reject”, optionally adding a comment:
📩 Email Notification is sent to:


The original sender


Other reviewers (if applicable)


“Your document was rejected by [Role/Name] on [Date/Time].
 Reason: [Comment].”



🔴 Dashboard Update on the sender’s screen:


Status: Rejected


Rejection reason/comment clearly displayed.




🚨 Emergency Document Workflow for Employees

🔐 Trigger Condition: Emergency Access Enabled
Employee initiates the document submission using the “Emergency Access” toggle/button.


This bypasses regular approval chains and directly opens up access to the Emergency Authorized Recipients list.



📜 Authorized Recipients List (Emergency Access)
Employees can select one or multiple roles from the following list:
  ✅Mentors/Employees/faculty (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)
  ✅ Program Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)
 ✅HODs  (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)
 ✅ Registrar
 ✅ CDC Department Employees
 ✅ Dean
 ✅ Chairman
 ✅ Director (For Information)
 ✅ Leadership
 ✅ Controller of Examinations
 ✅ Asst. Dean IIIC
 ✅ Head Operations
 ✅ Librarian
 ✅ SSG
 ✅ Principal

🔁 Emergency Workflow Stages
📤 Submitted (by Employee)


Emergency reason and document uploaded


Recipient roles selected from the Emergency list


📨 Notifications Triggered Instantly


All selected recipients receive:


✅ Email alert


✅ Dashboard alert


✅ Message: “Urgent Document Pending – Immediate Action Required”


📝 Review (by Recipients)


View document in read-only or editable mode


Add comments if necessary


Select “Approve” ✅ or “Reject” ❌


Option to add e-signature (if configured)


📬 Approval/Rejection Response


Employee receives:


Email + dashboard status update


Timestamped response and optional comments


📦 Final Status Logged


Stored in emergency submission log with:


Signature(s) if provided


Status summary


All recipient actions & response times



🔐 Security Note:
Emergency submissions are:


✅ Timestamped


✅ Role-logged


✅ Audited in a separate “Emergency Access Logbook” for compliance





✅ Feature: Live Meet (In-Person Communication Request)
🔹 Purpose:
To allow real-time clarification or discussion before or during the approval/rejection process of Letters, Circulars, or Reports.

📌 For Employees
Employees can request or be invited to a Live Meet at any stage of the workflow with the following authorized roles:
✅ Program Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


✅HODs  (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


✅ Registrar


✅ Principal


🕒 Options Meeting Scheduler:
Date Picker


Time Slot Selector


Notes/Agenda (Optional field)


Authorized Recipients from the list below can also initiate a Live Meet request to the employee before making a final decision in Between Approved and Rejected Stages.

📌 For Principal
The Principal can also request a Live Meet at any workflow stage (for better coordination or discussion) with the following roles:
✅Mentors/Employees/faculty (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)
✅Program Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)
✅HODs  (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)

 ✅ Registrar
 ✅ CDC Department Employees
 ✅ Dean
 ✅ Chairman
 ✅ Director (For Information)
 ✅ Leadership
 ✅ Controller of Examinations
 ✅ Asst. Dean IIIC
 ✅ Head Operations
 ✅ Librarian
 ✅ SSG



💬 Live Meet Request Triggers:
✅ Optional toggle available on each approval/rejection screen


✅ Live Meet notification sent via email + dashboard alert to the other party


✅ Google Meet / Zoom link auto-generated (if integrated)



✅ Document Types Supported:
✅ Letter


✅ Circular


✅ Report


The structure and content remain consistent across all document types, whether accessed via email or through the IAOMS HITAM system.
✅ IAOMS Enhancements: Status Filters, Weekly Analytics, and Upcoming Task Management
🔖 Tag Filters / Status Views
Enable quick filtering of documents using interactive filter chips or tabbed views:
🟡 In Progress Approvals


🟠 Pending Documents


🔴 Rejected with Comments


🟢 Approved and Archived
 These tags help track document status in real time and promote clarity for all users (Employees, HODs, Principal, Registrar, all kinds of recipients Roles etc.).



📈 1. Weekly Circular Approvals Overview
Use a dynamic analytics module to track approvals based on the document's creation date:
Key Data Points:
Total circulars generated this week


Count of:


✅ Approved


🕒 Pending


❌ Rejected


Display Format:
Bar or pie charts


Role-wise breakdown 

📆 2. Upcoming Tasks for HODs and Principal
Highlight actionable items across user dashboards using an integrated task manager.
Sources:
🗓️ Meeting scheduler entries


📄 Pending approvals


⏰ Scheduled reminders


Components:
Task cards with status (To Do / In Review / Done)


Role-based assignment and filters



🗓️ Calendar Widget Integration
Embed a calendar (e.g., FullCalendar or Google Calendar API) for:
📅 Viewing upcoming meetings


📝 Scheduling events linked to documents


🔔 Auto-reminders for critical actions


Each calendar entry can link to related circulars, approvals, or uploaded documents.



✅ Universal Search Integration
Implement a global search feature that allows users to search across all modules in the IAOMS system.

🔍 Searchable Categories:
📄 Letters, Circulars, Reports


👤 User Names (Principal, Registrar, HODs, Employees, and all recipient roles)


🏢 Departments (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


📅 Events & Meetings


📂 Document Status (In Progress, Approved, Rejected)



💡 Key Features:
🔖 Tag Filters – Filter results by status, type, or role.


✨ Autocomplete Suggestions – Predictive search with dropdown results.


🛡️ Role-Based Visibility – Only show relevant results to users based on their role and permissions.


⚡ Real-Time Updates – Integrate using:


Supabase Realtime (for live search data sync)


Supabase Full-Text Search or indexing for efficient querying





🔐 Secure Authentication & Access Control
🔐 Google Sign-In via SuperBase
 – Restricted to official @hitam.org mail IDs


🪪 HITAM ID + Password Login
 – Integrated with the HITAM identity system


🔁 Role-Based Login Portals for (All branches- EEE, MECH, CSE, ECE, CSM & CSO, CSD & CSC, and Years- 1st,2nd,3rd,4th):

Employees


– HODs (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)
 
– Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)
 
– Registrar
 
– Principal Sir



Google Authentication Security:


Only HITAM.ORG mail IDs are accepted


No external email IDs are allowed to access the system for additional security






🌳 HITAM Tree Loading Animation During Login
Purpose:
 Use the official HITAM tree logo as a dynamic loader during login or system initialization.

🎨 Animation Description:
The HITAM tree gradually fills with color from white (base) to green (top).


Simulates water rising inside the tree, visually indicating loading/progress.


Optional glow or ripple effect at the base to enhance visual appeal.


Color scheme and background aligned with HITAM’s branding (white to green gradient).



🔧 Technical Implementation Notes:
Use one of the following animation methods:


✅ SVG Animation


✅ Lottie JSON animation


✅ CSS keyframes


Integrate the animation with the login/authentication logic:


Display animation only during system init or login loading.


Hide once user is authenticated and dashboard loads.







📘 Footer Design – Legal & Contact
Includes:
📎 Legal Links: Terms of Service | Privacy Policy | Cookie Policy


📍 Contact Info: HITAM Campus Address, Email, Phone, Feedback Link


🔗 Social Icons: Facebook, Instagram, YouTube, LinkedIn


© 2025, All rights reserved. Designed by SocialDNA


Feature: Distribution System for the Employee
🔁 Decentralized Permission Report Workflow
Employees can submit Reports / Letters / Circulars to:
HODs (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


Program Department Head (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


Registrar


Principal


🧭 Workflow Stages:
Submitted ➝ Reviewed ➝ Approved (opens in a separate review page with a Hand-Drawn E-Signature Canvas for Digital Signature) / Rejected ➝ Comments ➝ Final Status
🧭 Decentralized System Workflow Stages
 Employee ➝ Program Department Head  (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th) ➝ HODs(All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)➝ Registrar ➝ Principal
🗝️ Key Features:
✅ Employee can directly choose and send to a specific individual (Program Head(All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th), HODs(All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th), Registrar, or Principal) based on the required hierarchy and decentralization.


✅ Upon review, the permission report/letter/circular opens in a dedicated review page.


✅ This review page includes a Hand-Drawn E-Signature Canvas (Digital Signature).


✅ The eSignature section appears dynamically, only for the selected recipient(s) for final approval or rejection.


✅ Approval interface includes status change, comment section, and review history.



📥 Employee Portal Features:
Display of current date and time


Upload via Google Drive API


View:


Your submitted reports


All reports across users


Report statuses: ✅ Approved / ❌ Rejected / ⏳ Pending


Color-coded status display:


✅ Green – Approved


❌ Red – Rejected (with comments)


📝 Re-Submission Flow


Edit or re-upload rejected reports


Track new approval status


View previous comments for clarity


📊 Dashboard & Filters
Filter reports by:


Status (Pending / Approved / Rejected)


Department (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


Reviewer Role (HODs(All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th), Program Head (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th), Registrar, Principal)


Search by:


Employee name, ID, Time, Date, or Report title

🧭 Decentralized System Workflow Stages
Employee ➝ Program Department Head  (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)➝ HODs (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th) ➝ Registrar ➝ Principal

The employee has the flexibility to define their own workflow by selecting specific individuals based on the requirement.
The employee can directly choose and send the Permission Report/Letter/Circular to any of the following roles:
✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


✅ HODs (All Branches-EEE, MECH, CSE, ECE, CSM, CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


Registrar


Principal


This decentralized system allows customized routing of requests according to organizational hierarchy or specific needs.

Decentralized Permission Report Workflow
Employees can send Permission Reports, Letters, or Circulars to any of the following, with decentralized role-based options:
Program Head (across all branches)


HOD (across all branches)


Registrar


Principal
Workflow Stages:
Submitted ➝ Reviewed ➝ Approved (opens in a separate review page with a Hand-Drawn E-Signature Canvas for Digital Signature) / Rejected ➝ Comments ➝ Final Status
Key Features:
Users can directly choose and send to a specific individual (Program Head, HOD, Registrar, or Principal) based on the required hierarchy and decentralization.


Upon review, the permission report/letter/circular opens in a separate review page with a Hand-Drawn E-Signature Canvas (Digital Signature).


The signature section is dynamically shown only to the selected recipient(s) for final approval or rejection.
🧭 Decentralized System Workflow Stages
 Employee ➝ Program Department Head  (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th) ➝ HODs(All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)➝ Registrar ➝ Principal
The employee has the flexibility to define their own workflow by selecting specific individuals based on the requirement.


The employee can directly choose and send the Permission Report/Letter/Circular to any of the following roles:


Program Head (All Branches)


HOD (All Branches)


Registrar


Principal


This decentralized system allows customized routing of requests according to organizational hierarchy or specific needs.

Document Options:
Users can select from: Letters, Circulars, or Reports



Workflow Stages:
Submitted ➝ Reviewed ➝
 Approved (clicking the “Approve” button turns it green, opens a separate review page with a Hand-Drawn E-Signature Canvas for Digital Signature, shows Date, Time, and optional Comments)
 / Rejected (clicking the “Reject” button turns it red, shows Comments bar) ➝ Final Status

Decentralized System Workflow:
Employee ➝ Program Department Head(All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)➝ HODs (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)➝ Registrar ➝ Principal
The employee can define their own approval flow by selecting specific individuals.


The workflow dynamically adapts based on the selected approvers.



Dynamic Error Handling:
If a selected person is unavailable, the system will:


Show a message on the signature bar: "Person not available at the time"


Send automatic email and website alerts to:


The unavailable person


The employee


Does not break or disconnect the workflow—only informs and logs the unavailability.


Alerts include:


Website pop-up message


Email alert at the beginning of the process



Signature & Review Features:
Upon review, the Letter / Circular / Report opens in a separate review page with:


Hand-Drawn E-Signature Canvas (Digital Signature)


Option to scan a signature using a camera (photo upload)


Option to save scanned signature for future use


Signature bar shows Date and Time, dynamically displayed only for selected recipients


The system allows dynamic resizing of the signature area—users can increase or decrease signature box size as needed.
Final Approval Interface:
Approved:


Green bar appears with Date, Time, and optional Comments


Signature applied and logged


Rejected:


Red bar appears with rejection reason in Comments


Email and system notifications sent to the employee and relevant reviewers


Final status reflects all actions taken by:
 Program Department Head ➝ HOD ➝ Registrar ➝ Principal







🚨 Emergency Document Workflow for Employees

🔐 Trigger Condition: Emergency Access Enabled
Employee initiates the document submission using the “Emergency Access” toggle/button.


This bypasses regular approval chains and directly opens up access to the Emergency Authorized Recipients list.



📜 Authorized Recipients List (Emergency Access)
Employees can select one or multiple roles from the following list:
✅Mentors/Employees/faculty (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)
✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)
✅ HODs (All Branches-EEE, MECH, CSE, ECE, CSM, CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)
 ✅ Registrar
 ✅ CDC Department Employees
 ✅ Dean
 ✅ Chairman
 ✅ Director (For Information)
 ✅ Leadership
 ✅ Controller of Examinations
 ✅ Asst. Dean IIIC
 ✅ Head Operations
 ✅ Librarian
 ✅ SSG


 ✅ Principal

🔁 Emergency Workflow Stages
📤 Submitted (by Employee)


Emergency reason and document uploaded


Recipient roles selected from the Emergency list


📨 Notifications Triggered Instantly


All selected recipients receive:


✅ Email alert


✅ Dashboard alert


✅ Message: “Urgent Document Pending – Immediate Action Required”


📝 Review (by Recipients)


View document in read-only or editable mode


Add comments if necessary


Select “Approve” ✅ or “Reject” ❌


Option to add e-signature (if configured)


📬 Approval/Rejection Response


Employee receives:


Email + dashboard status update


Timestamped response and optional comments


📦 Final Status Logged


Stored in emergency submission log with:


Signature(s) if provided


Status summary


All recipient actions & response times



🔐 Security Note:
Emergency submissions are:


✅ Timestamped


✅ Role-logged


✅ Audited in a separate “Emergency Access Logbook” for compliance



🧭 Decentralized System Workflow Stages
Employee ➝ ✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)➝✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)➝ Registrar ➝ Principal

The employee has the flexibility to define their own workflow by selecting specific individuals based on the requirement.
The employee can directly choose and send the Permission Report/Letter/Circular to any of the following roles:
✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


HODs (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


Registrar


Principal


This decentralized system allows customized routing of requests according to organizational hierarchy or specific needs.

Decentralized Permission Report Workflow
Employees can send Permission Reports, Letters, or Circulars to any of the following, with decentralized role-based options:
Program Head (across all branches)


HOD (across all branches)


Registrar


Principal
Workflow Stages:
Submitted ➝ Reviewed ➝ Approved (opens in a separate review page with a Hand-Drawn E-Signature Canvas for Digital Signature) / Rejected ➝ Comments ➝ Final Status
Key Features:
Users can directly choose and send to a specific individual (Program Head, HOD, Registrar, or Principal) based on the required hierarchy and decentralization.


Upon review, the permission report/letter/circular opens in a separate review page with a Hand-Drawn E-Signature Canvas (Digital Signature).


The signature section is dynamically shown only to the selected recipient(s) for final approval or rejection.
Workflow Stages:
 Employee ➝ Program Department Head  (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th) ➝ HODs  (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)➝ Registrar ➝ Principal
The employee has the flexibility to define their own workflow by selecting specific individuals based on the requirement.


The employee can directly choose and send the Permission Report/Letter/Circular to any of the following roles:


✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)



HODs (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


Registrar


Principal


This decentralized system allows customized routing of requests according to organizational hierarchy or specific needs.


Feature: Distribution System for the Principal
The Principal has advanced options to share/send Letters, Circulars, or Reports, with the ability to:

1. Mass Distribution Option (All-in-One Click):
The Principal can send a document to all the following roles at once:


 List of Authorized Signatories (Recipients)
This feature supports sending and collecting signatures from the following roles:
Mentors/Employees/faculty (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


Program Heads (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


HODs (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


Registrar


CDC Department Employees


Dean


Chairman


Director (for information)


Leadership


Controller of Examinations


Asst. Dean IIIC


Head Operations


Librarian


SSG





All recipients receive the document simultaneously and are required to:


Review and sign using the Hand-Drawn E-Signature Canvas (Digital Signature)


Alternatively, use the "Scan Signature using Camera" (photo upload option)


Signature bars will display dynamically for each selected recipient, with Date and Time stamps included



2. Decentralized Direct Send Option (To Selected Individual Only):
The Principal can also selectively send a document only to specific individual(s) using a decentralized option:


Choose any one or more from:


Mentors/Employees/faculty (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


Program Heads (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


HODs (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


Registrar


CDC Department Employees


Dean


Chairman
Director (for information)


Leadership


Controller of Examinations


Asst. Dean IIIC


Head Operations


Librarian


SSG


Based on the selected individual(s), the signature bar will be shown only to them.



Approval Workflow for Shared Documents:
Submitted ➝ Reviewed ➝
 Approved (opens a separate review page with Hand-Drawn E-Signature Canvas / Scan Signature using Camera)
 / Rejected ➝ Comments Bar ➝ Final Status
The signature section appears only to the chosen recipients.


Each action (approval/rejection) is time-stamped with Date and Time.


Approved signatures display a green bar, rejected ones display a red bar, with comments required in both cases.




✅ Feature: Document Distribution System for the Principal
The Principal can share or send Letters, Circulars, or Reports, with the ability to:

🔹 1. One-Click Mass Distribution and Signature Collection
The Principal can send the document to all relevant individuals in a single click.


Recipients will be able to review and sign using:


✍️ Hand-Drawn E-Signature Canvas (Digital Signature)


📷 Scan Signature Using a Camera (Photo Upload)



🔹 2. List of Authorized Signatories (Recipients)
This feature supports sending and collecting signatures from the following roles:
Mentors/Employees/faculty (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)



Program Heads (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


HODs (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


Registrar


CDC Department Employees


Dean


Chairman


Director (for information)


Leadership


Controller of Examinations


Asst. Dean IIIC


Head Operations


Librarian


SSG






🔹 3. Decentralized Direct Send Option
The Principal can also choose to send directly to specific individual(s) instead of all at once.


This customized distribution supports decentralized workflows where documents are only sent to the necessary reviewers.



🔹 4. Signature Handling Workflow
Submitted ➝ Reviewed ➝ Signature ➝ Final Status


When the document is reviewed, it opens in a dedicated E-signature review page.


The page includes a Hand-Drawn Signature Canvas


Option to upload a scanned signature via camera


The signature bar is shown only to the selected person


Includes Date and Time stamp, and optional Comment box


This system ensures:
✅ Fast, large-scale document distribution


✅ Role-based signature access


✅ Decentralized, custom-targeted sending


✅ Fully digital and secure signature collection




📤 Document Upload System Requirements
✅ Supported Document Types:
Letter


Circular


Report


Images (for scanned or photographed documents)


✅ Accepted File Formats:
.pdf, .doc, .docx, .xlsx, .xls, .png, .jpg, .jpeg
✅ Storage:
All uploaded documents are automatically stored in Google Drive.
📱 Smart Upload Behavior (Mobile Camera or Manual Upload)
If the document is scanned using a mobile phone camera (e.g., image or photo of a document):


The system will automatically convert the scanned file (if it's a letter, circular, or report) into a Google Docs file using OCR (Optical Character Recognition).


The content is cleaned and formatted into a professional Google Docs layout.


Space for signatures Box, date, time, and comments is dynamically added inline based on selected recipient roles.


If the uploaded document is already professionally scanned (e.g., high-resolution PDF or original Word file):


The file will not be converted.


It is preserved in its original format to maintain professional formatting and layout fidelity.
⚙️ Inline Enhancements (After Conversion to Google Docs)
Add signature placeholders dynamically for:


✍️ Digital hand-drawn signature


📷 Scanned signature (via photo upload)


🕒 Timestamp and role-based labels Such as Time, Date


💬 Comment sections per signer


Upload options (attachments, images, spreadsheets) embedded in-line if needed.

🖨️ User Download Options After Processing:
Once the document is generated or updated:
✅ Download as .pdf (print-ready)


✅ Download as .docx (Microsoft Word)


✅ Download as .txt (plain text version)


✅ Download as .html (if needed for embedding in web portal)


✅ Keep as .gdoc for future edits in Google Docs


📝 Note: Each format retains the embedded signatures Box, comments, and timestamps for final versions.

🔁 Automatic Role-Based Routing After Upload
Once a document (Letter, Circular, or Report) is uploaded by an Employee or the Principal:
📍 The system automatically detects the document type and matches it to the correct workflow.


🧭 Based on pre-defined logic, the system routes the document to the appropriate authorized recipients (e.g., HODs, Registrar, Principal) according to their role.


📨 Email + Dashboard notifications are triggered instantly to all selected roles for review, comment, and approval/rejection.
🔒 Role Access Control:
This feature is restricted to authenticated Employees and the Principal only.


Access is verified using Google HITAM Mail ID login and SuperBase Authentication.

Provide an option to scan a signature using the device camera (photo upload) and automatically place the scanned signature onto Letters, Circulars, or Reports.
Also include an option to save the scanned signature for future use across documents.
💾 Save Scanned Signature for Future Use
When a signatory uploads a scanned signature via the camera/photo:


Provide an option: “✅ Save this signature for future documents”


Save it securely for reuse with edit/delete options
✍️ Signature Input Options:
Each person will have 3 input options:
Hand-Drawn Signature Canvas


On touch screen or with mouse


Scan & Upload via Camera


Snap a photo of their physical signature


Reuse Saved Signature


From previous signed documents (if stored securely)


✅ Signature Overlay Includes:
✍️ Hand-Drawn Signature Canvas
 Allows users to draw their signature directly on the screen.


📷 Scan Signature Using Device Camera (Image Upload)
 Upload a scanned image of a handwritten signature using the device camera or file picker.


💾 Save Signature for Future Use
 Option to securely store the signature for reuse in future approvals.


📅 Auto Date & Time Stamp
 Automatically records the exact date and time when the signature is applied.


🗒️ Optional Comment Field
 Signers can add relevant notes or feedback alongside their signature.


📂 Optional Document Upload by Roles (If Required)
 Roles such as HODs, Registrar, or Principal can upload supporting documents during the signing process.

🔔 Notifications
Automated alerts using Gmail API on:


Document Submission


Approval/Rejection


Comments added


Document Options:
Users can select from: Letters, Circulars, or Reports



Workflow Stages:
Submitted ➝ Reviewed ➝
 Approved (clicking the “Approve” button turns it green, opens a separate review page with a Hand-Drawn E-Signature Canvas for Digital Signature, shows Date, Time, and optional Comments)
 / Rejected (clicking the “Reject” button turns it red, shows Comments bar) ➝ Final Status

Decentralized System Workflow:
Employee ➝ ✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)➝ HODs (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)➝ Registrar ➝ Principal
The employee can define their own approval flow by selecting specific individuals.


The workflow dynamically adapts based on the selected approvers.



Dynamic Error Handling:
If a selected person is unavailable, the system will:


Show a message on the signature bar: "Person not available at the time"


Send automatic email and website alerts to:


The unavailable person


The employee


Does not break or disconnect the workflow—only informs and logs the unavailability.


Alerts include:


Website pop-up message


Email alert at the beginning of the process



Signature & Review Features:
Upon review, the Letter / Circular / Report opens in a separate review page with:


Hand-Drawn E-Signature Canvas (Digital Signature)


Option to scan a signature using a camera (photo upload)


Option to save scanned signature for future use


Signature bar shows Date and Time, dynamically displayed only for selected recipients


The system allows dynamic resizing of the signature area—users can increase or decrease signature box size as needed.





Secure Signature Handling – Enhanced Signing Options
To ensure both security and professionalism, the system supports the following features for Letters, Circulars, or Reports:
Signature Capture Options (Secure Review Page):
✅ A dedicated and secure review page is provided for authorized recipients to sign documents using:


Hand-Drawn E-Signature Canvas


Scan Signature via Camera (photo upload option)

Provide an option to scan a signature using the device camera (photo upload) and automatically place the scanned signature onto Letters, Circulars, or Reports.
Also include an option to save the scanned signature for future use across documents.


Signature Metadata and Visibility:
Signature bars include:


✅ Date and Time Stamps


✅ Optional Comments


✅ Role-based access and visibility to ensure proper authorization



🔍 AI-Powered Document Insight & Smart Summary
Integrate Google Gemini API to:


Auto-summarize uploaded circulars, reports, or letters.


Generate “TL;DR” (Too Long; Didn’t Read) sections in bullet format.


Helps staff and students quickly grasp key insights without reading full content.


🗃️ Old Document Upload for Archiving & AI Enhancement
Enable users to upload older Letters, Circulars, and Reports into the system for the following purposes:

✅ Use Cases:
🔁 Future Referencing:


Easily retrieve historical documents during reviews or audits.


Enable full-text search through titles, content, and roles.


📂 Digital Archiving:


Categorize uploads by type (Letter/Circular/Report), department, year, and tags.


Store them securely in Google Drive, linked to Firebase for quick access.


🧠 AI-Powered Refinement (Google Docs + Gemini):


Automatically convert old scanned or typed documents into formatted Google Docs.


AI refines the structure using a standard college-style template (header, logo, signature block, etc.).


The system learns from uploaded formats and improves future document generation quality.


✅ The system intelligently learns from the structure and layout of previously uploaded documents to enhance and auto-improve the quality, formatting, and consistency of future document generation.


🤖 How the System Learns & Improves Document Generation
As more Letters, Circulars, and Reports are uploaded into the system, it applies a combination of machine learning techniques and AI-assisted document processing using tools like Google Gemini, Google Docs API, or custom NLP logic to:

1. 🧠 Format Recognition & Pattern Extraction
The system scans uploaded documents (PDF, Word, or converted Google Docs).


It extracts structural elements like:


Title formats (e.g., “NOTICE” in all caps)


Signature block positions


Role hierarchies


Common headings/subheadings (e.g., “Subject,” “Date,” “From,” “To”)



2. 📊 Statistical Learning from Usage Trends
It tracks:


How many documents share similar layouts


Which departments use which template types


Common phrases, formats, and section orderings


Builds a template probability model based on recurring formats



3. ✨ AI-Supported Refinement Using Gemini API
Gemini suggests:


Auto-corrected and well-aligned structure


More professional formatting


Inline signature space placement logic


It generates recommended Google Docs templates matching learned structure



4. 🧩 Template Matching & Smart Suggestions
When a new document is uploaded, the system:


Checks the content layout


Matches it against learned templates


Suggests or auto-applies the closest-matching structure


Signatures and role spaces are dynamically placed with adequate space based on previous usage



5. 📚 Institution-Specific Smart Template Library
Over time, the system builds a library of smart templates unique to HITAM’s usage:


Academic letters


Faculty circulars


Event notices


Each template evolves as more data is processed, creating a self-improving ecosystem


📤 Old Document Upload for Archiving & AI Enhancement
Provide users with the ability to upload older Letters, Circulars, and Reports to the system for:


🔁 Future referencing


📂 Archiving


🧠 Google Docs refinement with AI formatting



📝 Google Docs Integration:
Automatically structure uploaded documents in Google Docs with:


✅ Signature bar spaces per assigned roles


✅ Adjusted layout based on official templates


✅ AI-powered formatting (via Google Gemini API)

🤖 AI-Powered Future Enhancements
🧠 Grammar Correction using Google Gemini + Google API before report submission


🧾 AI-Powered Summary of report for reviewer preview


📊 Activity analytics dashboard for management



Predefined Templates with Smart Suggestions:


Integrated with Google API to suggest:


Most-used predefined templates


Structured and professional content for Letters, Circulars, and Reports


The same structured content is reflected in emails automatically.


Employees and the Principal can customize the template and adjust signature space inline, or let it open in a separate review page.
✍️ Form Auto-Fill & Smart Suggestions
When creating a document:


Auto-fill user name, department, and timestamp based on login.


Suggest previously used titles, document types, templates.


AI suggests roles to route the document to — based on keywords.

📬 Notifications & Email Alerts
🔔 Website Notifications
Real-time status updates on:


Report submission


Approval/Rejection


Reviewer comments
Automated Notifications for Principal’s Document Distribution
When the Employee, Principal and all kinds of Recipient send Letters, Circulars, or Reports, the system will automatically send email alerts and notifications to the selected recipients.

"Add email and notification alert options with customizable scheduling—for example, send alerts every 1 minute, every 15 minutes, or at specific intervals set by the user. Include the ability to configure alert frequency for different types of actions such as:
Document submission


Approval status updates


Rejection with comments


Reminder alerts for pending actions


Escalation alerts


Allow role-based customization for notification intervals (e.g., Principal receives summaries every 15 minutes, while Employees receive immediate alerts)."



📧 Email Notifications (via SuperBase Functions + SendGrid + Gmail API (Google Mail)
With AI-enhanced content using Google Gemini + Google API key:
Email Content Example:
Subject: [Permission Report] Status Update - IAOMS HITAM

Dear [Employee Name],

Your submitted report titled **"[Report Title]"** has been **[Approved/Rejected]** by [Reviewer Name & Role].

Comments (if any): "[Comment]"

Track your report here: [View Link]

Regards,  
IAOMS Automated System




Email Integration:
Using Google API Key, the system will:


Auto-generate email content based on:


The selected document type (Letter/Circular/Report)


The recipient’s role and (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)



The approval status (including unavailable persons)


Send emails with:


Direct view and sign link


Download option for the signed file


Employees can also view the file on the website (as secondary preference)


Automated Notifications for Principal’s Document Distribution
When the Employee and Principal sends Letters, Circulars, or Reports, the system will automatically send email alerts and notifications to the selected recipients.

✅ Document Types Supported:
✅ Letter


✅ Circular


✅ Report


The structure and content remain consistent across all document types, whether accessed via email or through the IAOMS HITAM system.

📧 Email Template
Subject: [IAOMS] Permission Report Update
Body:
Dear [Recipient Name],

Your document titled **“[Document Title]”** has been **[Approved / Rejected]** by **[Reviewer Name]**.

📝 **Comments (if any):**  
“[Optional Reviewer Comment]”

📂 **Access your document here:**  
[Secure View Link – Opens a  document With secure signature view with download option]  

🔗 Alternatively, you can view or resubmit the document via the IAOMS HITAM portal:  
[Website Link to Approved Letters, Circulars, or Reports with Signature]

Best regards,  
IAOMS HITAM System


🔒 Security & Accessibility
📥 Direct Access Without Login
 The secure email link:


✅ Opens a dedicated preview page (Canva-style layout)


✅ Displays the document along with visible signatures


✅ Allows direct download for physical or digital use


🌐 Web Portal Integration
 Documents are automatically archived in the IAOMS HITAM system for:


✅ Easy retrieval by document type (Letter, Circular, Report)


✅ Search and filter functionality
✅ Download history with approval metadata


✅ Email Notification Policy Using HITAM Credentials
Use Case:
 All system-generated notifications — including approvals, rejections, submissions, and workflow updates — must use the user’s official HITAM ID email, authenticated during login/signup.
Implementation Details:
Upon Google OAuth login using the HITAM email (e.g., @hitam.org), the system captures and verifies the user’s email address.


All outgoing notifications are sent from or on behalf of the same authenticated HITAM email ID.


This ensures:


✅ Verified sender identity


✅ Secure communication


✅ Traceability and audit-readiness for academic and administrative workflows


Example Notification Headers:
From: hod.cse@hitam.org
To: registrar@hitam.org, principal@hitam.org
Subject: [IAOMS] Circular Approval Request from HOD-CSE
Approved Comment Signature With Date and Time along with Email

⏫ Auto-Escalation & Reminder Rules
Set rules to auto-escalate documents if pending for more than X days:


Escalate to the next authority


Send periodic reminder emails or hard alerts


⚠️ Avoids delays in critical workflows.


Email Integration:
Using Google API Key, the system will:


Auto-generate email content based on:


The selected document type (Letter/Circular/Report)


The recipient’s role and branch/year


The approval status (including unavailable persons)


Send emails with:


Direct view and sign link


Download option for the signed file


Employees can also view the file on the website (as a secondary preference)




✅ Special Feature – Direct Notification During Meetings
Enable real-time, high-priority alerts to the Principal even during ongoing meetings to ensure urgent matters are not delayed.

🧑‍💼 Meeting Participants (Role-Based):
✅HODs (All branches-EEE, MECH, CSE, ECE, CSM, CSO, CSD ,CS,C and Years- 1st,2nd,3rd,4th)


✅ Program Heads (All branches-EEE, MECH, CSE, ECE, CSM, CSO, CSD , CSC, and Years- 1st,2nd,3rd,4th)


✅ Registrar


✅ Principal



🔔 Real-Time “Notify Principal” Option:
If any of the above roles (especially the Principal) are currently marked as “In a Meeting”, employees will see a “Notify Principal” button.


This feature allows them to:


🚨 Send urgent document-related alerts


📌 Include summary, file attachment, and reason


⏱️ Push an instant notification to the Principal via:


Dashboard popup


Email


Optional SMS alert (if enabled)



🔐 This Is Important:
Prevents delay in time-sensitive proposals


Ensures decision-makers remain informed, even when occupied


Adds a priority escalation channel without interrupting ongoing workflows



⏫ Auto-Escalation & Reminder Rules
Set rules to auto-escalate documents if pending for more than X days:


Escalate to the next authority


Send periodic reminder emails or hard alerts


⚠️ Avoids delays in critical workflows.

"Add email and notification alert options with customizable scheduling—for example, send alerts every 1 minute, every 15 minutes, or at specific intervals set by the user. Include the ability to configure alert frequency for different types of actions such as:
Document submission


Approval status updates


Rejection with comments


Reminder alerts for pending actions


Escalation alerts


Allow role-based customization for notification intervals (e.g., Principal receives summaries every 15 minutes, while Employees receive immediate alerts)."


OPTIONAL FOR USERS TO SELECT THIS OPTION                                                                   🔁 Bi-Directional Approval Routing
Purpose:
 To introduce flexible, dynamic, and hierarchical document approval workflows that adapt based on action outcomes (approval or rejection), reducing bottlenecks and enhancing accountability.

✅ Core Features:
Counter-Approval Workflow


After one authority approves, another can re-validate or counter-approve to ensure dual-verification.


(Example:


Principal ➝ Registrar


The Principal approves a circular, and it automatically goes to the Registrar for secondary confirmation.)


Conditional Escalation on Rejection


If a document is rejected at any stage, it is automatically escalated to a higher authority for review instead of terminating the workflow.


(Example:


HOD rejects a proposal ➝ The system routes it to the Director for a final decision.)


Role-Based Rules & Triggers


Routing logic is based on:


Role hierarchy (e.g., HOD → Director → Principal)


Document type (e.g., Academic vs Administrative)


Status (Approved, Rejected, Pending too long)


Supports dynamic fallback paths for various branches and departments.


Notification System Integration


All routed actions trigger:


📩 Email alerts to next approvers or escalation roles.


🔔 Dashboard notifications with context and history.


Comment Trail & Audit Logs


Each action (Approve/Reject/Escalate) logs:


Role


Timestamp


Comments (if any)


Routing history


🛠 Features Supported:
🔄 Automatic re-routing if the current approver rejects or delays action


📬 Email + dashboard alerts sent at every approval or routing transition


⚙️ Admin can configure routing logic 
✅ Outcome: Prevents Dead Ends & Supports Escalation Logic
By implementing bi-directional approval routing, auto-escalation rules, and dynamic workflow paths, the system ensures that:
⚠️ No document gets stuck due to inaction or rejection.


🔁 Rejected items are automatically forwarded to higher roles (e.g., Director or Principal).


⏰ Delayed approvals trigger reminders or escalate to the next authorized person.


🧭 Routing adapts based on approval/rejection conditions — ensuring continuous flow.


📌 Result: A seamless, fail-safe approval system that maintains momentum, reduces communication lags, and prevents bottlenecks in institutional workflows.
OPTIONAL FOR USERS TO SELECT                                                                    🔁 Bi-Directional Approval Routing
Enable flexible, hierarchical routing workflows:


Example 1: Principal ➝ Registrar (counter-approval)


Example 2: HOD rejects ➝ auto-forward to Director for final review


Prevents bottlenecks and ensures fallback or escalation paths.


✅ Decentralized Chat 
🔁 Chat Sessions & Decentralized Communication:
Enable secure and decentralized chat sessions between selected roles for collaborative discussion:
✅ HODs (All Branches-EEE, MECH, CSE, ECE, CSM, CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


✅ Registrar


✅ Principal
Mentors/Employees/faculty (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)

💬 Chat Sessions & Decentralized Communication System
🧩 Core Features
1. 🔐 Role-Based Group & Private Chat
Auto-create chat groups based on roles:


e.g., All HODs, Registrar + Dean, CSE Department Only, etc.


Support 1-on-1 chats (Employee ↔ Registrar).



2. 🧾 Attach Documents and Media
Upload PDFs, Excel, Docs, Images, etc.


Auto-preview feature (especially for circulars or letters).


Link integration with Google Drive or Docs.



3. 🛠️ Decentralized Threads (Topic-Based Conversations)
Each document/circular/report creates a dedicated discussion thread.


Roles involved can comment, suggest edits, or clarify — without affecting other conversations.




🚀 Advanced Features for IAOMS – HITAM
💬 Role-Based Chat Channels (Slack-like)
Create dedicated chatrooms for roles such as:


✅ HODs (All Branches-EEE, MECH, CSE, ECE, CSM, CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)
✅Mentors/Employees/faculty (All branches-EEE, MECH, CSE, ECE, CSM, CSO, CSD, CS,C and Years- 1st,2nd,3rd,4th)


✅ Registrar


✅ Principal


✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)

Allow role-restricted conversations, file sharing, and updates in real time.


Archive chat history per document or discussion thread.

📦 Document Collaboration & Workflow Chat
 🗃️ Document-Centric Chat Rooms
Each Letter, Circular, or Report has its own chat room.


Track discussions, edits, and approval updates in context.



12. 📊 Live Chat Status Badge
Show document approval status inside chat:


🟢 Approved


🔴 Rejected


🟡 Awaiting Review


Auto-update based on workflow.



🛡️ Security & Decentralization Features
13. 🔐 End-to-End Encryption
Secure communication between all users.


No access by system admins to private chats.



14. 🧭 Decentralized Hosting Option (Optional)
Use Superbase or P2P architecture for decentralized communication (if going beyond institutional setup).



15. 🧾 Message Receipt Logs & Accountability
Track if a recipient has:


✅ Read


🕒 Skipped


⛔ Ignored


Useful for accountability in official workflows.





✅ Access to Share Documents Within Chat Sessions
Supported Sources & File Types for Sharing:
📁 Google Drive
 📊 Google Sheets / Microsoft Excel
 📄 Google Docs
 📷Images 
 📂 Local Device Uploads
Supported File Formats:
 .pdf, .doc, .docx, .xlsx, .xls, .png, .jpg, .jpeg
Chat Support (Internal Helpbot)
Let users ask things like:


“Where’s my last approved circular?”


“Who signed my report?”


AI bot responds with direct links or filters

🔄 New & Advanced Features to Add
✅ Smart Features
🧠 AI-Based Auto-Summarizer
Auto-generate chat summaries using Google Gemini API.


Show TL;DR of long chats and key decisions made.


 🔔 Smart Notification Engine
Real-time dashboard + email + mobile push notifications:


When a user is tagged


When their document is approved/rejected


When a decision is made in a group chat


 📥 Offline Mode with Catch-Up Sync
Allow users to view messages offline and sync replies later (for mobile app).


Useful in areas with poor connectivity.


📎 Inline Signature Requests from Chat
Within chat threads, users can be tagged to sign a document.


“@HOD-CSE please review and sign this letter” → triggers a signature canvas inline.


             📆 Live Chat Reminders & Action Flags
Mark messages as:


✅ Approved


❌ Rejected


🕒 Pending Review


Assign tasks or flag messages for follow-up.


🔁 Audit Trail of Chat for Approvals
All chats related to official documents are logged for future audits.


Exportable chat history per document, with timestamps and role tags.


💬 Live Chat & Prompt Assist
Add real-time communication support with:
Live chat channels per role or department


AI-powered prompts to suggest next steps


Integrated message + document sharing


Tag Filters (In Progress, Pending, Rejected, Approved)


Weekly Circular Approvals overview


Upcoming Tasks with Calendar Integration

🔁 Google Calendar, Microsoft Teams & Zoom Integration
✅ One-Click Scheduling:
Schedule meetings using IAOMS interface or via calendar API integrations


Automatically sync with:


📅 Google Calendar


💼 Microsoft Teams
Google Meet


📹 Zoom


✅ Smart Calendar Attachments:
Attach auto-generated IAOMS documents like:


Circulars


Agendas


Proposals


These are accessible directly from the calendar invite


✅ Multi-Channel Notifications:
Auto-email alerts to all invitees


Teams notifications (if enabled)



✅ Automatic Linking & Tracing:
Meeting entry links back to:


All attached files


MoM notes


Chat discussions (if decentralized module enabled)


📅 Meeting Scheduling & Management System
Feature Overview:
Enable a built-in system for scheduling, conducting, and managing meetings by authorized users:
🧑‍💼 Roles Authorized to Schedule/Conduct Meetings:
✅ Principal
✅Employees


✅ HODs (All Branches-EEE, MECH, CSE, ECE, CSM, CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)
✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)
✅ Registrar
🕒 Meeting Scheduler Options (UI Design Requirements):
Provide an intuitive interface for scheduling meetings with the following elements:

✅ 1. Date Picker
Allows users to select a specific meeting date using a calendar interface.


✅ 2. Time Slot Selector
Users can choose available time slots from a dropdown or slider (e.g., 10:00 AM – 11:00 AM).


Optional integration with calendar APIs to avoid clashes.


✅ 3. Notes / Agenda (Optional Field)
A text input area where the meeting initiator can specify the purpose, discussion points, or any additional notes.
✅ Core Capabilities:
Schedule Meetings:


Set meeting title, agenda, participants, date & time, and location (physical or online).


Attach relevant documents (letters, circulars, reports) during scheduling.


Auto-generate and send email/calendar invites to all selected roles.


Meeting Notifications:


Instant email + dashboard alerts to invited members.


Real-time reminders (e.g., 15 mins before) with join links for online meetings.


Meeting Participation Status:


Track RSVP: ✅ Accepted / ❌ Declined / ❓ Pending.


Participants can mark “I’m in a Meeting” to update status system-wide.
ESSENTIAL FEATURES TO ADD
🔄 Recurring Meetings Support
Allow organizers to schedule weekly/monthly recurring meetings (e.g., staff meetings every Monday).


Options: Daily, Weekly, Monthly, Custom.
📍 Location & Meeting Type
Options:


Physical Room (with building/room no.)


Online (Zoom/Meet link)


Hybrid
 👥 Participant Role-Based Selection
Allow organizers to invite based on predefined roles or groups, such as:


✅ HODs (All Branches-EEE, MECH, CSE, ECE, CSM, CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


Specific✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


Registrar & Dean


Custom role selection
. ✅ Approval Workflow Before Finalizing
Add an approval option for high-level meetings (e.g., Principal or Registrar must approve before sending invites).
🧠 AI-Based Scheduling Suggestion (Gemini API / Google AI)
Suggest optimal times based on:


Participants' availability


Avoiding class timings / other events


Historical meeting patterns


🚨 INTELLIGENT FEATURES
7. 🔔 Smart Reminders & Notifications
Send automatic email and dashboard notifications:


24 hrs, 1 hr, and 10 mins before the meeting.


After the meeting ends (summary/minutes if available).


🗓️ Meeting Scheduling System (for Organizers)
Requirement:
Meeting organizers must be able to:
✅ Fix specific dates and time slots for meetings or events.
✅ Automatically block those dates on the Decentralized and centralized event/activity calendar to avoid scheduling conflicts.

✅ Features:
Central Calendar Integration


All scheduled meetings/events are synced to a shared calendar (e.g., Google Calendar, Firebase Calendar DB).


Dates marked as "Busy" for the organizer and invited roles.


Conflict Detection


The system should prevent overlapping meetings by checking existing entries.


Role-Based Organizer Access


Authorized roles Recipients can block calendar slots.


Automatic Notifications


Once the date is fixed, emails and dashboard alerts are sent to all invitees.




✅ ESSENTIAL FEATURES TO ADD
1. 🔄 Recurring Meetings Support
Allow organizers to schedule weekly/monthly recurring meetings (e.g., staff meetings every Monday).


Options: Daily, Weekly, Monthly, Custom.



2. 📋 Meeting Agenda & Documents Upload
Upload documents (PDF, Excel, Word, etc.) directly when scheduling.


Attach the agenda, circulars, reports, or presentations in advance.



3. 👥 Participant Role-Based Selection
Allow organizers to invite based on predefined roles or groups, such as:


✅ HODs (All Branches-EEE, MECH, CSE, ECE, CSM, CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


Specific ✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


Registrar & Dean


Custom role selection



4. 🖼️ Meeting Cover Page or Circular View
Auto-generate a meeting letter/circular format with:


Date, Time, Location


Attendees


Signature space for approvals (if required)


Exportable as Google Doc or PDF



5. 📍 Location & Meeting Type
Options:


Physical Room (with building/room no.)


Online (Zoom/Meet link)


Hybrid



6. 🔁 Follow-up Actions & Attendance Tracker
Option to log minutes of meeting (MoM) post-event.


Track attendance manually or auto-record login-based attendance.


Provide space for decisions taken, action items, and remarks.



🚨 INTELLIGENT FEATURES
7. 🔔 Smart Reminders & Notifications
Send automatic email and dashboard notifications:


24 hrs, 1 hr, and 10 mins before the meeting.


After the meeting ends (summary/minutes if available).



8. 🧠 AI-Based Scheduling Suggestion (Gemini API / Google AI)
Suggest optimal times based on:


Participants' availability


Avoiding class timings / other events


Historical meeting patterns



9. 📊 Meeting Analytics Dashboard
View logs of all meetings:


Who scheduled, when, how many attended, meeting duration, approval status.



10. ✅ Approval Workflow Before Finalizing
Add an approval option for high-level meetings (e.g., Principal or Registrar must approve before sending invites).



🧩 ADVANCED INTEGRATIONS
11. 📅 Sync with Google Calendar / Outlook
Allow meetings to auto-sync with external calendars via OAuth.



12. 🎥 Auto-Generated Meeting Recording Upload (Optional)
Link recordings (Meet/Zoom) and upload to Google Drive with shared access to attendees.



13. 🧾 Downloadable Summary Report
Generate a PDF summary for:


Meeting details


Attendees


Agenda


Action points


Next meeting date



📅 Advanced Integrations for Meeting Scheduling System
✅ Google Calendar Sync With Google Calendar API integration
Automatically sync scheduled meetings with Google Calendar for all participants.


Real-time updates and reminders via Google Calendar notifications.


Supports time zone management and recurring meeting options.


✅ Advance Date Blocking
Organizers (Principal, Registrar, HODs, Program Heads) can pre-block specific dates to avoid scheduling conflicts.


Blocked dates are reflected across all users’ dashboards and calendars.


Includes support for exam periods, holidays, academic events, and blackout dates.


✅ Smart Suggestions
Based on availability and blocked dates, the system can suggest optimal meeting times.

📆 Integrated Activity Calendar (Role-Based Filters)
Unified calendar view for:


📅 Academic Events


🧑‍🏫 Department Activities


🧑‍🎓 Student Clubs & Workshops


🎓 Placement & Training Events


Integrate Google Calendar API with role-specific visibility.


📹 Instant Audio & Video Chat Option
Live video/audio calls within groups (especially for urgent document reviews or clarifications).


Schedule meetings directly from chat (integration with Google Meet or Zoom).



📅 Meeting Integration + Auto MoM Notes (IAOMS)
✅ 1. Google Calendar, Microsoft Teams, Zoom & Google Meet Integration
Enable scheduling, joining, and managing meetings from within IAOMS.
🔗 Key Features:
One-Click Integration with:


🗓️ Google Calendar (via Google Calendar API)


📹 Google Meet (auto-generated links)


🎥 Zoom (via Zoom API)


💬 Microsoft Teams (via Microsoft Graph API)


Attach IAOMS documents (letters, circulars, proposals) to meetings.


Add participants by role (e.g., Principal, Registrar, HODs).


Auto-email invites + in-app notifications.



💾 3. Storage & Distribution
MoMs are saved automatically as PDFs in:


The linked meeting folder (e.g., Google Drive)


Attached to the scheduled meeting on the IAOMS dashboard


Option to email MoM to all participants post-meeting.







✅ 📅 Principal-Led Meeting Scheduling with Auto MoM Integration (IAOMS)
🔷 1. Meeting Scheduling Initiated (Google Calendar Integration)
User: Principal logs in via IAOMS


Action: Schedules a meeting using an embedded Google Calendar Picker


Configuration:


Select Date & Time


Add Meeting Title


Choose Participants by Role (e.g., HODs, Registrar)


Toggle to Enable Auto MoM Generation


📎 Attach IAOMS Document → Select from existing:


Circulars (e.g., Circular D-2025)


Reports, Letters



🔗 2. Google Meet Link Auto-Generation
Upon scheduling:


Google Meet link is automatically generated using Calendar API


Meeting invite is:


📧 Emailed to all selected participants


🔔 Shown in the IAOMS dashboard under Upcoming Meetings



📝 3. Auto-Generated MoM Template
Created in Google Docs or IAOMS' internal notes system


Template includes:

 🗓 Date & Time  
👥 Participants (based on selected roles)  
📋 Agenda  
🗒 Discussion Points  
✅ Decisions Made  
📌 Action Items (with due dates)  



🤖 5. AI-Assisted Summary (Optional)
After the meeting ends:


Use Gemini API to:


Summarize key decisions


Extract action items


Highlight important points


Summary is added to the bottom of the MoM doc (under “AI Summary” section)



📤 6. Final MoM Distribution
🧾 MoM auto-saved as PDF


📁 Stored in a meeting-specific Google Drive folder


📩 Emailed to:


All participants


The initiator (Principal)


🔐 View/download from IAOMS dashboard archive


Feature Integration Overview
1. Meeting Scheduling with Google Meet
Use the Google Calendar API to programmatically create events on users’ calendars that include Google Meet conference links. Google for Developers+1


To generate a Meet link when creating an event, include a conferenceData object with a unique requestId and set conferenceSolutionKey.type to "hangoutsMeet". Also, specify conferenceDataVersion=1. Stack OverflowGist


This ensures that each scheduled meeting has a valid Meet link automatically included in the event metadata.


2. How It Works in IAOMS
On the meeting scheduling page, authenticated users select date, time, participants, and agenda.


IAOMS calls the Google Calendar API to create an event under the user’s calendar, embedding a Meet link.


The generated Meet URL is then displayed in the platform and included in email/dashboard notifications for attendees.

scheduling & joining meetings in IAOMS
1. Use Google Calendar API
Authenticate users with Google OAuth.


Use calendar.events.insert() to create a new event with date, time, and participants.


Add conferenceData.createRequest to automatically generate a Google Meet link.


Store and display this Meet link inside IAOMS for quick joining.


2. Workflow in IAOMS
User opens “Schedule Meeting” in IAOMS → selects date, time, and participants.


IAOMS calls the Calendar API → Event is created with a Meet link.


Meet link is shown on the meeting card & sent via email/notifications.


3. Benefits
No need to embed Google Meet itself — users just click the Meet link to join.


Works on web & mobile instantly.


Keeps integration light and secure.

Feature
How It Works
Meet Link Generation
Calendar API with conferenceData.createRequest, hangoutsMeet, version=1
Event Scheduling Flow
User schedules meeting → IAOMS inserts event via API → Meet link created




Integration Benefits
Streamlined meeting creation, real-time collaboration, enhanced workflows




📊 Poll & Feedback System
✅ Post-Event or Meeting Feedback Collection
Auto-Triggered Feedback Forms


After meetings (e.g., HOD reviews, circular briefings, or training sessions), the system:


Auto-sends a Google Form or internal form module


Includes key fields: Rating (1–5), Comments, Suggestions


Tagged to the specific event, date, and organizer for tracking


Smart Reminders


If feedback is not submitted within a deadline, the system sends a gentle reminder


✅ Live Polling During Review/Discussions
Real-time polls inside the IAOMS chat/discussion system


Used during circular reviews, academic planning, etc.


Poll types:


Multiple choice


Yes/No


Likert scale (1–5)


Results visualized instantly as:


Pie charts


Bar graphs


Exportable poll data for record keeping



🗳️ Digital Voting & Approvals
✅ Use Case: Academic Council / Committee Voting
Secure Voting System inside IAOMS:


Voting options: Yes / No / Abstain


Roles allowed: Committee Members, Council Heads, etc.


Live Tally + Summary


Visual vote count in real-time


Voter identity hidden (anonymized) or shown (based on setting)


After completion:


Email summary is sent to participants


Decision and vote count are auto-logged


✅ Permanent Decision Logs
Each voting session is:


Archived in a Decision Logbook


Assigned a reference number, timestamp and Date, and final outcome


Can be filtered and searched by:


Department


Topic


Date


Voter group





🧩 Visual Workflow Builder – Vector-Based Drag-and-Drop Interface
A no-code canvas interface that allows institutional administrators to visually design document approval workflows with ease.

🖥️ 1. Interactive Canvas: Role-Based Node Blocks (With Role Library for Recipient)
The canvas includes a dynamic drag-and-drop role library for creating approval flows.

🎯 Role Block Categories (by Sender Type):

✅ Principal – Authorized Node Blocks:
(Used when the Principal initiates the workflow)
Role Name
Block Icon/Color
Mentors/Employees/faculty (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)


🟩 Green
✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


🟦 Blue
HODs (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)
🟪 Purple
Registrar
🟨 Yellow
CDC Department Employees
🟫 Brown
Dean
🟥 Red
Chairman
🟧 Orange
Director (For Information)
⬛ Black
Leadership
⚪ White
Controller of Examinations
🟫 Dark Red
Asst. Dean IIIC
🟨 Light Orange
Head Operations
🟩 Teal
Librarian
🟪 Light Purple
SSG
🟥 Pink
HOD EEE
🟨 Yellow
HOD MECH
🟩 Green
HOD CSE
🟦 Blue
HOD ECE
🟥 Red
HOD CSM & CSO
🟧 Orange
HOD CSD & CSC
🟪 Purple


✅ Employee – Authorized Node Blocks:
(Used when an employee initiates the workflow)
Role Name
Block Icon/Color
Program Department Heads (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)
🟦 Blue
HODs (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)
🟪 Purple
Registrar
🟨 Yellow
Principal
🟥 Red

.

🧩 Drag, Connect & Build:
Drag the relevant role blocks to the canvas.


Connect them with arrows to define the approval sequence.


Add smart logic (conditions, parallel flow, timeouts, etc.).






➡️ 2. Connect With Smart Arrows
Draw arrows between role nodes to define workflow order:
🔁 Flow Types:
Linear Flow – (e.g., Employee ➝ Registrar ➝ Principal)


Parallel Approval – (e.g., sent to HODs (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th) at the same time)


Conditional Routing – (e.g., If Rejected by Registrar ➝ Escalate to Dean)


Arrows can be:
Dashed for conditional logic


Solid for mandatory flow


Colored based on type (e.g., Red = Rejection, Green = Approval)



🧠 3. Smart Logic & Advanced Options
Each node or connector allows smart customization:
Feature
Function
🔀 Decision Nodes
Add "If-Else" conditions (e.g., If Rejected ➝ Escalate to X)
🕒 Timeout Triggers
Auto-escalate if a role takes no action within X days
💬 Comment Toggle
Require mandatory comments before proceeding
🔒 Lock Step
Lock editing after a specific approval (e.g., After Principal signs)
🔁 Auto Loops
Return to originator if incomplete or rejected


🛠️ 4. No-Code Editing Capabilities
Admins can:
⚙️ Customize and save templates (e.g., "Academic Approval", "Placement Letter Flow")


📤 Export, duplicate, and share workflow templates across departments


🧪 Simulate/test routing before going live


All without developer assistance.

🎯 Sample Use Case: Research Grant Proposal Flow
Employee ➝ HOD-CSE ➝ Registrar ➝ Principal
If Registrar Rejects → Escalate to Dean
If no action in 2 days → Auto-notify Director

✔️ This can be visually created, tested, and deployed in minutes.

🔍 AI-Powered Gemini Integration (Optional)
Gemini AI suggests the optimal flow based on past documents or content type.


Can auto-fill roles, detect dependencies, and recommend templates.



✅ Benefits for IAOMS
Feature
Benefit
🧩 Drag-and-Drop Customization
Build workflows easily, visually, intuitively
🔄 Role-Based Dynamic Routing
Supports department-level personalization
💡 AI Recommendations
Speeds up flow setup using Gemini insights
👥 Decentralized Access
Admins, Deans, Principals can independently configure
📦 Workflow Reusability
Save and reuse across Letters, Reports, Circulars



🛠️ Low-Code Workflow Builder (Admin Panel Feature)
A visual drag-and-drop interface that empowers administrators to design, customize, and update approval workflows — all without developer involvement.

✨ Core Capabilities
🔧 Define Workflow Logic:
Select and assign user roles (e.g., HOD, Registrar, Principal).


Build sequential or parallel approval flows.


🔁 Set Conditional Rules:
Example:
 “If document is rejected by Registrar ➝ auto-escalate to Director for re-evaluation.”


🔕 Notification Control:
Toggle email alerts and dashboard notifications per stage.


Enable/disable comment fields or attachments during approvals.


🔐 Document Access Controls:
Lock or unlock the document for editing at each stage.


Set visibility rules (e.g., draft mode visible to HOD only).



⚙️ Advanced Features
🔄 Auto Re-routing on Delay or Rejection:
Automatically redirect the workflow if:


An approver fails to respond within X days


A document is rejected, triggering an escalation or reassignment.


📬 Real-Time Communication:
Email + Dashboard alerts triggered on:


New document submission


Stage transitions


Final approvals or rejections


🔗 Dynamic Routing (Decentralized Support):
Centrally managed routing by Principal/Admin
 or


Decentralized flow where each department controls its own internal routing logic.



✅ Why This Matters
Eliminates coding dependency for minor changes.


Empowers HITAM admin staff to respond quickly to institutional process changes.


Enables experimentation and optimization of workflows without risk.





✅ How NLP Can Be Used in IAOMS (All kinds of Recipient)
1. 🧠 Auto-Summarization of Documents (TL;DR)
Use NLP to automatically summarize Letters, Circulars, and Reports.
🔍 Extracts the key points


📝 Generates a "Too Long; Didn’t Read" (TL;DR) version


💼 Helps HODs, Principals, and Employees quickly grasp intent


Tech Stack:
 Gemini AP/ Hugging Face Transformers (Bart, T5)

2. 🧾 Intent Recognition in Submissions
When an Employee enters free-text in a form or email:
NLP detects intent: (e.g., "I need approval for a guest lecture" → recognized as “Permission Request”)


Classify it into: Leave, Event, Budget, Resource, etc.


Route the document accordingly and suggest templates


Tech Stack:
 spaCy for entity recognition + custom-trained classification models

3. ✍️ Smart Drafting and Auto-Completion
Auto-generate drafts of:
Circulars


Meeting Agendas


Reports


Based on form data or previous examples using NLP:
Pre-fill headers, roles, salutations


Adjust tone (formal/informal)


Suggest closing lines or signature formats


Tech Stack:
Gemini + templating via Google Docs + Apps Script

4. 📥 Automated Comment Interpretation
When a document is rejected and a comment is entered:
NLP parses comment to extract actionable reason


Tags common issues (e.g., “missing budget line,” “wrong department”)


Suggests revision automatically


Tech Stack:
 Keyword extraction models + rule-based sentiment tagging

5. 🧾 Document Tagging and Metadata Extraction
Use NLP to automatically tag uploaded documents:
Detect document type, department, topic, and urgency


Apply intelligent tags like: "Academic", "Finance", "Time Sensitive"


Use Case:
 Improves search, filtering, and analytics in the dashboard

6. 💬 Smart Chat Assistant for Employees/Principals
Provide a chatbot assistant for:
Asking, “Who should approve my leave?”


“Show me documents pending with the registrar”


“Draft a circular for Workshop X”


Tech Stack:
 ChatGPT + Firebase Auth for access-level control

7. 🗓️ Natural Language Date & Time Recognition
Let users type:
“Schedule meeting next Friday at 2 PM with recipients"
NLP interprets it and schedules it in the system’s calendar.
Tech Stack:
 Duckling / NLP.js / Chrono Node for time parsing

8. 🔍 Semantic Search Engine for Archived Docs
Use NLP for contextual search:
“Find circulars about workshops in 2023”


“Show rejected documents with comments about budget”


Tech Stack:
 Elasticsearch + NLP embeddings (sentence-transformers, GoogleAI embeddings)

🔐 Bonus: Role-Based NLP Restrictions
Ensure NLP-based suggestions or access is aligned with:
Google Login Role


Department (HOD, Registrar, Employee)


Document Permission Level


🤖 AI & NLP-Powered Automation Features for IAOMS

🔍 AI-Powered Intent Detection in Proposals
When employees or departments submit requests or circulars:
✅ Detect Intent Type:


Emergency ⚠️


Informational ℹ️


Formal Approval ✅


Follow-up/Reminder 🔁


✅ Smart Recipient Suggestions:


NLP analyzes the subject/content and auto-suggests relevant roles Recipients

✅ Auto-Routing:


Proposals are automatically routed to the right reviewers based on urgency and department.



🧠 NLP-Based Role Suggestion Engine
When typing or uploading circulars, reports, or letters:
✅ Real-time Intent Recognition:


Example:


 "Detected intent: Faculty Duty Exemption"
 Suggest Routing:Employee ➝ Program Department Head  (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)➝ HODs (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th) ➝ Registrar ➝ Principal


✅ Auto-Suggest Signature Roles:


Based on context (e.g. academics, student affairs).


✅ Smart Suggestions for Templates:


Recommends structure/layout used in similar past documents.



🎓 Auto-Generate Certificates (Event Automation)
When an event or workshop concludes:
🎯 On submission of feedback form:


System auto-generates Certificate of Participation/Completion using:


Google Docs templates


Embedded eSignatures


📥 Download includes:


“Certified by: Principal, Registrar, Event Coordinator”


Optionally archived for future audits



✍️ Smart Form Auto-Fill
During circular or letter submission:
✅ Auto-fills:


Logged-in user’s department


Date


Designation


✅ Recommends:


Pre-used templates


Signature roles


Attachments based on topic (e.g., MoU, Approval copy)



📊 Reporting & Analytics Dashboard
For Principals, Registrars, or HODs:
Graphs & Panels Show:


🧾 Total documents generated, reviewed, approved


⏱️ Average approval time


🔁 Delay frequency (by role or month)


📅 Time-to-closure metrics



🚨 Auto-Escalation Engine
To prevent bottlenecks:
⏰ If a document remains unapproved for X days:


Auto-escalate to the next senior authority


Trigger email/WhatsApp alerts



🧩 Smart Compliance Mapper (AI for Accreditation Readiness)
When generating or uploading a document:


The system auto-detects compliance relevance, such as:


🏛 AICTE


🔍 NAAC


📊 NIRF


✅ Tags documents accordingly


✅ Suggests folders to archive


✅ Optionally notifies the Compliance Officer


✍️ Form Auto-Fill & Smart Suggestions
When creating a document:


Auto-fill user name, department, and timestamp based on login.


Suggest previously used titles, document types, templates.


AI suggests roles to route the document to — based on keywords.










Let IAOMS users interact with Google Workspace content (Docs, Sheets, Slides) inside the IAOMS website without leaving it.
How it works:
Embed Google files directly into IAOMS pages so users can view (or lightly edit) them right there.


Example: A teacher opens a report Google Doc directly on IAOMS without opening Google Docs in another tab.


This can be done using an HTML <iframe> tag, which acts like a live window showing the document inside your site.


Light editing inside IAOMS:


Change the link type from /preview to /edit in the file URL to let users edit.


Example:


View: https://docs.google.com/document/d/FILE_ID/preview


Edit: https://docs.google.com/document/d/FILE_ID/edit


Drive API integration:


Use Google Drive API to fetch a list of relevant files for a user’s role (Principal, HOD, Employee).


Display those files as inline widgets or previews in IAOMS.


Clicking a file opens it right in the dashboard using <iframe> or a custom viewer.


Why this is useful for IAOMS:
No need to switch between IAOMS and Google Drive.


Reports, circulars, letters can be viewed, edited, and approved in one place.


Keeps workflow smooth for busy institutional roles.
📌 Feature: Google Workspace Integration for IAOMS
Objective:
 Integrate Google Workspace into IAOMS to display embedded files, inline previews, and actionable insights directly in the UI, enhancing collaboration without leaving the platform.

🔹 Implementation Approach:
Google Drive API Integration


Use the Drive API to fetch, list, and manage Workspace files (Docs, Sheets, Slides).


Apply role-based permissions (from IAOMS PRD) to ensure only authorized users see files.


File Embedding & Preview


Use <iframe> embeds for quick viewing or light editing:

 <iframe src="https://docs.google.com/document/d/FILE_ID/preview" width="100%" height="600"></iframe>


Supported: Google Docs, Sheets, Slides.


Inline Widgets


Design UI cards or widgets that preview the first page/sheet/slide.


Show metadata: file name, last modified, owner, AI-generated summary.


AI-Powered Enhancements


Google Gemini API to auto-generate insights, summaries, and suggestions.


Example: If a file is a circular, auto-extract deadlines and approval roles.


User Actions


View → Inline preview via <iframe>


Edit → Opens file in Google Docs/Sheets/Slides in a new tab or embedded editor.


Share → Role-based sharing link creation via Drive API.


Security & Compliance


Use OAuth 2.0 with restricted @hitam.org access.


Apply Supabase Row-Level Security to match file access with IAOMS role hierarchy.


Right now, we’re talking about embedding Google Workspace content (Docs, Slides, Sheets) in IAOMS so users can open and see them right inside your site.
Earlier, you also mentioned a Google Docs embedded editor with:
AI formatting & summarization


Digital signature tools


Approval workflows


When I said I could pair this into your PRD, I meant:
Combine both concepts into one section in your IAOMS PRD.


That section would describe:


Viewing & previewing Workspace files via <iframe> or Drive API.


Full editing & collaboration inside IAOMS using the embedded Google Docs editor.


AI-powered enhancements (auto-format, summaries).


Built-in signature & approval tools without leaving IAOMS.


This way, instead of having two separate scattered ideas, you’d have one unified PRD section for Google Workspace + Google Docs AI + Signature Integration.
 That makes it easier for developers to implement it as a single feature set rather than piecing it together.
📄 Google Workspace & Docs AI Integration
Objective
Enable users to view, create, edit, and collaborate on institutional documents (Letters, Circulars, Reports) directly within IAOMS using Google Workspace tools, enhanced with AI formatting, summarization, and secure approval workflows.

Core Features
Embedded Workspace Previews


Use <iframe> embeds or Google Drive API to display Docs, Slides, Sheets within the IAOMS UI.


Modes:


View Only – Secure preview without download.


Light Edit – Inline updates with permissions.


Inline Widgets for quick previews (file title, owner, last modified).


Full Google Docs Editor Inside IAOMS


Edit and collaborate in real time without leaving the platform.


Google Docs editor embedded inside IAOMS with:


Role-based permissions (View/Edit/Comment).


Auto-save to Google Drive institutional folder.


AI-powered auto-formatting, auto-summarization, and grammar correction using Google Gemini API.


Digital Signature & Approval Workflow


Integrated signature tools within the Google Docs editor:


✍️ Draw or upload signature.


📅 Auto timestamp & role tagging.


🛡️ Flatten signatures for final exports (PDF/DOCX).


Approval buttons (✅ Approve, ❌ Reject, 💬 Comment) directly in the embedded doc interface.


Integrated Insights & Search


Workspace file metadata integrated into IAOMS Universal Search.


AI-driven insights:


Detect document type (leave letter, meeting circular).


Recommend recipient routing based on content.



Technical Implementation
Google Drive API for file storage and retrieval.


Google Docs API for embedded editing.


Google Calendar API for meeting links from document discussions.


<iframe> embeds for preview and light editing mode.


AI layer via Google Gemini API for formatting & summarization.


Role-based access control via Supabase Auth + Workspace Permissions.



Expected Benefits
One-stop document hub – No need to download or switch tabs.


Faster approval cycles – Edits + signatures happen in the same space.


Consistency – All docs stored in structured, searchable format.


AI efficiency – Content auto-polished before review.




1. Embedding for View-Only
You can embed a published Google Doc into an iframe for read-only viewing:
Publish the document via File → Share → Publish to the web → Embed.


Insert the generated <iframe> in your IAOMS page. Updates in the Doc reflect automatically.ClickUpsupport.strikingly.com


2. API-Based Document Creation and Editing
To enable full document workflows, use the Google Drive API and Google Docs API:
Create new documents using files.create from the Drive API.Latenode Official Community


Populate or edit document content using the Google Docs API, particularly methods like documents.create, get, and batchUpdate.Google for Developers+1


3. In-App Editing Workflow (Indirect)
To simulate an embedded editing experience:
Upload or create the document via the Google Drive API.


Redirect users to the Google Docs editor URL (docs.google.com/document/d/{documentId}/edit).Latenode Official CommunityStack Overflow


Once edits are complete, sync changes back into IAOMS using Docs API if needed.


This maintains full editing functionality while keeping your system in control of routing, permissions, and tracking.

Why This Approach Works for IAOMS (Per PRD)
Seamless Integration: Users can click "Edit in Docs," make changes, and return to IAOMS automatically.


AI & Signature Features: IAOMS can generate drafts, insert signature placeholders, and route workflows before handing off to the Google Docs editor.


Security & Compliance: You retain control over who can access documents, via your app’s authentication and Google’s OAuth.


Audit Trail & Archiving: Store document IDs and change logs via API, aligning with PRD’s archival and audit requirements.



Functionality
Implementation Option




View-Only Embedding
via iframe published doc
In-App Editing
via Drive & Docs API with redirection
AI Integration
Pre-populate templates, summaries via API
Signature Workflow
Insert placeholders before user edits
Document Sync & Archival
Track via API, store metadata and versioning


Use this object for dashboard filtering, approval flows, and signature stamping.

In IAOMS, a Google Docs Canvas (integrated or embedded editor) can be a powerful feature to make your document creation, editing, and approval process seamless — without leaving the system interface.
Here’s how Google Docs Canvas can be used in IAOMS:

1. Embedded Document Editing in IAOMS
Inline Editing:
 Users can open and edit Google Docs directly inside IAOMS via an embedded iframe or Docs API integration.


Real-Time Collaboration:
 Principal, HODs, Program Heads, and Employees can co-edit in the same IAOMS window without switching tabs.



2. Role-Based Signature Integration
Signature Placeholders in Canva:
 When a document is opened in the embedded Docs Canva, the system automatically inserts role-based signature zones (Principal, HOD, etc.) in the correct positions.


Interactive Signing:
 Once reviewed, the signature canvas (hand-drawn, upload, saved) appears in Docs Canva, and the signed version is auto-saved.



3. AI-Enhanced Editing Inside Canva
Gemini AI Toolbar in Canva:


Grammar correction.


AI-generated summaries.


Role suggestions (e.g., detect “Leave Request” → auto-assign to HOD).


Layout suggestions (font, spacing, NAAC compliance).



4. Workflow Automation
Pre-Filled Docs:
 When a user selects “Create Circular” in IAOMS, the system:


Loads a Google Docs Canva editor with a pre-filled template (date, department, sender details).


Lets the user edit directly.


Save & Route:
 Clicking Submit for Approval saves the document to Google Drive (linked to IAOMS) and routes it to the selected roles in the approval workflow.



5. Compliance & Archival Benefits
Audit Trail:
 Google Docs Canvas maintains edit history inside IAOMS for NAAC/NIRF audits.


Export Options:
 Final approved docs can be exported directly from Canva as PDF/DOCX with embedded signatures.


Version Snapshots:
 Each approval stage can store a version snapshot for legal compliance.







💡 Why it’s powerful in IAOMS:
Eliminates downloading & re-uploading files.


Integrates AI, approvals, and signatures in one live document interface.


Keeps all versions centralized in Google Drive with instant cloud backup.





1. Centralized & Standardized Document Creation
Templates:
 Predefined Google Docs templates for letters, circulars, and reports ensure uniform formatting across departments (aligned with HITAM branding).


Version Control:
 Google Docs automatically keeps a version history, so users can revert to previous drafts if needed.


Real-Time Collaboration:
 Multiple roles (HOD, Principal, Registrar) can co-edit documents during review before final approval.



2. AI + Google Docs Integration
Google Gemini API (as per PRD) can pull a draft into Google Docs, apply grammar correction, summarization, or role-based formatting.


Automatic insertion of signature placeholders in the correct zones based on document type and recipient role.



3. Structured Workflow Support
Role-Based Access Control:
 Supabase + Google Docs permissions ensure:


Principal → full access.


Employees → edit until submission.


Reviewers → comment/suggest mode.


Eliminates multiple file versions being sent over email.



4. Signature Workflow
After AI processing, Google Docs → PDF conversion can embed signatures (drawn, uploaded, or saved) directly into the correct positions.


Back-side signature pages can be auto-generated before exporting the final approved document.



5. Automation & Archiving
Auto-Conversion: Uploaded .docx, .pdf, or scanned images can be converted into editable Google Docs for formatting and signature placement.


Archiving: Final signed Google Docs are automatically saved in a Google Drive institutional folder with role-based access.



6. Approval Integration.


MoM (Minutes of Meeting) auto-generated in Docs → stored in project’s Google Drive → linked in IAOMS dashboard.



7. Compliance & Audit
Maintains a timestamped change log for NAAC, NIRF, or AICTE audits.


Can integrate QR code in the final document linking to the live Google Doc (read-only mode) for verification.



Google Docs Canva embedded inside IAOMS with AI and signature tools, so you can pitch it visually in your project.



Automatically stored in Google Drive in a structured folder hierarchy (e.g., Department → Year → Type → Date).


Indexed for AI processing so Google Gemini (or other AI) can:


Learn from existing documents to suggest templates.


Auto-complete repetitive sections.


Recommend correct recipients based on past patterns.


Reusable as smart templates — allowing users to quickly load a past document, adapt it, and re-send it.


Searchable via full-text and tag-based filters inside IAOMS.


Linked with signature workflows — previous documents retain signature zones so similar layouts can be reused without manual setup.


Essentially, the AI can be trained on stored Google Docs so IAOMS “remembers” institutional document formats, approval flows, and common phrases, making future document creation and routing faster.
📄 AI-Enhanced Google Docs Integration in IAOMS
Training on Institutional Documents:
 The Google Docs canvas inside IAOMS is trained on the uploaded files (reports, circulars, letters) to understand institutional formats, tone, and compliance requirements.


Automated Storage & Reuse:
 Every submitted document (letter, circular, or report) is automatically stored in a secure, role-based institutional repository.


Accessible for future reference, template reuse, and AI-powered drafting.


Searchable via Universal Search with filters (document type, department, status).


AI-Assisted Drafting:
 When a new document is created, the AI references the stored collection to auto-generate drafts in institution-approved formats, reducing manual editing.


Version Control & History:
 Stored docs maintain version history, showing all edits, approvals, and signatures.


Role-Based Retrieval:
 Principal, HODs, Registrar, and Employees can retrieve stored documents only within their access rights, as defined in the PRD’s Role-Based Access Control.

Here are four visual references that align well with the IAOMS Google Docs Canvas integration concept:
Google Docs Approval Sidebar – Demonstrates how an approval interface can appear integrated next to the document editor (source: Wake Forest University) .


Document Approval Workflow Mockup – Shows a clean task/status view for document reviews—great for inspiration on approval dashboards or status displays .


E-Signature Integration Panel – Example of adding signatures directly within the Docs interface via a side panel .


Signature Workflow Form Extension – Illustrates embedding signature workflows in forms, helpful for role-based signing logic .



Design Recommendations for IAOMS Docs Canvas
Embedded UI Layout:
Central Pane: Houses the Google Docs editor with embedded signature placeholders and handoff interface (e.g., Approve/Reject buttons).


Left Sidebar: A visual workflow navigator with user roles (Principal, HOD, Registrar, etc.), showing document status for each.


Right Sidebar: An AI-powered assistant panel offering:


Grammar corrections


Summarization


Routing suggestions


A signature tools menu (hand-draw, upload, saved signature option)


UX Flow Highlights:
Document auto-loads with pre-filled template and role-based signature zones.


Collaborators can review inline—AI assists in real-time.


When signing, the right sidebar presents tools for choosing or drawing a signature.


All edits, comments, and signature actions are logged for audit and version history.



Profile Settings Page – Recommended Structure
1. Basic Information
Profile Picture – Upload/change option with preview.


Full Name – Editable.


Email ID – Pre-filled from authentication (Google Sign-In / HITAM ID) and non-editable.


Role & Department – Auto-filled from database (Principal, HOD, Employee, etc.).



2. Contact Details
Phone number (optional, editable).


Alternative email (optional).



3. Authentication & Security
Change password (for HITAM ID login).


2FA toggle (if enabled in PRD scope).


Logout from all devices option.



4. Notification Preferences
Email Alerts – Toggle + frequency selector (every 1 min / 15 mins / 1 hour / daily).


Dashboard Notifications – Toggle.


WhatsApp Alerts – Toggle (if WhatsApp API integrated).



5. Document & Workflow Preferences
Default document view (list / grid).


Auto-open approval canvas toggle.


Default signature option:


✍️ Draw


📷 Camera scan


💾 Saved signature



6. Personalization
Dark mode toggle.


Language selection (future Gemini NLP regional support).



7. Saved Signatures
Manage stored signatures (add / remove).


Preview with name + timestamp.



8. Account Actions
Download my activity log.


Request data deletion (GDPR compliance).




✅ Document Signature Processing & Smart Layout System in Google Docs
📌 Functionality Overview
A smart and flexible digital document signing system designed to support employees, principals, and multiple institutional roles in approving official documents like letters, circulars, and reports with complete integrity, layout preservation, and seamless export.

🛠️ Problem Scenarios & Solutions

🔹 Inline Signature Requirement
Scenario: Some professionals prefer to download and sign on the same page rather than using a separate review page.
✅ Back-Side Signature Download Option
 Users can download the document with all signatures placed on the back side of the document for clean presentation.
 → Scanned signatures are auto-resized using adjustable logic to fit clearly and professionally.


✅ Approval Without Signature (Basic Use Cases)
 Users can choose to simply Approve or Reject with a comment – no signature canvas required. Ideal for routine approvals.



🔹 Multiple Signatories on the Same Page
Scenario: Multiple roles (HODs, Program Heads, Registrar, Principal, etc.) must sign the same document.
✅ Multi-Signature Overflow Management
 If signatures exceed page limits:
 → System auto-creates additional pages per group of signers.
 → Users can scroll or navigate tabs to see and sign.



🔐 Secure Signature Handling – Enhanced Options
✅ E-signature Canvas Options


✍️ Hand-Drawn Signature


📷 Upload Signature via Camera


💾 Use Saved Signature


✅ Auto Date & Time Stamp, Comments (optional), and Role-based Visibility



📄 Google Docs Integration for Document Structuring
✅ Auto-Conversion of Letters, Circulars, Reports
 → The uploaded content is parsed and converted into structured Google Docs using predefined templates.
 → Roles selected for signatures are dynamically embedded with signature placeholders.


✅ Smart Layout Adjustments:


Font resizing


Spacing optimization


Role-specific formatting


Predefined zones for signature alignment



⚠️ Content Size Warning System
If a document exceeds layout limits (e.g., >500 words):
 → Display warning message
 → Recommend predefined Google Doc template
 → Open Canvas Editor for manual layout + signature zone creation



🤖 AI-Powered Workflow Enhancements
✅ Google Gemini API Integration
Refines raw content


Extracts signer roles


Suggests formatting templates


Auto-draft summaries, circulars, or reports



✅ Role-Based Signature Canvas
Scans documents for roles


Adds “View to Sign” buttons per role


Opens a small canvas panel for signature


Auto-embed metadata: Name, Role, Timestamp, Optional Comment



📥 Final Download & Export System
✅ Export Formats:


PDF


Google Docs


DOCX


✅ Clean Output:


Removes all “View to Sign” elements


Auto-embeds signatures directly


Generates flattened PDF with all signatures as non-editable static elements



🖋️ Verified Signature Block Output Example
─────────────────────────────
🖋️ Verified Signatures:
[Signature Image] Dr. ABC – Principal – 25/07/2025, 4:32 PM  
[Signature Image] Mr. XYZ – Registrar – 25/07/2025, 4:40 PM  
[Signature Image] Ms. LMN – HOD-CSE – 25/07/2025, 5:02 PM  
─────────────────────────────


✅ Dynamic Signature Placement & Layout Control
1. Role-Based Signature Zones
Role
Zone
Principal/Registrar
Top-right (Header)
HODs
Body-End (Left)
Program Heads
Footer (Right)

2. Collapsible Signature Blocks
Compact tiles expand to show:


✍️ Draw Signature


📷 Upload Photo


🛡️ Use Certificate (optional)


3. Auto Pagination (If Needed)
If >4 signatories on one page:


Auto-generate “Signature Page 2”


Add inline notes: “See Page 2 for Principal Signature”



📄 Alternative Workflows
✅ Manual Download + Upload Workflow
User downloads doc with signature placeholders


Signs manually


Re-uploads to complete the approval process
 → Signatures placed at designated blocks.



✅ Signature-less Approval Flow
Simple Approve / Reject buttons


Optional comment


Logged in backend (Sheets/Firebase)


Trigger email notifications via Gmail API



✅ Minimal Layout + QR Code/Audit Trail Optional
Auto-generate digital stamps:


🛡️ Verified: Prof. A. Sharma, HOD-CSE | 2025-07-26 14:30 IST

Optional:


🔗 View audit log: https://portal.hitam.org/signatures/2025-07-26


✅ Final Flattened Output:
All signatures are embedded as static, non-clickable elements


No view links, no extra pages, no external canvases


Clean, professional, and offline printable


PDF = Fully sealed, legally valid, and ready for records



✅ Supported Roles for Digital Signatures
Principal


Registrar


Dean


Director


– HODs (All branches-EEE, MECH, CSE, ECE, CSM, CSO, CSD, CSC, and Years- 1st,2nd,3rd,4th)


– Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD, CSC, and Years- 1st,2nd,3rd,4th)


Asst. Dean / CDC / IIIC / Library


Controller of Examinations


Operations / Leadership / SSG


Mentors (All Years)


Employees with assigned workflow access





📄 Professional Document Signature Processing & Smart Layout System in Google Docs
✅ Core Functionality Overview
Back-Side Signature Download


Users can download documents with all collected signatures neatly placed on the back side for better space utilization.


Scanned signature images auto-resize dynamically using adjustable logic to fit designated areas.


Signature-less Approvals


For basic workflows: Users can Approve or Reject with optional comments — no signature canvas required.


Multi-Signature Overflow Management


Automatically splits signatures across dedicated continuation pages when the main page lacks space.


Roles are organized hierarchically (e.g., Principal → HODs → Program Heads).


Users can scroll/swipe between signature pages or use a horizontal tray layout for compact overflows.


Role-Based Signatory Support


Fully supports institutional hierarchy:


Principal, Registrar, Dean,– HODs (All branches-EEE, MECH, CSE, ECE, CSM,CSO, CSD,CSC and Years- 1st,2nd,3rd,4th)
– Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)
 Controller of Examinations, etc.



🤖 AI-Powered Document Processing
Google Gemini Integration


Uses Gemini to refine content, extract signatory roles, and generate templates.


Supports auto-summarization and professional drafting of Letters, Circulars, and Reports.


Auto-Conversion & Structured Layout


Uploaded PDFs are converted into structured Google Docs using smart templates.


Role-specific signature placeholders are inserted.


Content is optimized for:


Font size, spacing, alignment.


Includes a word limit warning system (e.g., >500 words triggers a layout suggestion).


Role-Based Signature Canvas


Automatically detects signatory roles in the document.


Embeds interactive “🖋️ View to Sign” buttons next to each role.


Opens a lightweight inline panel supporting:


✍️ Hand-drawn canvas


📷 Camera-scan or image upload


💾 Saved signature reuse


📅 Auto timestamp + 🗒️ optional comments



🛠️ Signature Handling & Security
Dynamic Placement Zones


Based on the user’s role, signatures are auto-placed in specific areas:


Principal/Registrar: Top-right or footer


HODs: Lower body section


Program Heads: Page end/right margin


Collapsible Blocks: Compact views that expand only on interaction.


Secure Workflows


Digital signature canvas for manual signing.


Optional Blockchain support (optional): Document hashes stored for immutable verification.


Encrypted Signature Stamps:

 ✔ Verified: [Encrypted Stamp ID]
Prof. A. Sharma, HOD-CSE
2025-07-26 | 14:30 IST


Offline/Manual Signing


Download the document with pre-filled signature fields and re-upload after manual signing.



📥 Export & Finalization
Flattened PDF Export


All interactive elements (e.g., “View to Sign” buttons) are removed.


Embedded as static, professional signatures with:


Name, role, time


Size-minimized for clarity


Consolidated Signature Section


Adds a final block:

 🔐 SIGNATURES
[Sig] Dr. ABC – Principal – 25/07/2025, 4:32 PM
[Sig] Mr. XYZ – Registrar – 25/07/2025, 4:40 PM


If overflow occurs: A separate Signature Continuation Page is created automatically.


Single-Page Optimization


If space permits, embeds all signatures directly on the same page — 100% print-friendly and offline-compatible.



⚙️ Document Workflow Automation
Generation & Storage


Documents are auto-generated from templates, ERP exports, or forms.


Stored in Google Drive with role-specific access via SuperBase Authentication.


Notification System


Gmail API sends automated alerts for approvals, rejections, and comments.


Audit & Verification


Generates a QR code or link to a complete log of digital signatures:

 🔗 View Signatory Log: https://portal.example.org/signatures/2025-07-26



🚫 Critical Workflow Constraints
No interactive UI elements remain in final exports.


No need to redesign original circulars to “fit” signatures.


Compact layout: Max 3–4 signatures per page; rest go to next.


Compatible with original uploads (PDF/Word); no full dependency on templates.



🌐 User Flow Summary
Upload document (PDF or Doc).


Select required signatory roles.


Each signatory:


Signs via canvas/camera


Or approves/rejects with comments


System auto-embeds all final signatures and metadata.


Flattened version generated → download or archive.





🖥️ 1. Interactive Canvas: Role-Based Node Blocks
(With Role Library for Principal & Employee)
Design an interactive visual workflow builder—similar to Blender’s node-based system—for institutional processes within IAOMS.
✅ Canvas Features:
Drag-and-drop role blocks All Kinds of Recipient


Connect blocks with arrows/lines to define workflows (linear, conditional, or parallel approvals)


Zoom & pan controls for ease of navigation


Real-time preview of approval logic


✅ Role Library (Customizable per Institution):
Principal


Registrar


All HODs (EEE, MECH, CSE, ECE, CSM,CSO, CSD, CSC)


✅ Program Department Heads (All Branches-EEE, MECH, CSE, ECE, CSM ,CSO, CSD, CSC and Years- 1st,2nd,3rd,4th)


Mentors (All Years)


Employees


Dean, Director, Chairman, Controller of Examinations, etc.


✅ Advanced Logic Nodes:
🔀 Decision nodes (If Approved / Rejected → Go To...)


⏳ Timeout Escalation (e.g., escalate if pending > 2 days)


💬 Add Comment Required


🔒 Lock Document on Approval


✅ Key Benefits:
No-code, admin-friendly setup


Reusable templates for common workflows (e.g., academic approvals, emergency reports)


Faster customization for department-specific logic


Simulation Mode: Preview and test the node path before publishing





✅ Solving the Role-Based Login & Workflow Without HITAM's Official Database
You want to simulate role-based login and approval workflows using HITAM email IDs (*@hitam.org) and HITAM IDs (e.g., HITAMCSE1234) without access to HITAM's internal role directory.
Here’s a step-by-step solution using Supabase with options for flexibility, fallback, and future scalability:

✅ 🔐 1. Google Sign-In with HITAM Email Domain Restriction
Use Supabase Auth or Firebase Auth with Google OAuth:
Supabase Setup:
Enable Google Sign-In from Supabase dashboard.


In email domain restriction, allow only: @hitam.org.


-- Row-Level Security logic (optional)
check_email_domain(email) RETURNS boolean AS $$
BEGIN
  RETURN email LIKE '%@hitam.org';
END;
$$ LANGUAGE plpgsql;


🧠 2. Simulated Role Assignment Approaches
✅ Option A: Mock Role-Based Database (Best for Demo)
Create a users table:
Table: users

| id (uuid) | name        | email                | hitam_id    | role       | department | created_at       |
|-----------|-------------|----------------------|-------------|------------|------------|------------------|
| UUID      | SriChaitanya    | 22e51a6917@hitam.org  | HITAM001    | Principal  | Admin      | CURRENT_TIMESTAMP|
| UUID      | Ms. Lakshmi | registrar@hitam.org  | HITAM002    | Registrar  | Admin      | CURRENT_TIMESTAMP|
| UUID      | Mr. Arvind  | arvind.cse@hitam.org | HITAMCSE101 | HOD        | CSE        | CURRENT_TIMESTAMP|

On login:
Query by email or HITAM ID


Pull role, name, and department


Save into sessionStorage or backend token claims


✅ Option B: Email/ID Pattern-Based Detection (Fallback)
function inferRole(email, id) {
  if (email === "principal@hitam.org") return "Principal";
  if (email.includes("registrar")) return "Registrar";
  if (email.includes(".cse@hitam.org") || id.startsWith("HITAMCSE")) return "HOD-CSE";
  return "Employee";
}


📝 3. Manual Admin Approval (Optional, Recommended for Edge Cases)
If role detection fails:
Save user to pending_users table


Admin panel allows manual role assignment


Once approved, move to users table



🗃️ 4. Role Persistence & Identity Mapping
Save role/session information securely:
Backend:
users table stores: email, hitam_id, name, role, department, login_time


Frontend:
localStorage.setItem("user", JSON.stringify({
  name: "Mr. Arvind",
  email: "arvind.cse@hitam.org",
  role: "HOD-CSE",
  department: "CSE"
}));

Used for:
Approval routing


Audit trails


Signature metadata


Personalized dashboard experience



📊 5. Dynamic Dashboards Based on Role
Render different views depending on logged-in role:
switch (user.role) {
  case "Principal":
    render(<PrincipalDashboard />);
    break;
  case "Registrar":
    render(<RegistrarDashboard />);
    break;
  case "HOD-CSE":
    render(<HODDashboard dept="CSE" />);
    break;
  default:
    render(<EmployeeDashboard />);
}


✅ 6. Simulated Approval & Document Routing System
Create documents table:
Table: documents
- id (uuid)
- title (text)
- content (text)
- submitted_by (uuid)
- assigned_to_role (text)
- status: pending | approved | rejected
- signed_at (timestamp)

Use assigned_to_role to route approvals dynamically.

🔐 7. Full Identity Flow Summary
Step
Description
🔑 Auth
Google Sign-In restricted to @hitam.org domain
🧾 Role assignment
Auto-detected via mock DB or email/ID pattern
🗃️ Role persistence
Stored in users table and session/context
🎯 UI rendering
Dynamic dashboards and routing based on user role
📋 Future audit & workflows
Role used in document metadata, approvals, and analytics


🚀 Recommended Tech Stack
Feature
Tool
Auth
Supabase Auth / Firebase
DB
Supabase PG 
UI
React + Tailwind UI
Logic
Node.js or Supabase Edge
Email/Notif
SendGrid / Firebase Mail
Realtime updates
Supabase Realtime


✅ Final Verdict – Best Method:
✅ Use Supabase Auth + Mock Users Table + Email Domain Restriction
 ➕ Add optional fallback logic or admin verification panel
 🔁 Simulate real behavior with dynamic dashboards and workflows



🗃️ Future Usage Support: Securely Persist Session & Role Data
✅ 1. Store User Identity After Login (Once Authenticated)
Upon successful Google Sign-In (with @hitam.org restriction), capture the following:
Field
Description
name
User's full name
email
HITAM Email (e.g., principal@hitam.org)
hitam_id
Unique HITAM ID (e.g., HITAMCSE001)
role
Principal, Registrar, HOD, Faculty, etc.
department
CSE, MECH, ECE, etc.
login_time
Timestamp of login

🔐 Save it to:
users table (PostgreSQL in Supabase or Firestore)


sessionStorage or localStorage for frontend use


Example:
localStorage.setItem("user", JSON.stringify({
  name: "SriChaitanyar",
  email: "22e51a6917@hitam.org",
  role: "Principal",
  hitam_id: "HITAM001",
  department: "Admin"
}));


✅ 2. Enable Reuse Across Core Features
Feature
Role Data Usage
✅ Approvals & Routing
Route documents to assigned_to_role
✅ Signature Stamp Mapping
Auto-stamp: “Signed by Dr. Ravi Kumar, Principal, HITAM001”
✅ Notifications
Auto-send to: registrar@hitam.org, hodcse@hitam.org
✅ Dashboard Analytics
Group data by role, department, status
✅ MoM Auto-fill
Auto-inject name, role, HITAM ID into meeting documents
✅ Audit Trails
“Approved by Principal (HITAM001) on 2025-08-01”
✅ Escalation Rules
If rejected by HOD → auto-escalate to Principal


🧠 3. Auto-Fill System-Wide Fields Using Session Role Info
When generating documents or templates:
Document Section
Auto-Fill Field
Header
name + role + department
Footer
Signed digitally by metadata
Routing Info
assigned_to_role, status
Notification Target
email, role
Comments
name (for attribution)


🎨 Personalized UI (Role-Based Views)
Use the stored role data to dynamically filter and tailor the user interface.
🔁 Example: Conditional UI Rendering in React
const user = JSON.parse(localStorage.getItem("user"));

if (user.role === "Principal") {
  return <PrincipalDashboard />;
}

if (user.role === "Registrar") {
  return <RegistrarDashboard />;
}

if (user.role.includes("HOD")) {
  return <HODDashboard department={user.department} />;
}

return <EmployeeDashboard />;


📑 Filtered Menus and Feature Access
Role
Access to Menu Items
Principal
All documents, escalations, and approval dashboards
Registrar
Department routing templates, compliance views
HOD-CSE
Department-only approvals, schedule meetings
Faculty
Submit, track, view status

🧩 Example Feature Toggles:
if (user.role === "Registrar") {
  showRoutingTemplateManager(); // Only Registrar can access
}

if (user.role === "Principal") {
  enableGlobalEscalationAnalytics();
}


🛡️ Security Best Practices for Role Persistence
Layer
Security Tip
Auth
Only accept verified @hitam.org Google accounts
DB
Use RLS (Row-Level Security) based on user_id/role
Client
Never trust local role alone — always verify from DB
API
Attach user token with email/role claims


✅ Summary
Your system will:
🔐 Safely persist role-based identity


🔁 Reuse this info across workflows, MoM, approvals, and signatures


📩 Route notifications and documents automatically


🧠 Power personalized UI and dynamic dashboards


📊 Improve data tracking, audit, and analytics



:

✅ Google Sign-Up Flow with @hitam.org Restriction
🔹 Step 1: Enable Google Sign-In (Supabase or Firebase)
In Supabase:
Go to Auth → Providers → Google


Enable and configure your OAuth credentials


Add @hitam.org to "Domain Whitelist" (or enforce in backend)



🔍 Step 2: Capture Required User Data on Sign-Up
Field
Description
name
User's full name from Google profile
email
Google account email (*@hitam.org)
hitam_id
Collected via form after first login or popup
role
Assigned via logic or admin dashboard
department
Inferred from HITAM ID or user input
login_time
Captured using Date.now() or server timestamp


✍️ Example: JavaScript Signup Logic (Frontend)
import { supabase } from './client'; // Supabase client

async function handleGoogleSignUp() {
  const { user, session, error } = await supabase.auth.signInWithOAuth({
    provider: 'google',
  });

  if (error) return alert('Login failed.');

  const email = user.email;

  // Restrict to @hitam.org only
  if (!email.endsWith('@hitam.org')) {
    await supabase.auth.signOut();
    return alert("Only HITAM email IDs are allowed.");
  }

  // Open a popup/modal to collect HITAM ID, role, department
  const hitam_id = prompt("Enter your HITAM ID");
  const role = inferRoleFromEmail(email, hitam_id); // or manual selection
  const department = extractDepartment(hitam_id);

  const userData = {
    name: user.user_metadata.full_name,
    email,
    hitam_id,
    role,
    department,
    login_time: new Date().toISOString(),
  };

  // 1️⃣ Save to Firestore or Supabase DB
  await supabase.from("users").insert([userData]);

  // 2️⃣ Save to session/localStorage for UI use
  localStorage.setItem("user", JSON.stringify(userData));
}


🧠 inferRoleFromEmail and extractDepartment Examples
function inferRoleFromEmail(email, hitamId) {
  if (email.includes("principal")) return "Principal";
  if (email.includes("registrar")) return "Registrar";
  if (email.includes("hodcse") || hitamId.startsWith("HITAMCSE")) return "HOD";
  if (email.includes(".cse")) return "Faculty";
  return "Employee";
}

function extractDepartment(hitamId) {
  if (hitamId.includes("CSE")) return "CSE";
  if (hitamId.includes("ECE")) return "ECE";
  if (hitamId.includes("MECH")) return "MECH";
  return "General";
}


✅ Supabase DB Table: users
CREATE TABLE users (
  id uuid PRIMARY KEY DEFAULT gen_random_uuid(),
  name TEXT,
  email TEXT UNIQUE,
  hitam_id TEXT,
  role TEXT,
  department TEXT,
  login_time TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

🔒 Enable RLS (Row Level Security) and apply @hitam.org domain filtering with a policy.

✅ Use Session/Local Storage (Frontend)
const user = {
  name: "SriChaitanya",
  email: "22e51a6917@hitam.org",
  hitam_id: "HITAM001",
  role: "Principal",
  department: "Admin",
  login_time: new Date().toISOString()
};

localStorage.setItem("user", JSON.stringify(user));












