# Functional Dependencies

PATIENT:
PatientID → FullName, DateOfBirth, Gender, Phone, Email

DOCTOR:
DoctorID → FullName, Specialty, Phone, HireDate

APPOINTMENT:
AppointmentID → PatientID, DoctorID, Date, Time, Status

MEDICAL_RECORD:
RecordID → AppointmentID, Diagnosis, Notes, CreatedDate
AppointmentID → RecordID

PRESCRIPTION:
PrescriptionID → RecordID, Medication, Dosage, Duration

BILL:
BillID → AppointmentID, ConsultationFee, MedicationCost, TotalAmount, Status
AppointmentID → BillID

# Normalization

All relations are in 3NF.
All relations satisfy BCNF.
