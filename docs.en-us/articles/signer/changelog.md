﻿# Signer changelog

> [!NOTE]
> This version history currently contains only the most recent changes to the application. We are working on
> documenting older versions.

<a name="v1-35-0" />
### 1.35.0 (2021-09-15)

* New Features
  * [SIG-752] Instance setting to define which document version is sent in the document conclusion notification
  * [SIG-576] Folder selector that allows to navigate in folder hierarchy

* Improvements
  * [SIG-745] Add signature type (electronic or digital) in document reports
  * [SIG-699] Setting to mask CPFs
  * [SIG-687] Document signature with certificate requirements

* Bug fixes
  * [SIG-753] Signature positioning not available in document generation
  * [SIG-749] Instance with disabled printer friendly version is attaching it in document conclusion notifications
  * [SIG-733] Document creator in organization cannot edit or delete documents he created

Updates database model: yes

<a name="v1-34-0" />
### 1.34.0 (2021-08-20)

* New Features
  * [SIG-740] Add setting that allows notification of pending actions in batch signature
  * [SIG-737] Create space cadet yellow theme
  * [SIG-181] Default signature image for both digital and electronic signatures

* Improvements
  * [SIG-719] Allow reduction of possible actions in the public area
  * [SIG-689] Handle repeated headers in the document generation CSV
  * [SIG-662] Cloud certificate signature does not display certificate validation errors in single signature

* Bug fixes
  * [SIG-742] Printer friendly version displays expiration watermark even if the document is concluded
  * [SIG-734] Incorrect selfie orientation when taking picture in iOS
  * [SIG-725] Error while removing participant from flow after sending SMS or creating Pix authentication
  * [SIG-706] Organization is not unblocked after paying due invoices

Updates database model: no

<a name="v1-33-1" />
### 1.33.1 (2021-07-30)

* Improvements
  * [SIG-736] Update Azure blob management library

* Bug fixes
  * [SIG-735] Error while signing PDF electronically

Updates database model: no

<a name="v1-33-0" />
### 1.33.0 (2021-07-22)

* New Features
  * [SIG-418] Display update history in document details
  * [SIG-422] Envelope submission (public batch signature/approval)
  * [SIG-480] Batch signature reminders in documents screen
  * [SIG-524] Document report by folder
  * [SIG-596] Document saved flows management
  * [SIG-618] Document refusal and cancellation
  * [SIG-686] Add e-CNPJ information in the signature mark
  * [SIG-696] Advanced document search
  * [SIG-697] Due date for signing documents
  * [SIG-713] Email templates customization per instance

* Improvements
  * [SIG-633] Signature ticket simplification to have shorter URLs
  * [SIG-703] Enable TSP provider names to be hidden for cloud certificates
  * [SIG-712] Add international orange apricot theme
  * [SIG-720] Update document due date
  * [SIG-724] Add generic viridian blue theme

* Bug fixes
  * [SIG-701] Electronic signature with Selfie not working in iOS

Updates database model: yes

<a name="v1-32-0" />
### 1.32.0 (2021-06-25)

* New Features
  * [SIG-670] Electronic signature with PIX authentication
  * [SIG-631] Electronic signature with facial biometric validated by SERPRO
  * [SIG-538] Refuse to sign a document

* Improvements
  * [SIG-653] Embedded signature without document preview

* Bug fixes
  * [SIG-690] Error signing deleted document if the enabled deleted document validation is enabled

Updates database model: yes

<a name="v1-31-1" />
### 1.31.1 (2021-06-08)

* Bug fixes
  * [SIG-691] Share participant link button should direct approvers to private area

Updates database model: no

<a name="v1-31-0" />
### 1.31.0 (2021-06-08)

* New Features
  * [SIG-688] Add international orange green and onyx carrot orange themes
  * [SIG-664] Instance documents per month report
  * [SIG-655] Generate share link for document participants

* Improvements
  * [SIG-685] Add support to alternative authentication methods with AWS S3
  * [SIG-656] Support signature validation with obsolete algorithms
  * [SIG-650] Display non PDF files while signing documents
  * [SIG-648] Improve error handling of password protected PDFs
  * [SIG-628] Add warning that attachments are not signed
  * [SIG-560] Support validation of files with more than 100 signatures

