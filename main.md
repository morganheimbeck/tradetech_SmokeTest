## Use

### Authoring

Use headings to drill into a particular part of the application.

Use checked boxes (`[x]`) to indicate something has been tested automatically.

Use unchecked boxes (`[ ]`) to indicate something has NOT been tested automatically.

For specific __readonly__ or __tsc__ user-class behavior include a __USER_CLASS__ tag by the test case. For example: __readonly__.

### Creating a test

- Copy this to a new file or issue.  Check the checkboxes you've tested.


## Login
- [ ] login as a user
- [ ] failed login
- [ ] reset password
- [ ] close login dialog, click Log In to restore

## Profiles - Account Profile

### Account Profile - Create New

- [ ] `PX` Create a new corporation.
- [ ] `PX` Create a new corporation, but choose "Same Corporation - New Company"

### Account Profile - Reports - Quick Search

- [ ] `PX` Search by a corporation, verify the corporation you created shows up.
- [ ] Search by each field, matching results in flyout
- [ ] filter table headers at top of flyout table filter the results.
- [ ] clicking company name in table opens up company in main page
- [ ] clicking expansion icon in table opens contacts table below company entry in search results table
  - [ ] new contacts can be added in table

### Account Profile - Reports - other searches

- [ ] Full search
- [ ] Quotes by station
- [ ] Quotes by user
- [ ] Profile approval report

### Account Profile - Edit

#### View/Edit Corporation

- [ ] `PX` Edit the corporation details.  Click save to see results are actually saved.
- [ ] `PX` Edit the corporation details.  Click "cancel" and verify data went back to its previous state.
- [ ]  Click cancel with no changes; profile closes

##### Corporation Subtabs
- [ ] Contacts subtab opens contacts table in tray
- [ ] CRM subtab shows form in tray
- [ ] Pricing Controls subtab shows form with two text fields in tray.

#### Add Company

- [ ] `PX` Click `+ Add Company`.  Add a company.  Verify you can hit left-and-right buttons to see new and existing companies.

#### Edit Company

- [ ] `PX` Edit the company details.  Click save to see results are actually saved.
- [ ] `PX` Edit the company details.  Click "cancel" and verify data went back to its previous state.

##### Company Subtabs
- [ ] Contacts subtab opens contacts table in tray
- [ ] CRM subtab shows form in tray
- [ ] compliance subtab shows forms for Importer/Exporter/Carrier in tray.
  - [ ] verify forms
- [ ] Accounting subtab shows forms for Billing/Tax Information/Insurance in tray
- [ ] Communications subtab shows form with mostly radios in tray.
  - [ ] verify radio options working.
- [ ] NSA/NRA subtab shows "Feature coming soon" in tray
- [ ] Consignment subtab shows grid of 10 expandable person forms in tray
- [ ] Linked Accounts subtab shows table of associations in tray
  - [ ] Verify associations can be added and filtered.

#### Edit Location
- [ ] `PX` Edit the location details.  Click save to see results are actually saved.
- [ ] `PX` Edit the location details.  Click "cancel" and verify data went back to its previous state.

##### Location Subtabs
- [ ] Contacts subtab opens contacts table in tray
- [ ] Accounting subtab shows read-only form in tray
- [ ] Admin Workflow subtab shows form with mostly autocompletes in tray.
  - [ ] verify working autocompletes
- [ ] Compliance subtab shows form of text entries and selects in tray
- [ ] Consignment subtab shows grid of 10 expandable person forms in tray
- [ ] Local subtab shows form of local addresses (text fields) in tray.

### Sidebar buttons

#### Corporation sidebar
- [ ] View Rates pops up search dialog
  - [ ] search dialog functions without error, results in flyout.
- [ ] Terms and Conditions opens modal dialog.
- [ ] Add/Edit Service Fees opens tray below profile with global and corporation fees
  - [ ] filter fields in header of each table filter results.
  - Is this editable?  I don't see editing features. --BM

#### Company sidebar
- [ ] View Rates pops up search dialog
  - [ ] search dialog functions without error, results in flyout.
- [ ] Add/Edit Service Fees opens tray below profile with global and corporation fees
- [ ] Support Documents opens tray with upload box
  - [ ] uploading a document succeeds.

#### Location sidebar
- [ ] View Rates pops up search dialog
  - [ ] search dialog functions without error, results in flyout.
- [ ] Add/Edit Service Fees opens tray below profile with global and corporation fees

## Trade Rates - Rates

### Trade Rates - Rates - Create New Quote

