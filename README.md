# Ustool App — Privacy Policy

**Effective date:** 1 November 2025

> **Short version (TL;DR):** We collect only the details we need to run a restaurant order and dispatch workflow. That includes staff account information, restaurant profile details, order metadata, driver availability and the push-notification tokens needed to alert teams in real time. We do not track precise device location or sell personal data. You can ask us to access, correct, delete or export your information, and you can disable notifications from your device settings.

---

## 1) Who we are

**Ustool** (the “App”) is provided by **[Ahmad Amireh]**. In this policy, “we”, “us” and “our” refer to this provider.

**Contact for privacy matters:**

* Email: **[ahmad.ali.amireh@gmail.com](mailto:ahmad.ali.amireh@gmail.com)**

Depending on how the App is used, we may act as a **data controller** (e.g., for driver/admin accounts and platform operations) and/or a **data processor** on behalf of restaurants that use Ustool (e.g., order information entered by a restaurant). Where a restaurant inputs its customers’ details, that restaurant is usually the **controller** for those customer records; Ustool acts as their **processor**.

---

## 2) Scope of this policy

This policy applies to your use of the Ustool mobile application and related services, support channels and websites that link to it (together, the “Services”). It covers information we collect from:

* **Restaurant staff/admins** operating the order management views
* **Drivers** who receive and action delivery assignments
* **End customers** whose information may be entered by a restaurant to fulfil an order

---

## 3) Personal data we collect

We collect different information depending on your role and how you interact with the Services.

### A) Data collected from **all users**

* **Account profile:** Firebase user ID, name, email address, optional phone number, and assigned role (restaurant staff, admin or driver).
* **Authentication details:** session status derived from Firebase Authentication to confirm you are signed in before we load or update profile data.
* **Push-notification tokens:** Expo push tokens tied to your account and locale so we can deliver operational alerts, stored in Firestore with timestamps.

### B) Data related to **restaurant staff/admins**

* **Restaurant profile:** restaurant name, phone number, address and join date.
* **Order activity:** records you create in the orders collection, including code, restaurant identifiers, preparation time, delivery region, creator ID and timestamps.

### C) Data related to **drivers**

* **Availability:** driver status (online/offline) that you can toggle in your profile and that we validate via Firestore rules.
* **Assignment history:** which driver was assigned to an order and related lifecycle timestamps (assigned, accepted, picked up, delivered) maintained on the order document.

> We do **not** collect precise GPS location or background location trails. Driver state is limited to availability toggles and order milestone timestamps, and we do not request location permissions.

### D) Data related to **end customers** (entered by restaurants)

* **Order metadata:** human-readable code, restaurant details, preparation time, delivery region ID, delivery fee (if any) and lifecycle timestamps used to fulfil and audit orders.

Restaurants are instructed not to enter special-category data (e.g., health or religious details) in free-text fields. If such data is added in error, please contact us so we can address it.

---

## 4) How and why we use your data (purposes & lawful bases)

Under UK/EU GDPR and similar laws, we rely on the following bases:

* **Contractual necessity** — to operate the Services you request:
  * authenticate accounts and load the correct restaurant profile before showing data or letting you create orders.
  * generate and store order codes, regions and preparation times so teams can fulfil requests.
  * send operational notifications (new order, assignment updates) using your registered push token.
* **Legitimate interests** — to secure and improve the platform:
  * enforce role-based access controls and audit changes through Firestore security rules.
  * monitor error conditions (e.g., failed notification registration) to maintain service reliability.
* **Consent** — for any optional communications (such as marketing) we may offer in the future. You can withdraw consent at any time.
* **Legal obligations** — to comply with record-keeping, tax or law-enforcement requirements that apply to the restaurants or to us.

---

## 5) Location services (drivers)

The current Ustool app does **not** request or store precise location data. Driver-focused functionality records whether you are online or offline and updates order status timestamps as you progress through a job. If we introduce location tracking in the future, we will update this policy and ask for the appropriate permissions.

---

## 6) Push notifications

We use Expo Notifications (APNs/FCM) to deliver operational alerts such as new orders or assignment updates. The app requests notification permission, registers a push token and stores it alongside your user ID and locale to route messages correctly. You can change notification preferences or disable them entirely in your device settings, though doing so may affect timely order handling.

---

## 7) Cookies and similar technologies

The mobile app does not use browser cookies. We rely on local state and secure storage provided by the device operating system and Firebase SDKs to keep you signed in and to deliver notifications. If you access any accompanying web dashboard, additional cookie notices may apply there.

