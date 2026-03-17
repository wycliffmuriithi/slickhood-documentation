# Configuring Custom Payment Options


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

![Payment Settings]({{ img }}/paymentSettings.png)

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
   - The system dynamically displays fields based on the selected type. Fill in all the required fields   
   - Currently Supported Payment Types are: 
      a) **M-Pesa** : Refer to the **[M-Pesa Daraja Guide](mpesa_configuration.md)** for detailed instructions on obtaining these credentials.
      b) **FlutterWave** : Refer to the **[FlutterWave Setup Guide](flutterwave_configuration.md)** for detailed instructions on obtaining these credentials.

4. Click on **Create Settings** to save the configuration  
   - This submits the payment parameters to the **Superadmin for review**  
   - All keys are **encrypted before storage**  
   > No one except the landlord can access the original values, not even the Superadmin  

![Add Payment Settings]({{ img }}/addPaymentSetting.png)
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