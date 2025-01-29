 ## Printing module 

 The Printing module in Frappe helps you create and print documents like invoices, orders, quotes, and delivery notes. It allows you to customize how these documents look when printed, such as adding your company logo, adjusting the layout, and choosing fonts.

List of doctypes:

![image](https://github.com/user-attachments/assets/73a2f9b2-1987-4f88-bc06-ef206d6c235f)



### 1. Letter Head
   - **Purpose**: Used to define the layout and design for the letterhead of printed documents (like invoices, orders, etc.).
   - **Fields**: 
     - Letterhead Name
     - Header
     - Footer
     - Font
     - Image (e.g., company logo)
     - Other styling elements

### 2. Print Format
   - **Purpose**: Represents the design/layout for printing documents like sales invoices, purchase orders, quotations, etc.
   - **Fields**: 
     - Print Format Name
     - Document Type (e.g., Sales Invoice)
     - Template (HTML for design)
     - CSS (for styling)
     - Jinja syntax to insert dynamic data

### 3. Network Printer Settings
   - **Purpose**: Configures the settings for network printers that are integrated with the Frappe system. This allows printing directly from Frappe to networked printers.
   - **Fields**: 
     - Printer Name
     - Printer Type
     - IP Address
     - Port
     - Printer Settings (e.g., resolution, paper size)

### 4. Print Settings
   - **Purpose**: Stores system-level settings for printing, such as paper size, print orientation, and other global print-related preferences.
   - **Fields**: 
     - Paper Size (A4, Letter)
     - Print Orientation (Portrait, Landscape)
     - Margins
     - Printer Configuration

### 5. Print Style
   - **Purpose**: Allows defining custom print styles to be applied to specific print formats or document types.
   - **Fields**: 
     - Style Name
     - CSS (for styling elements like fonts, colors, and other visual settings)

### 6. Print Format Field Style
   - **Purpose**: Used to define the style for individual fields (e.g., how the data in a field should appear when printed).
   - **Fields**: 
     - Field Name
     - Font Style
     - Font Size
     - Color
     - Alignment
     - Background
     - Other visual formatting

### 7. Print Heading
   - **Purpose**: Defines the headings or titles that should appear on printed documents.
   - **Fields**: 
     - Heading Text
     - Font Style
     - Alignment
     - Placement on the page
