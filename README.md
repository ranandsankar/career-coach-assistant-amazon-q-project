# Amazon Q Business – Career Coaching Assistant

This project implements a Career Coaching Assistant Q App using **Amazon Q Business**, as part of the Udacity "Building Generative AI Apps with Amazon Q Business" course.

The application allows:
- Uploading a CV and job description
- Performing skill gap analysis
- Generating personalized training recommendations using S3 + PDF catalogs
- Creating a learning schedule
- Allowing coaches to provide custom notes
- Enforcing document-level security using ACL rules
- Managing restricted vs public catalogs

---

## 📁 Project Structure
q-app/
prompts/
acl/
screenshots/
docs/



Each folder supports a specific part of the project.

---

## 🎯 Features Implemented

- ✔ Q App with 2 input cards (CV, JD)
- ✔ Skill Gap Analysis output card
- ✔ Training Recommendations using S3 + PDF catalogs
- ✔ Learning Schedule generator
- ✔ Coach Notes input card
- ✔ Data Source integration (S3 + PDF)
- ✔ Daily sync for S3 catalog
- ✔ ACL-based document access control
- ✔ Blocked keyword guardrails
- ✔ Verified and shared Q App

---

## 📸 Screenshots Required (place in `q-app/screenshots/`)

- Q App UI  
- Data sources list  
- Blocked words configuration  
- ACL success (approved user access)  
- ACL denial (unapproved user restricted content hidden)

---

## 📚 Documentation Included

- Architecture overview  
- Data source configuration  
- ACL & security setup  
- Guardrails configuration  

---
