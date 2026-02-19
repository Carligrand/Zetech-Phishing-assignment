Assignment: Phishing Simulation
Name: Benjamin Gathogo
Student ID: BSE-05-0289/2023
Course: BCT 412 (Information Security/Cybersecurity)
1. Project Overview
This project demonstrates a controlled phishing simulation using the Gophish open-source framework. The goal was to configure a functional SMTP relay, bypass authentication security measures, and successfully deliver a simulated phishing email to a target address.
2. Tool Used
Gophish: A powerful, open-source phishing toolkit used for security awareness training.
SMTP Provider: Gmail (Google Mail).
3. Technical Configuration
To ensure successful delivery, the following technical settings were implemented:
SMTP Host: smtp.gmail.com:587
Sender Address: 004jamestrump@gmail.com
Authentication: Implemented Google App Passwords. Because Google blocks "Less Secure Apps," I enabled 2-Step Verification and generated a unique 16-character application key to bypass the 535 5.7.8 Authentication Error.
Payload: A direct hyperlink to the official university domain (https://zetech.ac.ke) was used to increase the perceived legitimacy of the email and avoid being flagged by simple URL reputation filters.
4. Implementation Steps
Sending Profile Setup: Configured the SMTP relay with the Gmail App Password and verified the connection.
Email Template Creation: Designed a template based on Social Engineering principles (Urgency and Authority), masquerading as an "IT Support" security update.
Alpha Testing: Conducted a successful test send to the sender's own address to verify that formatting and delivery were functional.
Campaign Launch: Created and triggered the final campaign targeting the lecturer's email address.
5. Evidence (Screenshots)
5.1 Successful Delivery Test
Below is an image of a successful test fake email sent from 004jamestrump@gmail.com to verify that the SMTP configuration was correct and bypassing Gmail's security blocks.
<img width="828" height="499" alt="Successful Test Email" src="https://github.com/user-attachments/assets/ab091111-6066-432c-9317-905661e9d7ac" />
5.2 Sending Profile Configuration
Below is a screenshot of the final Sending Profile used for the campaign. Note the use of the full email address as the username and the TLS port (587) for secure transmission.
<img width="828" height="949" alt="Gophish Sending Profile" src="https://github.com/user-attachments/assets/203ef3ff-dff9-44bf-8ce1-6e51d7d24c25" />
6. Conclusion
The simulation was successful. The Gophish framework was able to authenticate via the Gmail SMTP relay and deliver the message. This exercise highlights the importance of multi-factor authentication and the ease with which attackers can use legitimate SMTP providers to conduct social engineering campaigns.
