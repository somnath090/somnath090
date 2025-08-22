As a hotel maintenance user, 

I want to manage contact information for a hotel 

so that I can maintain accurate phone numbers, fax numbers, manager information, and communication details for distribution systems.

The Contact section is part of the General tab in the Hotel Maintenance application and manages all contact-related information for hotels. This section handles phone numbers, fax numbers, manager details, and other communication information organized into logical groupings.

Backend Logic:

Data is managed through the InfosetContacts class which contains contact-specific information

The InfosetContactsBuilder populates data from multiple sources:

Primary phone from hotel.getPrimaryPhoneNumber()

Other phones (toll-free, fax, sales fax, call forwarding) from hotel.getContactInfo().getContactNumbers()

Manager information from hotel.getHotelManagement()

Phone numbers are handled through PhoneBean objects with components: international dialing code, area code, number, extension

Manager names are constructed by combining first and last names from the hotel management data

Data is persisted through the DialogControllerSaveContacts controller using the DialogContactsForm

Frontend Logic:

The contact information is displayed in a read-only format organized into two fieldsets: "Phone & Fax" and "Managers"

Users can edit contact information through a modal dialog with accordion-style sections

The dialog contains structured input fields for phone components and manager names

Phone number validation includes international dialing code autocomplete functionality

Manager fields are read-only and prevent copy/paste operations

Data Fields and Validations:

Phone & Fax Section:

Phone (phone)

Type: PhoneBean with components

Components: International Dialing Code (3 chars), Area Code (3 chars), Number (10 chars), Extension (4 chars)

Display: Formatted phone number in infoset, structured input fields in dialog

Validation: Phone format validation, optional field

Toll-free Number (tollfreePhone)

Type: PhoneBean with components

Components: International Dialing Code (3 chars), Area Code (3 chars), Number (10 chars), Extension (4 chars)

Display: Formatted phone number in infoset, structured input fields in dialog

Validation: Phone format validation, optional field

Fax (fax)

Type: PhoneBean with components

Components: International Dialing Code (3 chars), Area Code (3 chars), Number (10 chars), Extension (4 chars)

Display: Formatted phone number in infoset, structured input fields in dialog

Validation: Phone format validation, optional field

Sales Fax (salesFax)

Type: PhoneBean with components

Components: International Dialing Code (3 chars), Area Code (3 chars), Number (10 chars), Extension (4 chars)

Display: Formatted phone number in infoset, structured input fields in dialog

Validation: Phone format validation, optional field

ResConnect (Call Forwarding) (callForwarding)

Type: PhoneBean with components

Components: International Dialing Code (3 chars), Area Code (3 chars), Number (10 chars), Extension (4 chars)

Display: Formatted phone number in infoset, disabled input fields in dialog

Validation: Read-only field, cannot be edited

Managers Section:

General Manager (generalManager)

Type: String (combined first and last name)

Display: Full name in infoset, separate first/last name fields in dialog

Components: First Name (40 chars), Last Name (40 chars)

Validation: Read-only fields, alphanumeric with allowed special characters (. , / -)

Behavior: Copy/paste disabled

Sales Manager (salesManager)

Type: String (combined first and last name)

Display: Full name in infoset, separate first/last name fields in dialog

Components: First Name (40 chars), Last Name (40 chars)

Validation: Read-only fields, alphanumeric with allowed special characters (. , / -)

Behavior: Copy/paste disabled

Authorization:

All changes require authorization through the "Authorized By" field

Users can choose to remember authorization for the session