- [ ] `PX` Create New > Quote starts wizard from Preferences panel.
- [ ] `PX` Create a new quote

### Trade Rates - Rates - Reports - View Rates
- [ ] Search by rate type (FCL / LCL)
- [ ] Search by each field, matching results in flyout
- [ ] filter table headers at top of flyout table filter the results.
- [ ] clicking expansion icon in table opens read-only form detailing container load
  - [ ] Click Expire Alert --  alerts "Expiration Warning has been sent"
- [ ] Click File -- rate gets a value in Tariff Number

### Trade Rates - Rates - Reports - other searches
- [ ] View Shipment Specific Rates -- same features as View Rates
- [ ] Sell Rate GRI/GRD -- shows grid, each row expands to read-only form
  - [ ] click Copy in a grid result -- opens Trade Rates » Rates » Create GRI/GRD in main page
- [ ] Sales Productivity -- choose date range -- opens grid of regions, each row opens grid of salespersons, each opens grid of customers, each opens grid of rates for items from origin to destination
- [ ] Service Fees -- no results for searches in DEV here, unsure what should happen
- [ ] Margin Monitor -- no results for searches in DEV

## Trade Rates - Tariff Rules

### Trade Rates - Tariff Rules - Create New
- [ ] `PX` Create a new Tariff Rule.

## Trade Rates - Tariff Rules - Reports - General Rules
- [ ] Search with no criteria to see all results
- [ ] Search by each field, matching results in flyout
- [ ] filter table headers at top of flyout table filter the results.

## Trade Rates - Tariff Rules - Reports - Accessorials
- note: in latest bitbucket mainline, accessorials has been given its own primary menu entry under Trade Rates
- cannot test this currently -- request fails with "One of the fields that you have requested is not readable." (may be destinationPort.description)

## Trade Rates - Tariff Title Page
- [ ] search title pages with no criteria
- [ ] search by organization number
- [ ] clicking organization number in flyout grid opens title page in main page

## Trade Rates - Sailing Schedules
- [ ] Search by origin and destination
- [ ] Search additionally by each field, matching results in flyout
- [ ] filter table headers at top of flyout table filter the results.
- [ ] clicking expansion icon in Carrier column opens read-only list of carriers
- [ ] Click Mother Vessel entry (not all are clickable) -- see dialog with Travel Map

## Trade Rates - Tender Management
- Cannot test due to following issues (happen on mainline branch):
- Attempting to open the Tender Management report throws an error (error dialog is shown)
- Attempting to create new throws console error and only the Syrinx logo is shown in main page.


## Trade Manager - Operations

### Trade Manager - Operations - Create New
- [ ] click Create New, shows blank shipment with Essentials wizard step visible.  Route shows `/trade_manager/operations/view/<some ID>`
- [ ] Continue button is disabled until all required fields are filled.
- Note: from here all edit operations are the same as viewing/editing an existing shipment; see below for testing steps.

### Trade Manager - Operations - Reports - Quick Search
- [ ] Search by house bill # (e.g. 1234)
- [ ] Search by each field, matching results in flyout
- [ ] filter table headers at top of flyout table filter the results.
- [ ] clicking expansion icon in table opens table of container loads
  - [ ] Click expansion icon in container loads table, shows table of purchase orders.
- [ ] Hover chevron in House Bill, see a popover with editable fields -- edit fields and verify values are updated after a new search (bug in system does not update display until a new search)
- [ ] Hover over chevron in MBL #, see a popover with editable fields -- edit fields and verify values are updated after a new search (bug in system does not update display until a new search)
- [ ] Click house bill number -- shipment opens in main page.

### Trade Manager - Operations - Reports - Other search types
- [ ] Shipments in Progress; search result is read-only table.
  - [ ] Click expansion icon; containers table is shown
    - [ ] Click expansion icon in containers table; summary of container contents is shown.
  - [ ] Click "House" column entry; shipment is shown in main page
  - [ ] Click copy icon (fourth column); prompt is shown confirming copy
- [ ] Sailing Schedules; search by origin and destination, search result is read-only table
  - [ ] Click expansion icon in Carrier column; list of carriers and services is shown
  - [ ] Click Mother Vessel column data (not all are clickable); Transit map dialog is shown 

#### Trade Manager - Operations - Reports - Other search types - Shipments
- [ ] Booking Report -- search result is a read-only table of bookings
  - [ ] Click expansion icon; row expands to show a read-only table of numbered containers
  - [ ] Click on booking number; shipment opens in main page