* Bug fixes
  * [SIG-649] Do not display signature positioning option for non PDF documents

Updates database model: no

<a name="v1-30-0" />
### 1.30.0 (2021-05-25)

* Improvements
  * [SIG-659] Auto retry timestamp request after a failure
  * [SIG-646] Add home page dynamic HTML as a trusted resource
  * [SIG-629] Batch signature of documents without the need to select them page by page

* Bug fixes
  * [SIG-661] Conclusion notification not being sent in fast signature mode
  * [SIG-658] Emails to be notified when document are concluded are not being notified when the documents are signed in batch
  * [SIG-657] Too many emails sent to participants when generating documents
  * [SIG-654] Cannot edit the text positioning of the signature visual representation after the images has been sent
  * [SIG-645] Display of signers in the manifest is different if the file type is not PDF

Updates database model: yes

<a name="v1-29-0" />
### 1.29.0 (2021-04-27)

* New Features
  * [SIG-638] Zoom meetings integration
  * [SIG-624] Set notified emails to send documents as attachment after the flow is concluded
  * [SIG-543] CSV with flow information to generate multiple documents with document specific flows

* Improvements
  * [SIG-460] Display pending signatures in the signature manifest

* Bug fixes
  * [SIG-643] Signature intials options is not displayed if document authentication option is not visible 
  * [SIG-642] Wrong extensions added when downloading multiple documents at once

Updates database model: yes

<a name="v1-28-0" />
### 1.28.0 (2021-04-06)

* New Features
  * [SIG-555] Require the selection of a signature representation position
  * [SIG-476] Consent Removal

* Improvements
  * [SIG-634] Allow Timestamper authentication with Basic Authentication
  * [SIG-621] Send welcome notification only after the document is concluded
  * [SIG-613] Allow a user submitting a document to inform the cellphone number for SMS electronic signature signers
  * [SIG-578] Add new SMS providers

* Bug fixes
  * [SIG-635] Invoice webhook does not included owner information
  * [SIG-630] Edit flow button is displayed even for concluded flows
  * [SIG-470] Error signing with custom visual representation that has .webp file

Updates database model: yes

<a name="v1-27-0" />
### 1.27.0 (2021-03-25)

* New Features
  * [SIG-614] Service receipt generation (NFS-e)

* [SIG-549] iugu payment gateway integration:
  * [SIG-588] Create checkout page
  * [SIG-593] Allow user to view and set his favorite payment method
  * [SIG-592] Send emails to clients regarding invoices statuses
  * [SIG-590] Display payment information in the invoice details screen

* Improvements
  * [SIG-625] Add new API for SECURITI integration
  * [SIG-620] Fix tests that are failing in the development environment
  * [SIG-606] Add setting to remove view documents button in multiple documents notifications

* Bug fixes
  * [SIG-626] Fix signature time displayed in the printer friendly version
  * [SIG-617] Incorrect detection of Scanner integration

Updates database model: yes

<a name="v1-26-1" />
### 1.26.1 (2021-02-18)

* Bug fixes
  * [SIG-616] File name is required when uploading with API
  * [SIG-615] Error sending document to user with email that is a part of other emails
  * [SIG-609] Fix translation of resource common.search (i18n)

Updates database model: no

<a name="v1-26-0" />
### 1.26.0 (2021-02-11)

* Improvements
  * [SIG-605] Update New Relic Sink to improve exception log
  * [SIG-604] Update Lacuna SPA

Updates database model: no

<a name="v1-25-0" />
### 1.25.0 (2021-02-03)

* Improvements
  * [SIG-602] - Improve AWS S3 support

Updates database model: yes

<a name="v1-24-3" />
### 1.24.3 (2021-01-28)

* Improvements
  * [SIG-599] - Do not send invite email if the document was created with the disable notifications option

* Bug fixes
  * [SIG-601] - Cannot use signature rules with private attachments

Updates database model: no

