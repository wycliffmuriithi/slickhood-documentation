# Configuring Custom Payment Options

> **Disclaimer:** This guide applies to **SlickHood version 1.0.[COMMIT_HASH]**.  

This guide explains how **Landlords** and **Property Managers** can configure payment options for their properties on [SlickHood](https://slickhood.com/login).

SlickHood supports multiple payment methods, including:
- **Mobile Money (M-Pesa)**
- **Card Payments (Flutterwave)**
- **Manual Payments (recorded by property managers)**

---

## 1. Accessing Payment Settings

To begin configuring payment options:

1. Log in to your [SlickHood](https://slickhood.com/login) account  
2. Navigate to your **User Profile Menu**  
3. Click on **Payment Settings**

Below is the Payment Settings entry point:

<img width="251" height="221" alt="image" src="https://github.com/user-attachments/assets/8469a3e1-b168-4572-8af0-6c0a8258829d" />





> **Note:** Payment settings are tied to your profile. Ensure you are logged in as the correct landlord or property manager account before making changes.

---

## 2. Adding a Payment Configuration

On the **Payment Configuration** page, a landlord can add either **M-Pesa** or **Flutterwave** configuration.

### Step-by-step:

1. Click on the **Add Settings** button  
   - This opens a dialog that captures the payment option details  

2. Fill in the **Name of the Payment Option**  
   - Use a descriptive name  
   - Example: `Jabali Properties M-Pesa Paybill`

3. Select the **Payment Type**  
   - The system dynamically displays fields based on the selected type  

<img width="514" height="346" alt="image" src="https://github.com/user-attachments/assets/8bf425ad-d971-4123-919d-f5bb07ff5d51" />


---

### M-Pesa Configuration

For **M-Pesa**, there are four required fields:

a) **M-Pesa Paybill**  
   - 6-digit M-Pesa Paybill code  

b) **M-Pesa Consumer Key**  
   - A generated key from the Daraja platform used for API authentication  

c) **M-Pesa Consumer Secret**  
   - Paired with the Consumer Key  
   - Also obtained from the Daraja platform  

d) **M-Pesa STK Passkey**  
   - Used to initiate STK push requests (payment prompts to tenant phone numbers)  


<img width="514" height="589" alt="Screenshot From 2026-03-17 12-40-54" src="https://github.com/user-attachments/assets/647b4113-9d88-4881-9787-9d487f2b72d1" />


> Refer to the **M-Pesa Daraja Guide** for detailed instructions on obtaining these credentials.

---

### Flutterwave Configuration

For **Flutterwave**, there are three required fields:

a) **Flutterwave Public Key**  
   - Authentication key provided in your Flutterwave account  

b) **Flutterwave Encryption Key**  
   - Used to secure transaction payloads  

c) **Flutterwave Secret Key**  
   - Paired with the Public Key **Must never be exposed publicly**  
   
<img width="514" height="533" alt="Screenshot From 2026-03-17 12-41-42" src="https://github.com/user-attachments/assets/759ccc83-824e-41fa-b797-e8963ae24585" />
 

---

4. Click on **Create Settings** to save the configuration  

- This submits the payment parameters to the **Superadmin for review**  
- All keys are **encrypted before storage**  
> No one except the landlord can access the original values, not even the Superadmin  

---

## 3. Verification Process

After submission:

- The configuration undergoes a **verification process**  
- This ensures the provided credentials are valid and can successfully process transactions  

Once verified:

- The Payment Option will display a **Verified Badge**  
- It becomes available for **assignment to properties**

---

## 4. Assigning Payment Settings to Properties

Once verified:

1. Navigate to **Property Management**  
2. Select the relevant property  
3. Assign the verified payment option  

> **Important:** Only verified payment configurations can be used for live transactions.

---