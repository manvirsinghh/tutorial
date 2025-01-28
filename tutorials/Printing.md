## Printing module

Frappe framework has support for generating print formats for documents and also convert them into PDF. Frappe uses Jinja as the templating language for print formats.


It has following doctypes:-

![image](https://github.com/user-attachments/assets/795948b2-e881-4528-9c12-9d62310dbb98)


### 1. **Letterhead**

**Purpose**: Letterhead is used to customize the top portion of the printed document to reflect your company's branding.

**Fields**:
- **Name**: The name of the letterhead.
- **Letterhead Type**: Specifies whether it's for print or email.
- **Content**: The content of the letterhead, including the logo, company name, and contact details.
- **Is Standard**: Marks the letterhead as standard for all documents.

**Steps**:
1. Go to **Letterhead** in Frappe.
2. Create a new letterhead, add your company’s details and logo.
3. Save the configuration.

---

### 2. **Print Format**

**Purpose**: Print Format defines the layout and structure of the printed document, including sections like the header, body, and footer.

**Fields**:
- **Name**: The name of the print format.
- **Document Type**: The type of document this format applies to (e.g., `Sales Invoice`).
- **Is Standard**: Whether this format should be set as the default for all users.
- **Print Style**: The style used for printing (e.g., custom CSS).
- **Letterhead**: The letterhead to be used for this print format.

**Steps**:
1. Go to **Print Format** in Frappe.
2. Create a new print format and select the document type.
3. Add HTML, Jinja code, or placeholders to customize the layout.
4. Save and set this print format as the default if needed.

---

### 3. **Network Printer Settings**

**Purpose**: Configure network printers for printing directly from Frappe.

**Fields**:
- **Name**: The name of the printer.
- **Printer Type**: The type of printer (e.g., Network Printer).
- **Printer Address**: The IP address or network location of the printer.
- **Print Server**: Optionally configure a print server if required.

**Steps**:
1. Go to **Network Printer Settings**.
2. Add the printer details (IP address or network path).
3. Save the configuration.

---

### 4. **Print Style**

**Purpose**: A Print Style determines the formatting of the print output, such as CSS styles that define fonts, colors, and visual elements.

**Fields**:
- **Name**: The name of the print style.
- **Style Type**: Either use a default style or create a custom style.
- **CSS**: Define custom CSS to adjust the appearance of the document when printed.

**Steps**:
1. Go to **Print Style** in Frappe.
2. Create a new print style or use an existing one.
3. Add or modify CSS for visual adjustments.
4. Save the changes.

---

### 5. **Print Format File Template**

**Purpose**: This is the HTML or Jinja file that defines how the print format should be rendered, acting as a template for generating the printed document.

**Fields**:
- **Name**: The name of the template file.
- **Content**: HTML content with placeholders to dynamically render values.
- **Is Default**: Whether this template is the default for the document type.

**Steps**:
1. Go to **Print Format File Template**.
2. Create a new template with HTML and Jinja code for dynamic rendering.
3. Save and link it to a print format.

---

### 6. **Print Heading**

**Purpose**: A print heading allows you to define a title or header for your printed document, typically used in print formats to display a section heading.

**Fields**:
- **Name**: The name of the print heading.
- **Heading**: The text or title to display.
- **Is Standard**: Whether the heading is standard for all documents.

**Steps**:
1. Go to **Print Heading**.
2. Create a new heading with the appropriate title.
3. Link the heading to the corresponding print format or document.

---

### Conclusion

By configuring these print settings, you can create highly customized, professional-looking documents in Frappe. These features allow you to:
- Set up letterheads for branding.
- Define flexible print formats.
- Manage printer settings and network printers.
- Customize print styles using CSS.
- Use templates for rendering print formats dynamically.
- Add print headings to improve document clarity.