<a name="v1-24-2" />
### 1.24.2 (2021-01-18)

* Bug fixes
  * [SIG-598] - Error opening document creation screen without organizations in the closed system mode

Updates database model: no

<a name="v1-24-1" />
### 1.24.1 (2021-01-15)

* Bug fixes
  * [SIG-597] - Wrong theming of the signature position message

Updates database model: no

<a name="v1-24-0" />
### 1.24.0 (2021-01-14)

* New Features
  * [SIG-463] - Display electronic signature as first option in signature page
  * [SIG-594] - Electronic signature validation for CAdES and XAdES

* Improvements
  * [SIG-441] - Create options to define which PDF page should be displayed first in the Embedded Signature Widget
  * [SIG-474] - Add consent message in screens for LGPD
  * [SIG-496] - Improve handling of password protected PDFs in Fast Signature
  * [SIG-566] - Document flow completion email should redirect to public area
  * [SIG-584] - Simplify user experience of the public signature page

* Bug fixes
  * [SIG-568] - Signature position instructions still displayed after signature
  * [SIG-595] - Error deleting approver that is last participant in the flow

Updates database model: yes

<a name="v1-23-0" />
### 1.23.0 (2021-01-07)

* New Features
  * [SIG-430] - Electronic signature with Selfie
  * [SIG-554] - Allow adding attachments to documents

* Improvements
  * [SIG-408] - Allow signature pre-positioning in edit flow screen
  * [SIG-583] - Update PKI SDK to correct text positioning

* Bug fixes
  * [SIG-582] - Fix RUC validation (Ecuador)

Updates database model: yes

<a name="v1-22-0" />
### 1.22.0 (2020-12-17)

* New Features
  * [SIG-144] - Display electronic signature evidences
  * [SIG-551] - Add document description field
  * [SIG-541] - Allow user to set a message that will be added to pending signature/approval emails

* Improvements
  * [SIG-330] - Allow user to define signature positions for multiple files
  * [SIG-390] - Show all signature in signature pre-positioning
  * [SIG-425] - Validate Scanner verification code of any Scanner subscription
  * [SIG-426] - Add validation stamp in Scanned document
  * [SIG-531] - Improve error handling of HSM signatures
  * [SIG-545] - API to validate signatures and retrieve electronic signature evidences by document ID
  * [SIG-550] - Increase number of retrieved folder in document creation screen
  * [SIG-559] - Update Lacuna PKI to allow ANF certificates (Ecuador)
  * [SIG-570] - Fix welcome and terms of use emails i18n
  * [SIG-571] - Parameterize application default currency
  * [SIG-572] - Parameterize accepted file types for document creation

Updates database model: yes

<a name="v1-21-0" />
### 1.21.0 (2020-12-03)

* New Features
  * [SIG-217] - Allow CPF to be nullable

Updates database model: yes

<a name="v1-20-0" />
### 1.20.0 (2020-11-27)

* New Features
  * [SIG-477] - Integration with Securiti to automate LGDP/DSR requests
  * [SIG-486] - Billing of timestamps and SMS

* Improvements
  * [SIG-508] - Create option to disable email change while submitting a document
  * [SIG-553] - Add participant title in the Simplified manifest
  * [SIG-563] - Enable organization creation via integrations
  * [SIG-565] - Disable indexing of the document validation page

Updates database model: no

<a name="v1-19-0" />
### 1.19.0 (2020-11-18)

* Improvements
  * [SIG-468] - Allow creation of subfolders
  * [SIG-544] - Recognize electronic signatures in the manifest and code validation
  * [SIG-548] - Direct user to billing screen if he has not set billing information
  * [SIG-557] - Replace the name of the initial approval button to review

* Bug fixes
  * [SIG-546] - Document is displayed as signed if another participant has refused it
  * [SIG-547] - Error signing XLSX file
  * [SIG-558] - Prevent normalization of PDFs if they are signed

Updates database model: yes

<a name="v1-18-0" />
### 1.18.0 (2020-11-05)