- [ ] Daily Cargo Receiving Report; search by load facility. [cannot find any results]
- [ ] Inventory Planning Report; search by "Real Customer" [I receive no-access error; this is not a bug --BM]
- [ ] Trucker; search by House Bill, shows table with editable field
  - Note: Pickup Order button seems to be broken currently.  It's trying to POST to the .html url
  - [ ] Terminal Appt Book button is disabled?
- [ ] Warehouse; search is currently broken ("Mini_Search Trade_Manager Menu: WarehouseView did not refer to a valid menu option.")
- [ ] Fuji Xerox Report; search by customer and date range, search result is read-only table
- [ ] Empty Container Return; search result is read-only table
  - [ ] Click on House Bill number, shipment opens in main page
  - [ ] Click on Export to Excel, xls file downloads
- [ ] Container Summary Upload Tool; search by shipment type, search result is read-only table
  - [ ] hover chevron in Upload column, get a file upload popover
  - [ ] try uploading a file, file uploads but internal server error happens when trying to call /cgi/uploads/containers.pl  (this may be due to attempting to parse a document that isn't a container summary)


#### Trade Manager - Operations - Reports - Other search types - Cargo Security
- [ ] Cargo Security In Progress -- search result is a read only table with clickable house bill number and popovers for House Bill, AMS Status, and Origin Station.
  - [ ] Some rows have expansion icons.  Clicking those shows a transaction log table

#### Trade Manager - Operations - Reports - Other search types - Statistics
- [ ] Cargo Security Statistical Report; search result shows table of compliance/security records collated by security type and message
  - [ ] Expand record; see table of all records for grouping
  - [ ] Click House bill number in expanded table; loads Shipment in main page
- [ ] Volume Report; shows read-only table of statistics by selected First Level
  - [ ] Create report with no CY status; shows one record for each first level and CY status
  - [ ] Create report with CY status; shows one record for each first level
  - [ ] Create report with second and third levels; shows expansion button in table, expands to second level; second level expands to third level.
  - [ ] Click Export to Excel; opens new tab to .xls file with UUID name in /tmp folder
- [ ] On Time Report; search result is read-only table.

### Trade Manager - Operations - View Shipment
- [ ] Shipment numbers and other main data appear in header next to "Shipment"
- [ ] Shipper, Consignee, and Notify/Notify2 panels each have an editable contact.
  - [ ] Hover "Show Name and Phone" -- see popover with editable name/phone/email fields
- [ ] in Notify panel click Create Profile. Form for creating corp or company profile appears in panel.
- [ ] in Security / Compliance panel click Parties.  See overlay with editable contact form panels for each of Delivery Address, Seller, Buyer, Importer, Manufacturer (Supplier), Container Stuffing Location, Consolidator, and Booking party.
  - [ ] Edit form fields and verify changes are saved and re-shown when clicking away from and back to Parties.
- [ ] in Security / Compliance panel click AMS, see editable form of Customs information (select), Second Notify Party (table), and In-Bond logs (not editable).
- [ ] in Container panel click each of Overview, Security, Inventory, VGM, Pickup, Delivery, O. Rail, D. Rail; a table shows for each in overlay
  - [ ] Verify editable fields and popover fields save changes in each tab
  - [ ] Remove checkbox in Overview shows warning modal before removing shipment
  - [ ] Transmit button in VGM shows error modal if size is incorrect; shows Transmit VERMAS dialog if fields are valid.
  - [ ] Pickup tab, Pickup Order View button shows dialog with wizard for reviewing & transmitting pickup order
  - [ ] Book terminal order button [is disabled?  unknown what happens on click]
  - [ ] Delivery tab, Delivery Order View button shows dialog with wizard for reviewing & transmitting delivery order
- [ ] in Notes panel click Notes link, see overlay with Create Note textarea on right.
  - [ ] Adding a note shows added note on left with username.
- [ ] Routing panel shows autocomplete for each connection between origin and destination; popover next to vessel name is read only.
- [ ] Cargo Notes -- Marks & Numbers and Commodity Description tabs each show an editable textarea.
- [ ] Shipment Events -- Ports, scheduled, and actual dates are editable in table.

#### Trade Manager - Operations - View Shipment - wizard tabs
- [ ] at each step, Continue button opens next wizard step
- [ ] Essentials -- form
- [ ] Compliance -- list of regional authorities with select menus for compliance form type, except ISF which is a checkbox
- [ ] Route -- table of origin, connections, and destination.  changes here are reflected in the Routing panel
  - [ ] Ensure connections can be added, edited, and scheduled. Scheduling requires origin and destination to be filled in
- [ ] Admin Work Flow - form of all autocomplete fields
- [ ] Shipment Specifics - basic form

#### Trade Manager - Operations - View Shipment - Save button
- [ ] no changes in the panels, overlays, nor wizard tabs are saved unless the Save button is clicked.
- [ ] Click Save after making changes, reload, verify changes are saved.

#### Trade Manager - Operations - View Shipment - Actions drawer
- [ ] Click Actions, drawer with tabs slides in from right.
- [ ] Accounting tab -- Invoices, Costs, and Credits expand to read-only tables
- [ ] Documentation tab -- each button launches a dialog with a Review/Transmit wizard and sets Completed Date / Name for the document type
  - [ ] Printing the Original Negotiable B/L prevents future printings of the Sea Waybill
- [ ] Notification tab -- each button launches a dialog with a Review/Transmit wizard and sets Completed Date / Name for the document type
- [ ] Action tab -- Receive Carrier Confirmation button is disabled?
- [ ] Compliance tab -- [shows nothing, unsure what is supposed to be here]
- [ ] Uploaded Documents tab -- has upload button and drag target
- [ ] Tools tab -- Transfer Abi Data button shows Complete dialog when operation finishes.

## Trade Manager - PO Management

### Trade Manager - PO Management - Create New
- [ ]  click Create New; blank purchase order appears in main page; Essentials wizard step is visible
- TBD: edit flow for new or existing PO

### Trade Manager - PO Management - Reports
- PO In Progress Report; search is currently broken
- [ ] SKU Management Report; search by SKU number [required despite not being marked as such], search result is a read-only table
  - Expansion icon currently causes an error when clicked.
- [ ] PO Action Report; search result is a read-only table of purchase order events
  - [ ] Click expansion icon; table of shipped contents is shown
- [ ] Booking Approval Report; at least one search field is required, zero fields will cause an error; search result is a read-only table of bookings
  - [ ] Click expansion icon; table of shipped contents is shown
  - [ ] Click Export to Excel; downloads .xls file with UUID name from /tmp path

## Trade Manager - Consolidations

### Trade Manager - Consolidations - Create New
- [ ] click Create New, shows blank consolidation with Essentials wizard step visible.
- [ ] Shipment Type is the only required field in Essentials and is prefilled; Continue button is enabled.
- Note: from here all edit operations are the same as viewing/editing an existing consolidation; see below for testing steps.

### Trade Manager - Consolidations - Reports
- [ ] FCL; search by vessel name and voyage number
  - TBD need to find valid numbers to search
- Consolidation Planning; search results are not rendering
- [ ] Consolidation In Progress; search result is a read-only table
  - [ ] Click Expansion icon; opens a table of shipments
  - [ ] Click Copy icon; confirmation modal dialog is displayed
  - [ ] Click cell value in Consol number; consolidation opens in main page, Essentials wizard step is shown

### Trade Manager - Consolidations - View Consolidation
- [ ] Consolidation numbers and other main data appear in header next to "Consolidation"
- [ ] Consol Planning tab is visible
- [ ] Shipper, Consignee, and Notify panels each have a read-only contact.
  - [ ] Hover "Show Name and Phone" -- see popover with read-only name/phone/email fields
- [ ] in Shipments panel, grid of editable fields
- [ ] Routing panel shows autocomplete for origin and each connection between origin and destination; popover next to vessel name is read only.
- [ ] Events -- Ports, scheduled dates, and actual dates (from popover) are editable in table.

#### Trade Manager - Consolidations - View Consolidation - wizard tabs
- [ ] at each step, Continue button opens next wizard step
- [ ] Essentials -- form
- [ ] Compliance -- list of regional authorities with select menus for compliance type
- [ ] Route -- table of origin, connections, and destination.  changes here are reflected in the Routing panel
  - [ ] Ensure connections can be added, edited, and scheduled. Scheduling requires origin and destination to be filled in
- [ ] Admin Work Flow - form of two autocomplete fields for locations

#### Trade Manager - Consolidations - View Consolidation - Actions drawer
- [ ] Click slide-in button on right margin, drawer with tabs slides in from right.
- [ ] Documentation tab -- each button launches a dialog
  - [ ] B/L Instructions button shows Master Bill Specifics dialog with form of contacts and details
  - [ ] Container Manifest button validates the presence of Port Of Loading Sched Date, Admin Origin Gateway Station Id, and Admin Destination Gateway Station Id.  Dialog shown if any are missing.
  - TODO: click container manifest button when these are filled in.
  - [ ] Container Loading Plan button validates the presence of Port Of Loading Sched Date, Admin Origin Gateway Station Id, and Admin Destination Gateway Station Id.  Dialog shown if any are missing.
  - TODO: click container loading plan button when these are filled in.
- [ ] Notification tab -- each button launches a dialog
  - [ ] Arrival/Departure Notice button validates the presence of Port Of Loading Sched Date, Admin Origin Gateway Station Id, and Admin Destination Gateway Station Id.  Dialog shown if any are missing.
  - TODO: click arrival/departure notice button when these are filled in.
  - [ ] Pickup Order button validates the presence of Port Of Loading Sched Date, Admin Origin Gateway Station Id, and Admin Destination Gateway Station Id.  Dialog shown if any are missing.
  - TODO: click pickup order button when these are filled in.
  - [ ] Delivery Order button validates the presence of Port Of Loading Sched Date, Admin Origin Gateway Station Id, and Admin Destination Gateway Station Id.  Dialog shown if any are missing.
  - TODO: click delivery order button when these are filled in.
- [ ] Uploaded Documents tab -- has upload button and drag target

#### Trade Manager - Consolidations - View Consolidation - Consol Planning tab
- [ ] Left side table shows available shipments with filters and paging
- [ ] Right side has a table per consolidation with unique ID in header
- [ ] Right side table has editable load order field per shipment and expansion button in footer for other editable items
- [ ] verify adding shipments to consol with dragging, removing with remove button in table.
- [ ] Click edit button in right side table.  Error info is shown if consolidation has unsaved data.
  - TODO what happens when data is saved?  I'm getting some errors when saving consol.

## Trade Cash - Revenue / Expense

### Trade Cash - Revenue / Expense - Create New
- [ ] Click Create New; a form is shown for a new invoice
- [ ] Invoice Date (Revenue) / Due Date (Expense) is prefilled with the current date

## Trade Cash - Reports

### Trade Cash - Reports - Invoice/Cost Report
- [ ] Search by transaction type; Result is a read-only table with clickable invoices
- [ ] Search by invoice number, HBL number, reference number, and the autocomplete, select, and date fields; results should match criteria
- [ ] filter table headers at top of flyout table filter the results.
- [ ] Click invoice number in results table; invoice is opened in dialog window

### Trade Cash - Reports - Other Report Type
- [ ] Global Margin; result is a table of summaries by house bill;
  - [ ] Click expansion icon in second column of a result record; table of vouchers shown
  - [ ] mouseover Add & View in File Audit Notes; popover is shown.
  - [ ] in File Audit Notes Add popover, type a note and click Save; note can be seen in View when results are refreshed.
  - [ ] Click Origin Complete button if shown; button is replaced with Done and mouse target chevron
    - [ ] Mouseover chevron next to Done; your own username and the date Complete was clicked are shown in popover
  - [ ] Click Destination Complete button if shown; button is replaced with Done and mouse target chevron
    - [ ] Mouseover chevron next to Done; your own username and the date Complete was clicked are shown in popover
  - [ ] Click Finalize button if shown; button is replaced with Locked and mouse target chevron
    - [ ] Mouseover chevron next to Locked; your own username and the date Finalize was clicked are shown in popover
  - [ ] Click expansion icon in Profit Split column; records of Profit Share based on rate and total margin shown for HQ/Origin/Destination
- [ ] Monthly Statement; search by tx type and either company or location; result is table of month-end invoices with Export
  - [ ] Click expansion icon; table of individual invoice subtotals is shown
- Income Statement; cannot see results (no table shows locally, error on dev)
- [ ] Clearing House Summary; result is a read-only table
- Clearing House Detail returns a proxy error on search

### Trade Cash - View/Edit Revenue/Expense
- [ ] Test autocompletes for proper search and matching results
- [ ] Click Full Credit;  invoice is closed and cancelled
- [ ] Click Save; after save is complete, dialog is closed and reopened
  - [ ] prior to save, error popup if no changes have been made
- [ ] Click Close; voucher from dialog or main page is dismissed
- [ ] Click Save/Close;  after save is complete, voucher is dismissed from dialog or main page
  - [ ] prior to save, error popup if no changes have been made
- [ ] Click Send; voucher is closed and Print/Send dialog is opened; has Review Data/Review Document/Transmit steps.
  - [ ] prior to send dialog, error popup if no changes have been made

## Read-Only User Class

## TSC User Class 
