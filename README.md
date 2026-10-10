# Applicant Tracking System (ATS) - Project Documentation

## 1. Gitflow Branching Strategy
This repository implements the standard Gitflow workflow:
* **main**: Contains production-ready code.
* **develop**: Main integration branch for features.
* **feature/**: Individual branches created from develop for developing specific application features.

---

## 2. User Stories & Gherkin Scenarios

### Story 1: Submit Job Application
* **User Story:** As a job seeker, I want to submit my job application with my resume so that I can apply for a position.
* **Gherkin Scenario:**
  ```gherkin
  Given a job seeker is on the job details page
  When they upload their resume and click the "Apply Now" button
  Then their application should be successfully submitted and saved in the system

### Story 2: Update Application Status
* **User Story:** As an HR manager, I want to update a candidate's application status so that they know if they are shortlisted or rejected.
* **Gherkin Scenario:**
  ```gherkin
Given the HR manager is viewing a candidate's application
When they change the status to "Shortlisted" and save it
Then the candidate's status should be updated and an email notification should be triggered

### Story 3: View Applied Jobs History
* **User Story:** As a job seeker, I want to view a list of all the jobs I have applied for so that I can track my application progress.
* **Gherkin Scenario:**
  ```gherkin
Given the job seeker is logged into their account
When they navigate to the "My Applications" section
Then they should see a list of all jobs they have applied for along with their current status

### Story 4: Create New Job Posting
* **User Story:** As an HR manager, I want to post a new job opening so that candidates can view it and apply.
* **Gherkin Scenario:**
  ```gherkin
Given the HR manager is on the job creation dashboard
When they fill in the job title, description, and requirements and click "Publish"
Then the new job listing should appear on the public jobs portal