* New Features
  * [SIG-483] - Prevent completion of billable actions while billing information is not set
  * [SIG-513] - Disable signature visual representation automatic positioning
  * [SIG-519] - Webhook for completed flow actions

* Improvements
  * [SIG-528] - Allow validation of deleted document

Updates database model: no

<a name="v1-17-0" />
### 1.17.0 (2020-10-28)

* Improvements
  * [SIG-437] - Allow flow edit even with Simplified Manifest enabled
  * [SIG-506] - Add logo to lateral mark (validation stamp)
  * [SIG-517] - Changes to manifest and simplified manifest

Updates database model: no

<a name="v1-16-1" />
### 1.16.1 (2020-10-23)

* Improvements
  * [SIG-534] - Create billing administration profile

Updates database model: no

<a name="v1-16-0" />
### 1.16.0 (2020-10-22)

* Improvements
  * [SIG-484] - Include billing information in the closed invoice Webhook
  * [SIG-485] - API to Update invoice status
  * [SIG-525] - Improve error message when upload is not found

* Bug fixes
  * [SIG-511] - Scan button is over the exclude file button in the document submit screen
  * [SIG-526] - Error in unique signature for non PDF documents

Updates database model: no

<a name="v1-15-1" />
### 1.15.1 (2020-10-21)

* Bug fixes
  * [SIG-529] - Restricted access screen does not show if basic profiles are set as default

Updates database model: no

<a name="v1-15-0" />
### 1.15.0 (2020-10-08)

* New Features
  * [SIG-520] - Document versions direct download API
  * [SIG-521] - Simplified API for uploads
  * [SIG-522] - Enable configuration of maximum upload size

* Improvements
  * [SIG-471] - Update watermark text for the validation stamp

Updates database model: no

<a name="v1-14-0" />
### 1.14.0 (2020-09-30)

* Improvements
  * [SIG-427] - Notify the creator of a document upon flow conclusion

* Bug fixes
  * [SIG-499] - Validation screen shows email from registration instead of the one validated in the electronic signature
  * [SIG-505] - Flow order is lost when using a flow from another document
  * [SIG-512] - Error displaying document status in the document administration screen

Updates database model: no

<a name="v1-13-0" />
### 1.13.0 (2020-09-23)

* Improvements
  * [SIG-366] - Allow reproval in the approval flow action
  * [SIG-383] - Improve preview of digital certificates
  * [SIG-411] - Improve error message when a PDF has password and allow signature of protected PDFs
  * [SIG-438] - Set Restricted autocomplete mode as default

* Bug fixes
  * [SIG-442] - Cannot validate signed XML file
  * [SIG-457] - Invoices button is displayed even with billing disabled
  * [SIG-459] - Handle case where page number of a visual representation is set to a page that does not exist in the PDF
  * [SIG-479] - Electronic signature visual representation does not contain the tile specified for the signer

Updates database model: yes

<a name="v1-12-0" />
### 1.12.0 (2020-09-14)

* New Features
  * [SIG-462] - Add profiles to enable/disable creation of documents and organizations
  * [SIG-464] - Add phone number parameter to document creation API

* Improvements
  * [SIG-373] - Generate signing widget with Typescript
  * [SIG-465] - Fast signature with cloud certificate

* Bug fixes
  * [SIG-466] - Error editing order of flow actions

Updates database model: no

<a name="v1-11-0" />
### 1.11.0 (2020-09-02)

* New Features

* Improvements
  * [SIG-397] - Cloud certificates support

Updates database model: no

<a name="v1-10-4" />
### 1.10.4 (2020-08-31)

* New Features
  * [SIG-455] - Add persian-plum-sand theme

* Improvements
  * [SIG-417] - Add file segmented upload

Updates database model: no

<a name="v1-10-3" />
### 1.10.3 (2020-08-26)

* New Features
  * [SIG-429] - Add indicative text to download App for the QR code signature feature
  * [SIG-439] - Update texts and watermark of the simplified manifest

Updates database model: no

<a name="v1-10-2" />
### 1.10.2 (2020-08-25)

* New Features
  * [SIG-449] - Create viridian green yellow theme

