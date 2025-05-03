# Experiment 1: Entity-Relationship (ER) Diagram

## 🎯 Objective:
To understand and apply the concepts of ER modeling by creating an ER diagram for a real-world application.

## 📚 Purpose:
The purpose of this workshop is to gain hands-on experience in designing ER diagrams that visually represent the structure of a database including entities, relationships, attributes, and constraints.



---

### 🔹 Scenario  Hospital Database
Design a database for patient management, appointments, medical records, and billing.

*User Requirements:*
- Patient details including contact and insurance.
- Doctors and their departments, contact info, specialization.
- Appointments with reason, time, patient-doctor link.
- Medical records with treatments, diagnosis, test results.
- Billing and payment details for each appointment.

---

## 📝 Tasks:
1. Identify entities, relationships, and attributes.
2. Draw the ER diagram using any tool (draw.io, dbdiagram.io, hand-drawn and scanned).
3. Include:
   - Cardinality & participation constraints
   - Prerequisites for Billing for Hospital
4. Explain:
   - Why you chose the entities and relationships.
   - How you modeled prerequisites or billing.

# ER Diagram Submission 
# Name: HIRUTHIK SUDHAKAR
# Reg.no:212223240054
# Scenario Chosen:
HOSPITAL
## ER Diagram:
![image](https://github.com/user-attachments/assets/9498e45f-92bd-4812-a0ad-94d56445ce8c)


## Entities and Attributes:


1. Patient
   - patientID (PK)
   - FullName
   - DOB
   - Gender
   - Address
   - Phone number
   - Email
   - Insurance details

2. Doctor
   - DoctorID (PK)
   - FullName
   - Specialization
   - Phone
   - Email
   - Workschedule

3. Appointment
   - AppointmentID (PK)
   - AppointmentDate
   - Appointment Time
   - Reason
   - Notes
   - DoctorID (FK)
   - PatientID (FK)

4. Medical Record
   - RecordID (PK)
   - Diagnosis
   - Medications
   - Treatments
   - TestResults
   - Notes
   - DoctorID (FK)
   - PatientID (FK)

5. Department
   - DeptID (PK)
   - DeptName
   - DeptHead

6. Billing
   - BillID (PK)
   - TotalAmount
   - BillDate
   - appointmentID (FK)

7. Payment
   - paymentID (PK)
   - PaymentDate
   - amountPaid
   - paymentMethod
   - paymentStatus
   - BILLID (FK)


Relationships:

- Patient — books —> Appointment
- Patient — has record —> Medical Record
- Doctor — records for —> Medical Record
- Doctor — works in —> Department
- Doctor — consults —> Appointment
- Appointment — generates —> Billing
- Payment — pays for —> Billing


## RESULT
Thus, the Entity-Relationship (ER) Diagram have been created successfully.