---

## 8) Data sharing and recipients

We share data only as needed for the purposes above:

* **Restaurants & authorised staff:** order details and driver assignments visible to users linked to the same restaurant, controlled by Firestore security rules.
* **Service providers (processors):**
  * **Google Firebase** (Authentication, Firestore) hosts account, restaurant and order records in the `nam5` Firestore region.
  * **Expo / Apple APNs / Firebase Cloud Messaging** deliver push notifications using the tokens we register.
* **Legal & compliance:** if required by law, regulation or to protect safety and security.
* **Business transfers:** if we undergo a merger, acquisition or asset sale.

We do **not** sell personal data.

---

## 9) International data transfers

Firebase may process data in countries outside your own (including the United States, where the `nam5` Firestore region is hosted). When we transfer personal data internationally, we rely on lawful mechanisms such as adequacy decisions or standard contractual clauses.

---

## 10) Data retention

We keep personal data only for as long as needed to operate the platform and meet legal requirements:

* **Accounts and restaurant profiles:** retained while your organisation actively uses the Service and deleted or anonymised within a reasonable period after closure.
* **Order records:** retained to support operational history, reconciliation and legal obligations; typically no longer than required by the contracting restaurant’s policies.
* **Push tokens:** refreshed regularly and removed when you revoke permissions, sign out or delete your account.

We may anonymise order metrics for analytics; anonymised data is not considered personal data.

---

## 11) Security

We use administrative, technical and organisational measures to protect personal data, including Firebase Authentication, role-based access controls, and Firestore security rules that restrict who can read or update particular documents. While no system is perfectly secure, we monitor for errors and will notify affected users and regulators when required by law.

---

## 12) Your rights

Depending on your jurisdiction, you may have the right to access, correct, delete, restrict or object to processing of your personal data, and to data portability. If we process data based on consent, you may withdraw it at any time. **California (CCPA/CPRA):** you may have rights to know, delete and correct personal information, and to opt out of “sale” or “sharing” for cross-context behavioural advertising. We do not sell personal information. To exercise your rights or appeal a decision, contact us at **[ahmad.ali.amireh@gmail.com](mailto:ahmad.ali.amireh@gmail.com)**. Where we process data on behalf of a restaurant, we may refer your request to that restaurant.

---

## 13) Your choices & controls

* **Notifications:** manage push permissions in your device settings.
* **Account details:** update your profile or contact support to request changes.
* **Account deletion:** contact us (or your restaurant administrator) to request deletion of your account and associated records.

---

## 14) Children

The Services are not directed to children. We do not knowingly collect personal data from children. If you believe a child’s data has been provided to us, please contact us so we can take appropriate action.

---

## 15) Third-party links

The App may link to third-party sites or services. Their privacy practices are governed by their own policies. Please review those policies before using their services.

---

## 16) Changes to this policy

We may update this policy from time to time. We will post the new version in the App and update the effective date. Material changes may also be notified via in-app message or email where appropriate.

---

## 17) How to contact us

If you have questions, concerns or requests regarding your data, contact **[ahmad.ali.amireh@gmail.com](mailto:ahmad.ali.amireh@gmail.com)**. You may also have the right to complain to your local data protection authority.

---

## Annex A — Role-specific notices & permissions

### Restaurant staff & admins

* **Restaurant profile data:** we load and display the restaurant name, phone, address and join date tied to your account.
* **Order history:** orders you create include restaurant identifiers, preparation details and creator ID for operational tracking.

### Drivers

* **Availability toggles:** you can set your status to online/offline; Firestore rules ensure only you or authorised admins can change this field.
* **Order workflow:** assignment and completion timestamps are recorded on each order for accountability and customer updates.

### End customers

* **Order metadata:** restaurants may store order codes, restaurant identifiers, delivery regions and fulfilment timestamps to coordinate your delivery.

---

## Annex B — Service providers (illustrative)

* **Google Firebase (Authentication, Firestore)** — account, restaurant and order storage; infrastructure hosting in region `nam5` (Google Cloud).
* **Expo Push Service / Apple Push Notification service (APNs) / Firebase Cloud Messaging (FCM)** — delivery of push notifications to devices.

> **Note:** The exact list of providers may change as we improve the Service. We will update this annex or our website accordingly.

---

## Legal notice

This document is provided for general information and does not constitute legal advice. Privacy laws vary by jurisdiction. Please consult your legal adviser to tailor this policy to your specific circumstances.