* Bug fixes
  * [SIG-447] - Error sending SMS with TotalVoice
  * [SIG-448] - Timeout in login process

Updates database model: no

<a name="v1-10-1" />
### 1.10.1 (2020-08-21)

* New Features
  * [SIG-435] - Create oxford-blue-green theme
  * [SIG-436] - Create castleton-green-orange theme

* Bug fixes
  * [SIG-420] - Blocked screen after failed attempt to sign document with A3 certificate

Updates database model: no

<a name="v1-10-0" />
### 1.10.0 (2020-08-19)

* Improvements
  * [SIG-382] - Associate Applications to folders
  * [SIG-384] - Standard language for the system
  * [SIG-389] - Check if user is already registered in organization while adding
  * [SIG-399] - Check maximum attachment size while sending email
  * [SIG-400] - Load fast signature screen with pre-uploaded file 
  * [SIG-404] - Add simplified manifest option for the Validation Stamp
  * [SIG-409] - Improve error message when an email is already being used by another account
  * [SIG-412] - Support to medical prescriptions in document generation

* Bug fixes
  * [SIG-407] - Validation Stamp not showing for documents with size smaller than A4
  * [SIG-416] - Error creating non PDF documents when Validation Stamp is enabled

Updates database model: yes

<a name="v1-9-1" />
### 1.9.1 (2020-07-23)

* Bug fixes
  * [SIG-396] - String not translated in folder settings
  * [SIG-410] - Unnecessary scroll in home page

Updates database model: no

<a name="v1-9-0" />
### 1.9.0 (2020-07-23)

* New Features
  * [SIG-378] - Recovery procedure for deleted documents

* Improvements
  * [SIG-338] - Improve electronic signature description
  * [SIG-394] - Display participant actions of the document flow in alphabetic order
  * [SIG-395] - Refactor powered by position in the footer

* Bug fixes
  * [SIG-403] - Electronic signature with visual representation even with visual representations disabled

Updates database model: no

<a name="v1-8-0" />
### 1.8.0 (2020-07-16)

* New Features
  * [SIG-364] - Document Types for medical prescriptions

* Improvements
  * [SIG-337] - Updated fast signature button name
  * [SIG-362] - Create personal contacts list (LGPD adjustments)
  * [SIG-365] - Electronic signature with timestamp

* Bug fixes
  * [SIG-385] - Check if signer title is working when the flow has signature rules
  * [SIG-391] - Cannot add observers in the flow update
  * [SIG-392] - Fix Terms of use screen title

Updates database model: yes

<a name="v1-7-0" />
### 1.7.0 (2020-07-02)

* Bug fixes
  * [SIG-370] - Ticket parameter displayed in the Upload API documentation
  * [SIG-379] - Fix organization creation without Identifier (CNPJ)
  * [SIG-380] - Fix deed creation

* Improvements
  * [SIG-316] - Batch signature with HSM certificates
  * [SIG-317] - Changes to support Ecuador
  * [SIG-361] - Configure enabled/displayed document types
  * [SIG-376] - List documents with API key

Updates database model: no

<a name="v1-6-2" />
### 1.6.2 (2020-06-25)

* Bug fixes
  * [SIG-377] - Error viewing document details of a document with observer that is not in the flow

Updates database model: no

<a name="v1-6-1" />
### 1.6.1 (2020-06-24)

* Improvements
  * [SIG-374] - Add metallic-seaweed-emerald (MSE) theme

Updates database model: no

<a name="v1-6-0" />
### 1.6.0 (2020-06-24)

* New Features
  * [SIG-349] - Load document creation page with an upload file pre-loaded
  * [SIG-360] - Embedded signature integration

* Improvements
  * [SIG-227] - Simplify Swagger samples
  * [SIG-320] - Improve signature marks in printer friendly version for documents with a lot of signers
  * [SIG-327] - Update message in document upload validation to singular
  * [SIG-334] - Add document validation APIs documentation on Swagger
  * [SIG-335] - MoviDesk and JivoChat integration
  * [SIG-339] - Add Setting to configure if actions in the document flow should be ordered by default

