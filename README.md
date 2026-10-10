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

Updating from feature branch
