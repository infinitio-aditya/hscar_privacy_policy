HS-HRMS PRIVACY POLICY
Last Updated: July 16, 2026

HS-HRMS ("the Application", "we", "us", "our") is a corporate workforce management platform developed by Infinitio Software. This Privacy Policy describes how personal data is collected, used, stored, and protected when employees of registered businesses and organizations ("Users") use the TimeLoom mobile application.

1. COMPANION APP STATUS & ACCOUNT REGISTRATION
HS-HRMS is an enterprise-grade mobile application designed strictly as a reader and companion tool for employees of pre-registered organizations.

No In-App Registration: The Application does not allow public registration, account creation, or purchases for businesses or organizations.
Administrative Setup: Accounts and subscriptions must be created and configured externally by organization/company administrators through our web administration portal. Employees are provided login credentials by their respective employers.
2. DATA WE COLLECT AND PROCESS
To facilitate core workplace operations (such as attendance logging, geofenced check-ins, and task tracking), the Application collects and processes the following types of information:

Identity Information: First name, last name, email address, username, and Employee ID.
Location Information: Real-time geographical coordinates (GPS) collected during check-in/out to verify if an employee is within the organization's authorized geofenced work locations.
Device Information: Device token, OS version, and battery status (for debugging and notification delivery).
Biometric Verification Data (Facial Recognition): Mathematical representation of facial landmarks.
3. BIOMETRIC DATA & ATTENDANCE VERIFICATION
Our Application includes a face-recognition check-in feature to prevent time theft and ensure secure attendance marking. We handle this sensitive data with the highest security standards.

What Face Data is Processed: When you register your face or check-in, the Application accesses your device's camera locally to detect a face using Google ML Kit. It crops the detected face region and processes it locally on the device using a custom TensorFlow Lite facial recognition model (mobile_face_net.tflite) to calculate a 192-dimensional numerical vector (face embedding).

We do NOT collect, upload, share, or store raw photos, images, or video recordings of your face. Only the resulting 192-dimensional numerical coordinates are used.

Storage and Encryption: The numerical face embedding vector is stored locally in the device's secure private cache (via SharedPreferences) and sent securely via an encrypted HTTPS connection (with standard authorization tokens) to your organization's private backend server database.

No Third-Party Sharing: Your face embedding vector is never shared, disclosed, or sold to any third parties under any circumstances. It is strictly used for identity verification within your employing organization.

Data Retention & Deletion:

Device Cache Deletion: The face embedding vector stored in the device's local cache is immediately and completely wiped from the device when the user logs out of the Application.
Server Database Deletion: The face embedding vector is stored on the secure backend database only for as long as the employee is active with the organization. It is immediately and permanently deleted when:
The employer's administrator deletes the employee's profile.
The employee requests account/profile deletion.
The employee is deactivated or terminated by the employer.
4. DATA SECURITY
We implement industry-standard administrative, physical, and technical security measures (including HTTPS transport layer security, JWT authorization, and database access controls) to protect your personal information against unauthorized access, loss, misuse, or alteration.

5. YOUR RIGHTS AND CONTROL
Users and organization administrators have complete control over their personal data:

Access & Portability: You can request details of the personal data held about you.
Correction & Erasure: You can ask your company's administrator to correct or permanently erase your profile, which instantly deletes all associated location logs, session summaries, and biometric face embedding vectors from the backend servers.
6. CONTACT US
If you have any questions or concerns about this Privacy Policy or our data processing practices, please contact us at:

Infinitio Software Support
Email: support@infinitiosoftware.com
Web: https://infinitiosoftware.com