* Bug fixes
  * [SIG-307] - Fix DevOps tests
  * [SIG-352] - Error while viewing user's events
  * [SIG-356] - Error while creating document if electronic signature is enabled and IsAllowedByDefault setting is true
  * [SIG-357] - Timeout retrieving document details with many participants
  * [SIG-358] - Missing translations in the edit flow email notification
  * [SIG-359] - Batch electronic signature is redirecting to Web PKI installation page

Updates database model: yes

<a name="v1-5-0" />
### 1.5.0 (2020-06-15)

* New Features
  * [SIG-331] - Send email to all participants after the document is concluded
  * [SIG-343] - Batch Electronic Signature
  * [SIG-344] - Option to configure if electronic signature is allowed by default

* Improvements
  * [SIG-311] - Setting to set geolocation as required for electronic signature
  * [SIG-318] - Allow participant to access the document after signing/approving in the public area
  * [SIG-326] - Automated tests for scanned document with Scanner
  * [SIG-332] - Add application name in the PDF properties
  * [SIG-341] - Hide printer friendly version

* Bug fixes
  * [SIG-347] - Fix translations in the document validation page

Updates database model: yes

<a name="v1-4-1" />
### 1.4.1 (2020-06-08)

* Bug fixes
  * [SIG-313] - Wrong internationalization (en) for the approval and sign email

Updates database model: no

<a name="v1-4-0" />
### 1.4.0 (2020-06-08)

* New Features
  * [SIG-216] - Instance settings to configure details of the print version

* Improvements
  * [SIG-249] - Add notification internationalization
  * [SIG-285] - Removed fast scan button and updated behaviour of the scan flow
  * [SIG-294] - Send set password email for new users
  * [SIG-312] - Add setting to configure if visual representation information should be placed in the middle of the rectangle
  * [SIG-314] - Improve Scanner integration settings
  * [SIG-323] - Enable batch download
  * [SIG-329] - Add more auditing events

* Bug fixes
  * [SIG-313] - Folder document status shown as Pending when it is concluded

Updates database model: yes

<a name="v1-3-2" />
### 1.3.2 (2020-05-15)

* Bug fixes
  * [SIG-310] - Exceptions while logging special characters from PKI SDK stack traces

Updates database model: no

<a name="v1-3-1" />
### 1.3.1 (2020-05-05)

* Bug fixes
  * [SIG-309] - Hide batch download until Web PKI update

Updates database model: no

<a name="v1-3-0" />
### 1.3.0 (2020-05-05)

* New Features
  * [SIG-178] - Batch download
  * [SIG-187] - Select signature format (CADeS or PADeS) in the document creation API
  * [SIG-190] - Enable administrators to view documents from users/organizations
  * [SIG-287] - Enable applications to generate a link to an external action

* Improvements
  * [SIG-161] - Enable administrators to update user data
  * [SIG-193] - Add link to PDF user manual
  * [SIG-262] - Improvements to Authentication funcionality (on Fast Signature)
  * [SIG-293] - Sign terms of service with electronic signature
  * [SIG-297] - Add document list in administration
  * [SIG-301] - Responsiveness fixes and removed scrolls that showed while loader was being displayed
  * [SIG-302] - Validate Adobe PDF signatures
  * [SIG-305] - Handle PinValidationFailed error from Amplia


* Bug fixes
  * [SIG-304] - Certificate issue requests that cannot be issued in Cloud should be ignored
  * [SIG-306] - Emails not being sent when SMS is disabled

Updates database model: **yes**

<a name="v1-2-0" />
### 1.2.0 (2020-04-29)

* New Features
  * [SIG-284] - Document validation of an uploaded signed file
  * [SIG-296] - Add settings to configure printer friendly version marks


* Improvements
  * [SIG-225] - Improved batch signature performance


* Bug fixes
  * [SIG-292] - Unified name and alias uses in SPA/Signer components
  * [SIG-295] - Fixed XAdES signatures without parameters
  * [SIG-298] - Error trying to obtain Brasilia timezone on Linux

Updates database model: **yes**

