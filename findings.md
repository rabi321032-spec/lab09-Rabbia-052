
# MediTrack – Validation Findings

## Purpose
This document lists the problems found during the validation of the MediTrack SRS.

## Findings

### Finding 1: Conflicting Appointment Duration
**Requirement:** R-04, R-05

R-04 says every appointment is 15 minutes, but R-05 allows doctors to set appointments between 10 and 30 minutes.

**Problem:** These requirements conflict.

**Suggestion:** Clearly define whether doctors can change the default appointment duration.

### Finding 2: Vague Response Time
**Requirement:** R-02

The word "quickly" does not give a measurable response time.

**Problem:** We cannot properly test system speed.

**Suggestion:** Specify a response time, such as within 2 seconds.

### Finding 3: Double Booking Risk
**Requirement:** R-03

The requirement does not explain how simultaneous booking requests will be handled.

**Problem:** Two patients might receive the same appointment.

**Suggestion:** Add a rule to prevent two patients from booking the same doctor and time slot.

### Finding 4: Unclear Reminder System
**Requirement:** R-06

The requirement does not specify when reminders will be sent.

**Problem:** Patients may still forget their appointments.

**Suggestion:** Define reminder timing, such as 24 hours before the appointment.

### Finding 5: Weak Security Details
**Requirement:** R-09

The word "securely" does not explain how patient records will be protected.

**Problem:** Private medical information may be exposed.

**Suggestion:** Specify access permissions and security measures.

### Finding 6: Accessibility Problem
**Requirement:** R-08

The requirement says user-friendly for all age groups but gives no specific accessibility features.

**Problem:** Elderly patients may face difficulty using the system.

**Suggestion:** Include simple navigation, readable text and easy booking options.

### Finding 7: Emergency Walk-in Handling
**Requirement:** R-10

The requirement allows walk-in bookings but does not explain how emergency patients will be handled.

**Problem:** Emergency patients may face unnecessary delays.

**Suggestion:** Define an emergency appointment priority process.

### Finding 8: Busy Monday Morning
**Requirement:** Missing requirement

The SRS does not explain how the system will handle heavy booking traffic on Monday mornings.

**Problem:** The system may become slow during busy hours.

**Suggestion:** Add measurable peak-load performance requirements.

### Finding 9: Unclear Cancellation Process
**Requirement:** R-07

The requirement combines cancellation, schedule updating and receptionist notification.

**Problem:** It is difficult to validate each action separately.

**Suggestion:** Divide it into separate requirements and define the update and notification timing.

## Conclusion

The MediTrack SRS has several problems related to clarity, consistency, security, performance and completeness. These problems should be fixed before the clinic signs the contract.
