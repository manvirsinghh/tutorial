# Contacts module



The Contacts module in Frappe is used to store and manage information about individuals or organizations your business interacts with, such as customers, suppliers, and leads. It helps track details like names, addresses, emails, phone numbers, and communication history, and allows you to link contacts to other business records.
  
![image](https://github.com/user-attachments/assets/6e612aa3-a5da-4766-b174-f37d986fd3cb)

Following are the doctypes of contacs module

1. **Contact**
   - **Purpose**: Represents an individual or entity you interact with (e.g., customers, suppliers).
   - **Fields**:
     - **Name**: The name of the contact.
     - **Email**: Email address.
     - **Linked to Customer/Supplier**: If the contact is related to a Customer or Supplier.
     - **Address**: Address associated with the contact.
     - **Salutation**: Prefix (e.g., Mr., Mrs.).
     - **Gender**: Gender of the contact (optional).
     - **Communication Preference**: Preferred method of communication (e.g., email, phone).

2. **Address**
   - **Purpose**: Stores physical address information.
   - **Fields**:
     - **Address Line 1**: Primary address line.
     - **Address Line 2**: Additional address information.
     - **City**: City where the contact is located.
     - **State**: State or province.
     - **Country**: Country of the contact.
     - **Pincode**: Postal code.
     - **Address Type**: Type of address (e.g., Billing, Shipping).

3. **Contact Phone**
   - **Purpose**: Stores phone-related information for contacts.
   - **Fields**:
     - **Phone Number**: The phone number associated with the contact.
     - **Phone Type**: Type of phone (e.g., Mobile, Landline).
     - **Country Code**: Country-specific code (e.g., +1 for the USA).
     - **Is Primary**: Whether this phone number is the primary one for the contact.

4. **Contact Email**
   - **Purpose**: Stores email-related information for contacts.
   - **Fields**:
     - **Email Address**: The email associated with the contact.
     - **Email Type**: Type of email (e.g., Personal, Work).
     - **Is Primary**: Whether this email is the primary one for the contact.

5. **Address Template**
   - **Purpose**: Defines a template for address formatting.
   - **Fields**:
     - **Template Name**: Name of the address template.
     - **Template Type**: Type of template (e.g., Shipping Address, Billing Address).
     - **Address Structure**: Format or predefined structure for the address.

6. **Gender**
   - **Purpose**: Stores the gender options for contacts.
   - **Fields**:
     - **Gender**: The gender option (e.g., Male, Female, Other).

7. **Salutation**
   - **Purpose**: Stores prefixes or salutations for contacts.
   - **Fields**:
     - **Salutation**: The salutation for a contact (e.g., Mr., Mrs., Dr., Prof.).
