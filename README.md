### Role: Salesforce Administrator
### Rael kapanga
### Location: Kentucky, United States
### Industry: Formalwear Rentals & Event Planning

 # Project Overview
Designed and configured a Salesforce Lightning org to manage the full rental lifecycle for suits, tuxedos, and wedding events. The goal was to automate manual processes, improve cross‑team collaboration, secure customer data, and enhance reporting visibility for management decisions.

Geno Formal Affair uses this org to manage customers, rentals, pricing, and discount approvals, while maintaining efficient communication between the Sales, Marketing, and Customer Service departments.

## System Design & Configuration
### Category	Key Deliverables
- **Data Model	Custom object** Rental linked to Account (Master–Detail) and Contact (Lookup). Separate record types for Suit Rentals and Tuxedo Rentals with unique page layouts.

- **Automation (Flows)	Four Record‑Triggered Flows**: (1) auto‑set rental status to Order Placed, (2) mark Past Due after rental duration, (3) update to Returned, (4) send overdue email reminders.

- **Approvals	Two Approval Processes:** (1) Rental Extension (>7 days) requiring Manager approval, (2) Wedding Discount (>15%) requiring Manager authorization and email alerts.

- **Validation Rules**	Enforced date ordering, rental duration limits, and event pickup logic to prevent data corruption.

- **Security Model	Role Hierarchy** (CEO → Manager → Sales → Marketing → Support). OWD: Account = Private; Rentals = Controlled by Parent; Products = Read Only. Sharing Rules grant read access to Marketing and Customer Service.

-**Reporting & Dashboards**	Five custom reports (Past Due, Ready for Pickup, Returned Rentals, Placed Orders, Most Rented Style) and one consolidated Rental Operations Dashboard.

- **Profiles & Permissions**	Custom profiles for CEO, Manager, Sales, Marketing, and Customer Service. Used Permission Sets for targeted access to reports and admin features.

## Business Impact
- Automated 90% of rental lifecycle updates, reducing manual effort and errors.
- Enabled cross‑team visibility through structured role and sharing rules.
- Improved customer response time with automated emails and dashboard insights.
- Provided actionable data for management to forecast rental volume and trends.
## Tools & Features Used
- Salesforce Flows
- Approval Processes
-  Validation Rules
- Record Types
-  Sharing Rules
-  Reports & Dashboards
-  Field‑Level Security
-  Permission Sets
-  Email Alerts
