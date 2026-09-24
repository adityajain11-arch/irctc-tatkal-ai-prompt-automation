# ⚡ High-Speed IRCTC Tatkal Ticket Booking Automation Prompt

An optimized, end-to-end AI agent prompt designed to automate time-critical web form interactions, session re-use, and instant checkout for Tatkal train bookings.

---

## 🎯 Objective & Problem Statement
Human booking during Tatkal opening hours (10:00 AM / 11:00 AM IST) often fails due to network delays, form typing speed, and session timeouts. This workflow leverages browser session reuse and precise scheduled execution (`10:59:30 AM IST`) to complete the booking within seconds.

---

## 📝 The Master Prompt

```text
Book ONE confirmed IRCTC Tatkal ticket end to end:

Train: 19034 Gujarat Queen
From and boarding station: Ahmedabad Junction (ADI)
To: Vadodara Junction (BRC)
Journey Date: 24 September 2026
Expected departure/arrival: 18:10–20:08, Second Sitting (2S) in IRCTC's displayed schedule
Class/Quota: 2S, Tatkal
Passenger: [Passenger Name]
Payment: IRCTC eWallet
Maximum authorized payment: ₹200 TOTAL, including all fees.

Instructions:
1. Execute the exact journey search and booking to attempt payment within ₹200 without asking for another confirmation. My wallet balance has already been verified.
2. Reuse current IRCTC browser tab and signed-in session.
3. At 11:00 AM IST, refresh availability using normal site controls and proceed as soon as booking opens.
4. If IRCTC booking service has not started, retry through normal controls without excessive refreshing.
5. Report success only after IRCTC displays a PNR and confirmed booking status. Give me the PNR, coach, and seat details if assigned, journey details, and amount charged. If unsuccessful, state the exact blocker and whether any payment was deducted.

Schedule / Execution Command: Run at 10:59.5 and start the process.
