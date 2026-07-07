# clicksend.DefaultApi

All URIs are relative to *https://rest.clicksend.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_allowed_email**](DefaultApi.md#add_allowed_email) | **POST** /v3/sms/email-sms | Add Allowed Email
[**agree_to_rules_and_regulation**](DefaultApi.md#agree_to_rules_and_regulation) | **POST** /v3/user-countries/agree | Agree to rules and regulation
[**calculate_email_campaign_price**](DefaultApi.md#calculate_email_campaign_price) | **POST** /v3/email-campaigns/price | Calculate Email Campaign Price
[**calculate_email_price**](DefaultApi.md#calculate_email_price) | **POST** /v3/email/price | Calculate Email Price
[**calculate_fax_price**](DefaultApi.md#calculate_fax_price) | **POST** /v3/fax/price | Calculate Fax Price
[**calculate_letter_price**](DefaultApi.md#calculate_letter_price) | **POST** /v3/post/letters/price | Calculate Letter Price
[**calculate_mms_campaign_price**](DefaultApi.md#calculate_mms_campaign_price) | **POST** /v3/mms-campaigns/price | Calculate MMS Campaign Price
[**calculate_mms_price**](DefaultApi.md#calculate_mms_price) | **POST** /v3/mms/price | Calculate MMS Price
[**calculate_postcard_price**](DefaultApi.md#calculate_postcard_price) | **POST** /v3/post/postcards/price | Calculate Postcard Price
[**calculate_sms_campaign_price**](DefaultApi.md#calculate_sms_campaign_price) | **POST** /v3/sms-campaigns/price | Calculate SMS Campaign Price
[**calculate_sms_price**](DefaultApi.md#calculate_sms_price) | **POST** /v3/sms/price | Calculate SMS Price
[**calculate_voice_price**](DefaultApi.md#calculate_voice_price) | **POST** /v3/voice/price | Calculate Voice Price
[**cancel_all_sms**](DefaultApi.md#cancel_all_sms) | **PUT** /v3/sms/cancel-all | Cancel All SMS
[**cancel_all_voice_messages**](DefaultApi.md#cancel_all_voice_messages) | **PUT** /v3/voice/cancel-all | Cancel All Voice Messages
[**cancel_email_campaign**](DefaultApi.md#cancel_email_campaign) | **PUT** /v3/email-campaigns/{email_campaign_id}/cancel | Cancel Email Campaign
[**cancel_mms_campaign**](DefaultApi.md#cancel_mms_campaign) | **PUT** /v3/mms-campaigns/{mms_campaign_id}/cancel | Cancel MMS Campaign
[**cancel_scheduled_letter**](DefaultApi.md#cancel_scheduled_letter) | **PUT** /v3/post/letters/{message_id}/cancel | Cancel Scheduled Letter
[**cancel_scheduled_postcard**](DefaultApi.md#cancel_scheduled_postcard) | **PUT** /v3/post/postcards/{message_id}/cancel | Cancel Scheduled Postcard
[**cancel_sms**](DefaultApi.md#cancel_sms) | **PUT** /v3/sms/{message_id}/cancel | Cancel SMS
[**cancel_sms_campaign**](DefaultApi.md#cancel_sms_campaign) | **PUT** /v3/sms-campaigns/{sms_campaign_id}/cancel | Cancel SMS Campaign
[**cancel_voice_message**](DefaultApi.md#cancel_voice_message) | **PUT** /v3/voice/{message_id}/cancel | Cancel Voice Message
[**copy_contact_to_list**](DefaultApi.md#copy_contact_to_list) | **PUT** /v3/lists/{from_list_id}/contacts/{contact_id}/copy/{to_list_id} | Copy Contact to List
[**create_allowed_email_address**](DefaultApi.md#create_allowed_email_address) | **POST** /v3/email/addresses | Create Allowed Email Address
[**create_default_sender**](DefaultApi.md#create_default_sender) | **POST** /v3/senders/default-senders | Create Default Sender
[**create_delivery_issue**](DefaultApi.md#create_delivery_issue) | **POST** /v3/delivery-issues | Create Delivery Issues
[**create_email_delivery_receipt_rule**](DefaultApi.md#create_email_delivery_receipt_rule) | **POST** /v3/automations/email/receipts | Create Email Delivery Receipt Rule
[**create_email_template**](DefaultApi.md#create_email_template) | **POST** /v3/email/templates | Create Email Template
[**create_fax_delivery_receipt_rule**](DefaultApi.md#create_fax_delivery_receipt_rule) | **POST** /v3/automations/fax/receipts | Create FAX Delivery Receipt Rule
[**create_fax_inbound_rule**](DefaultApi.md#create_fax_inbound_rule) | **POST** /v3/automations/fax/inbound | Create Fax Inbound Rule
[**create_list**](DefaultApi.md#create_list) | **POST** /v3/lists | Create List
[**create_new_contact**](DefaultApi.md#create_new_contact) | **POST** /v3/lists/{list_id}/contacts | Create New Contact
[**create_reseller_account**](DefaultApi.md#create_reseller_account) | **POST** /v3/reseller/accounts | Create Reseller Account
[**create_return_address**](DefaultApi.md#create_return_address) | **POST** /v3/post/return-addresses | Create Return Address
[**create_sms_delivery_receipt_rule**](DefaultApi.md#create_sms_delivery_receipt_rule) | **POST** /v3/automations/sms/receipts | Create SMS Delivery Receipt Rule
[**create_sms_inbound_automation**](DefaultApi.md#create_sms_inbound_automation) | **POST** /v3/automations/sms/inbound | Create SMS Inbound Automation
[**create_sms_template**](DefaultApi.md#create_sms_template) | **POST** /v3/sms/templates | Create SMS Template
[**create_stripped_string_rule**](DefaultApi.md#create_stripped_string_rule) | **POST** /v3/sms/email-sms-stripped-strings | Create Stripped String Rule
[**create_subaccount**](DefaultApi.md#create_subaccount) | **POST** /v3/subaccounts | Create Subaccount
[**create_test_inbound_sms**](DefaultApi.md#create_test_inbound_sms) | **POST** /v3/sms/inbound | Create Test Inbound SMS
[**create_test_sms_receipt**](DefaultApi.md#create_test_sms_receipt) | **POST** /v3/sms/receipts | Create Test SMS Receipt
[**create_voice_delivery_receipt_rule**](DefaultApi.md#create_voice_delivery_receipt_rule) | **POST** /v3/automations/voice/receipts | Create Voice Delivery Receipt Rule
[**current_payment_info**](DefaultApi.md#current_payment_info) | **GET** /v3/recharge/credit-card | Current Payment Info
[**delete_allowed_email_address**](DefaultApi.md#delete_allowed_email_address) | **DELETE** /v3/email/addresses/{email_address_id} | Delete Allowed Email Address
[**delete_alpha_tag**](DefaultApi.md#delete_alpha_tag) | **DELETE** /v3/alpha-tags/{alpha_tag_id} | Delete Alpha Tag
[**delete_contact**](DefaultApi.md#delete_contact) | **DELETE** /v3/lists/{list_id}/contacts/{contact_id} | Delete Contact
[**delete_default_sender**](DefaultApi.md#delete_default_sender) | **DELETE** /v3/senders/default-senders/{default_sender_id} | Delete Default Sender
[**delete_email_delivery_receipt_rule**](DefaultApi.md#delete_email_delivery_receipt_rule) | **DELETE** /v3/automations/email/receipts/{receipt_rule_id} | Delete Email Delivery Receipt Rule
[**delete_email_template**](DefaultApi.md#delete_email_template) | **DELETE** /v3/email/templates/{template_id} | Delete Email Template
[**delete_fax_delivery_receipt_rule**](DefaultApi.md#delete_fax_delivery_receipt_rule) | **DELETE** /v3/automations/fax/receipts/{receipt_rule_id} | Delete FAX Delivery Receipt Rule
[**delete_fax_inbound_rule**](DefaultApi.md#delete_fax_inbound_rule) | **DELETE** /v3/automations/fax/inbound/{inbound_rule_id} | Delete Fax Inbound Rule
[**delete_list**](DefaultApi.md#delete_list) | **DELETE** /v3/lists/{list_id} | Delete List
[**delete_own_number**](DefaultApi.md#delete_own_number) | **DELETE** /v3/own-numbers/{own_number_id} | Delete Own Number
[**delete_return_address**](DefaultApi.md#delete_return_address) | **DELETE** /v3/post/return-addresses/{return_address_id} | Delete Return Address
[**delete_sms_delivery_receipt_rule**](DefaultApi.md#delete_sms_delivery_receipt_rule) | **DELETE** /v3/automations/sms/receipts/{receipt_rule_id} | Delete SMS Delivery Receipt Rule
[**delete_sms_inbound_automation**](DefaultApi.md#delete_sms_inbound_automation) | **DELETE** /v3/automations/sms/inbound/{inbound_rule_id} | Delete SMS Inbound Automation
[**delete_sms_template**](DefaultApi.md#delete_sms_template) | **DELETE** /v3/sms/templates/{template_id} | Delete SMS Template
[**delete_stripped_string_rule**](DefaultApi.md#delete_stripped_string_rule) | **DELETE** /v3/sms/email-sms-stripped-strings/{rule_id} | Delete Stripped String Rule
[**delete_subaccount**](DefaultApi.md#delete_subaccount) | **DELETE** /v3/subaccounts/{subaccount_id} | Delete Subaccount
[**delete_voice_delivery_receipt_rule**](DefaultApi.md#delete_voice_delivery_receipt_rule) | **DELETE** /v3/automations/voice/receipts/{receipt_rule_id} | Delete Voice Delivery Receipt Rule
[**detect_address**](DefaultApi.md#detect_address) | **POST** /v3/post/letters/detect-address | Detect Address
[**export_email_campaign_history**](DefaultApi.md#export_email_campaign_history) | **GET** /v3/email-campaigns/{email_campaign_id}/history/export | Export Email Campaign History
[**export_email_history**](DefaultApi.md#export_email_history) | **GET** /v3/email/history/export | Export Email History
[**export_letter_history**](DefaultApi.md#export_letter_history) | **GET** /v3/post/letters/history/export | Export Letter History
[**export_mms_history**](DefaultApi.md#export_mms_history) | **GET** /v3/mms/history/export | Export MMS History
[**export_postcard_history**](DefaultApi.md#export_postcard_history) | **GET** /v3/post/postcards/history/export | Export Postcard History
[**export_sms_history**](DefaultApi.md#export_sms_history) | **GET** /v3/sms/history/export | Export SMS History
[**export_voice_history**](DefaultApi.md#export_voice_history) | **GET** /v3/voice/history/export | Export Voice History
[**forgot_password**](DefaultApi.md#forgot_password) | **PUT** /v3/forgot-password | Forgot Password
[**forgot_username**](DefaultApi.md#forgot_username) | **PUT** /v3/forgot-username | Forgot Username
[**generate_new_api_key**](DefaultApi.md#generate_new_api_key) | **PUT** /v3/subaccounts/{subaccount_id}/regen-api-key | Generate New API Key
[**get_all_delivery_issues**](DefaultApi.md#get_all_delivery_issues) | **GET** /v3/delivery-issues | Get All Delivery Issues
[**get_alpha_tag**](DefaultApi.md#get_alpha_tag) | **GET** /v3/alpha-tags/{alpha_tag_id} | Get Alpha Tag
[**get_countries_for_global_sending**](DefaultApi.md#get_countries_for_global_sending) | **GET** /v3/user-countries | Get Countries for Global Sending
[**get_default_sender_details**](DefaultApi.md#get_default_sender_details) | **GET** /v3/senders/default-senders/{default_sender_id} | Get Default Sender Details
[**get_default_senders_list**](DefaultApi.md#get_default_senders_list) | **GET** /v3/senders/default-senders | Get List of Default Senders
[**get_own_number_detail**](DefaultApi.md#get_own_number_detail) | **GET** /v3/own-numbers/{own_number_id} | Get Own Number Detail
[**get_specific_contact**](DefaultApi.md#get_specific_contact) | **GET** /v3/lists/{list_id}/contacts/{contact_id} | Get Specific Contact
[**get_voice_history**](DefaultApi.md#get_voice_history) | **GET** /v3/voice/history | Get Voice History
[**import_contacts**](DefaultApi.md#import_contacts) | **POST** /v3/lists/{list_id}/import | Import Contacts
[**list_alpha_tags**](DefaultApi.md#list_alpha_tags) | **GET** /v3/alpha-tags | List Alpha Tags
[**list_compliant_sender_types**](DefaultApi.md#list_compliant_sender_types) | **GET** /v3/senders/compliant-sender-types | List Compliant Sender Types
[**list_countries**](DefaultApi.md#list_countries) | **GET** /v3/country-list | International Messaging
[**list_own_numbers**](DefaultApi.md#list_own_numbers) | **GET** /v3/own-numbers | List Own Numbers
[**mark_inbound_sms_as_read**](DefaultApi.md#mark_inbound_sms_as_read) | **PUT** /v3/sms/inbound-read | Mark Inbound SMS as Read
[**mark_sms_receipt_as_read**](DefaultApi.md#mark_sms_receipt_as_read) | **PUT** /v3/sms/receipts-read | Mark SMS Receipt As Read
[**mark_specific_inbound_sms_message_as_read**](DefaultApi.md#mark_specific_inbound_sms_message_as_read) | **PUT** /v3/sms/inbound-read/{message_id} | Mark Specific Inbound SMS Message As Read
[**purchase_dedicated_number**](DefaultApi.md#purchase_dedicated_number) | **POST** /v3/numbers/buy/{dedicated_number} | Purchase Dedicated Number
[**purchase_recharge_package**](DefaultApi.md#purchase_recharge_package) | **PUT** /v3/recharge/purchase/{package_id} | Purchase Recharge Package
[**register_numbers**](DefaultApi.md#register_numbers) | **POST** /v3/numbers/registrations/number-types/{number_type}/country/{country_code} | Register Numbers
[**remove_duplicate_contacts**](DefaultApi.md#remove_duplicate_contacts) | **PUT** /v3/lists/{list_id}/remove-duplicates/ | Remove Duplicate Contacts
[**remove_opted_out_contacts**](DefaultApi.md#remove_opted_out_contacts) | **PUT** /v3/lists/{list_id}/remove-opted-out-contacts/{opt_out_list_id} | Remove Opted Out Contacts
[**request_alpha_tag**](DefaultApi.md#request_alpha_tag) | **POST** /v3/alpha-tags | Request Alpha Tag
[**request_own_number_verification_otp**](DefaultApi.md#request_own_number_verification_otp) | **POST** /v3/own-numbers/verifications | Request Own Number Verification OTP
[**reseller_transfer_credit**](DefaultApi.md#reseller_transfer_credit) | **PUT** /v3/reseller/transfer-credit | Reseller Transfer Credit
[**select_countries_for_global_sending**](DefaultApi.md#select_countries_for_global_sending) | **POST** /v3/user-countries | Select Countries for Global Sending
[**send_email**](DefaultApi.md#send_email) | **POST** /v3/email/send | Send Email
[**send_email_campaign**](DefaultApi.md#send_email_campaign) | **POST** /v3/email-campaigns/send | Send Email Campaign
[**send_email_verification_token**](DefaultApi.md#send_email_verification_token) | **PUT** /v3/email/address-verify/{email_address_id}/send | Send Email Verification Token
[**send_fax**](DefaultApi.md#send_fax) | **POST** /v3/fax/send | Send Fax
[**send_letter**](DefaultApi.md#send_letter) | **POST** /v3/post/letters/send | Send Letter
[**send_mms**](DefaultApi.md#send_mms) | **POST** /v3/mms/send | Send MMS
[**send_mms_campaign**](DefaultApi.md#send_mms_campaign) | **POST** /v3/mms-campaigns/send | Send MMS Campaign
[**send_postcard**](DefaultApi.md#send_postcard) | **POST** /v3/post/postcards/send | Send Postcard
[**send_sms**](DefaultApi.md#send_sms) | **POST** /v3/sms/send | Send SMS
[**send_sms_campaign**](DefaultApi.md#send_sms_campaign) | **POST** /v3/sms-campaigns/send | Send SMS Campaign
[**send_voice_message**](DefaultApi.md#send_voice_message) | **POST** /v3/voice/send | Send Voice Message
[**short_url_get_statistics**](DefaultApi.md#short_url_get_statistics) | **GET** /v3/short-url/statistics/{source}/{source_id} | Get Statistics
[**short_url_get_tracking**](DefaultApi.md#short_url_get_tracking) | **GET** /v3/short-url/tracking/{long_url_id} | Get Tracking
[**timezones**](DefaultApi.md#timezones) | **GET** /v3/timezones | Timezones
[**transfer_contact_to_list**](DefaultApi.md#transfer_contact_to_list) | **PUT** /v3/lists/{from_list_id}/contacts/{contact_id}/transfer/{to_list_id} | Transfer Contact to List
[**update_client_account**](DefaultApi.md#update_client_account) | **PUT** /v3/reseller/accounts/{client_user_id} | Update Client Account
[**update_contact**](DefaultApi.md#update_contact) | **PUT** /v3/lists/{list_id}/contacts/{contact_id} | Update Contact
[**update_default_sender**](DefaultApi.md#update_default_sender) | **PATCH** /v3/senders/default-senders/{default_sender_id} | Update Default Sender
[**update_email_campaign**](DefaultApi.md#update_email_campaign) | **PUT** /v3/email-campaigns/{email_campaign_id} | Update Email Campaign
[**update_email_delivery_receipt_rule**](DefaultApi.md#update_email_delivery_receipt_rule) | **PUT** /v3/automations/email/receipts/{receipt_rule_id} | Update Email Delivery Receipt Rule
[**update_email_template**](DefaultApi.md#update_email_template) | **PUT** /v3/email/templates/{template_id} | Update Email Template
[**update_fax_delivery_receipt_rule**](DefaultApi.md#update_fax_delivery_receipt_rule) | **PUT** /v3/automations/fax/receipts/{receipt_rule_id} | Update FAX Delivery Receipt Rule
[**update_fax_inbound_rule**](DefaultApi.md#update_fax_inbound_rule) | **PUT** /v3/automations/fax/inbound/{inbound_rule_id} | Update Fax Inbound Rule
[**update_list**](DefaultApi.md#update_list) | **PUT** /v3/lists/{list_id} | Update List
[**update_mms_campaign**](DefaultApi.md#update_mms_campaign) | **PUT** /v3/mms-campaigns/{mms_campaign_id} | Update MMS Campaign
[**update_own_number**](DefaultApi.md#update_own_number) | **PATCH** /v3/own-numbers/{own_number_id} | Update Own Number
[**update_payment_info**](DefaultApi.md#update_payment_info) | **PUT** /v3/recharge/credit-card | Update Payment Info
[**update_return_address**](DefaultApi.md#update_return_address) | **PUT** /v3/post/return-addresses/{return_address_id} | Update Return Address
[**update_sms_campaign**](DefaultApi.md#update_sms_campaign) | **PUT** /v3/sms-campaigns/{sms_campaign_id} | Update SMS Campaign
[**update_sms_delivery_receipt_rule**](DefaultApi.md#update_sms_delivery_receipt_rule) | **PUT** /v3/automations/sms/receipts/{receipt_rule_id} | Update SMS Delivery Receipt Rule
[**update_sms_inbound_automation**](DefaultApi.md#update_sms_inbound_automation) | **PUT** /v3/automations/sms/inbound/{inbound_rule_id} | Update SMS Inbound Automation
[**update_sms_template**](DefaultApi.md#update_sms_template) | **PUT** /v3/sms/templates/{template_id} | Update SMS Template
[**update_stripped_string_rule**](DefaultApi.md#update_stripped_string_rule) | **PUT** /v3/sms/email-sms-stripped-strings/{rule_id} | Update Stripped String Rule
[**update_subaccount**](DefaultApi.md#update_subaccount) | **PUT** /v3/subaccounts/{subaccount_id} | Update Subaccount
[**update_voice_delivery_receipt_rule**](DefaultApi.md#update_voice_delivery_receipt_rule) | **PUT** /v3/automations/voice/receipts/{receipt_rule_id} | Update Voice Delivery Receipt Rule
[**upload_a_media_file**](DefaultApi.md#upload_a_media_file) | **POST** /v3/uploads | Upload Media File
[**verify_allowed_email_address**](DefaultApi.md#verify_allowed_email_address) | **PUT** /v3/email/address-verify/{email_address_id}/verify/{activation_token} | Verify Allowed Email Address
[**verify_own_number_otp**](DefaultApi.md#verify_own_number_otp) | **POST** /v3/own-numbers/verifications/{verification_id}/verify | Verify Own Number OTP
[**view_a_specific_inbound_sms_message**](DefaultApi.md#view_a_specific_inbound_sms_message) | **GET** /v3/sms/inbound/{original_message_id} | View a specific inbound SMS message
[**view_a_specific_sms_template**](DefaultApi.md#view_a_specific_sms_template) | **GET** /v3/sms/templates/{template_id} | View a Specific SMS Template
[**view_account_details**](DefaultApi.md#view_account_details) | **GET** /v3/account | View Account Details
[**view_account_usage**](DefaultApi.md#view_account_usage) | **GET** /v3/account/usage/{year}/{month}/subaccount | View Account Usage
[**view_all_email_campaigns**](DefaultApi.md#view_all_email_campaigns) | **GET** /v3/email-campaigns | View All Email Campaigns
[**view_all_mms_campaigns**](DefaultApi.md#view_all_mms_campaigns) | **GET** /v3/mms-campaigns | View All MMS Campaigns
[**view_all_transactions**](DefaultApi.md#view_all_transactions) | **GET** /v3/recharge/transactions | View All Transactions
[**view_allowed_email_address**](DefaultApi.md#view_allowed_email_address) | **GET** /v3/email/addresses/{email_address_id} | View Allowed Email Address
[**view_allowed_email_addresses**](DefaultApi.md#view_allowed_email_addresses) | **GET** /v3/email/addresses | View Allowed Email Addresses
[**view_allowed_emails**](DefaultApi.md#view_allowed_emails) | **GET** /v3/sms/email-sms | View Allowed Emails
[**view_available_numbers**](DefaultApi.md#view_available_numbers) | **GET** /v3/numbers/search/{country} | View Available Numbers
[**view_client_accounts**](DefaultApi.md#view_client_accounts) | **GET** /v3/reseller/accounts | View Client Accounts
[**view_contact_lists**](DefaultApi.md#view_contact_lists) | **GET** /v3/search/contacts-lists | View Contact Lists
[**view_countries**](DefaultApi.md#view_countries) | **GET** /v3/countries | View Countries
[**view_email_campaign**](DefaultApi.md#view_email_campaign) | **GET** /v3/email-campaigns/{email_campaign_id} | View Email Campaign
[**view_email_campaign_history**](DefaultApi.md#view_email_campaign_history) | **GET** /v3/email-campaigns/{email_campaign_id}/history | View Email Campaign History
[**view_email_delivery_receipt_rule**](DefaultApi.md#view_email_delivery_receipt_rule) | **GET** /v3/automations/email/receipts/{receipt_rule_id} | View Email Delivery Receipt Rule
[**view_email_delivery_receipt_rules**](DefaultApi.md#view_email_delivery_receipt_rules) | **GET** /v3/automations/email/receipts | View Email Delivery Receipt Rules
[**view_email_history**](DefaultApi.md#view_email_history) | **GET** /v3/email/history | View Email History
[**view_email_template**](DefaultApi.md#view_email_template) | **GET** /v3/email/templates/{template_id} | View Email Template
[**view_email_templates**](DefaultApi.md#view_email_templates) | **GET** /v3/email/templates | View Email Templates
[**view_fax_delivery_receipt_rule**](DefaultApi.md#view_fax_delivery_receipt_rule) | **GET** /v3/automations/fax/receipts/{receipt_rule_id} | View FAX Delivery Receipt Rule
[**view_fax_delivery_receipt_rules**](DefaultApi.md#view_fax_delivery_receipt_rules) | **GET** /v3/automations/fax/receipts | View FAX Delivery Receipt Rules
[**view_fax_history**](DefaultApi.md#view_fax_history) | **GET** /v3/fax/history | View Fax History
[**view_fax_inbound_rule**](DefaultApi.md#view_fax_inbound_rule) | **GET** /v3/automations/fax/inbound/{inbound_rule_id} | View Fax Inbound Rule
[**view_fax_inbound_rules**](DefaultApi.md#view_fax_inbound_rules) | **GET** /v3/automations/fax/inbound | View Fax Inbound Rules
[**view_fax_receipts**](DefaultApi.md#view_fax_receipts) | **GET** /v3/fax/receipts | View Fax Receipts
[**view_inbound_sms**](DefaultApi.md#view_inbound_sms) | **GET** /v3/sms/inbound | View Inbound SMS
[**view_letter_history**](DefaultApi.md#view_letter_history) | **GET** /v3/post/letters/history | View Letter History
[**view_list_contacts**](DefaultApi.md#view_list_contacts) | **GET** /v3/lists/{list_id}/contacts | View List Contacts
[**view_lists**](DefaultApi.md#view_lists) | **GET** /v3/lists | View Lists
[**view_master_email_template**](DefaultApi.md#view_master_email_template) | **GET** /v3/email/master-templates/{template_id} | View Master Email Template
[**view_master_email_templates**](DefaultApi.md#view_master_email_templates) | **GET** /v3/email/master-templates | View Master Email Templates
[**view_mms_campaign**](DefaultApi.md#view_mms_campaign) | **GET** /v3/mms-campaigns/{mms_campaign_id} | View MMS Campaign
[**view_mms_history**](DefaultApi.md#view_mms_history) | **GET** /v3/mms/history | View MMS History
[**view_postcard_history**](DefaultApi.md#view_postcard_history) | **GET** /v3/post/postcards/history | View Postcard History
[**view_recharge_packages**](DefaultApi.md#view_recharge_packages) | **GET** /v3/recharge/packages | View Recharge Packages
[**view_referral_accounts**](DefaultApi.md#view_referral_accounts) | **GET** /v3/referral/accounts/ | View Referral Accounts
[**view_sms_campaigns**](DefaultApi.md#view_sms_campaigns) | **GET** /v3/sms-campaigns | View SMS Campaigns
[**view_sms_delivery_receipt_rule**](DefaultApi.md#view_sms_delivery_receipt_rule) | **GET** /v3/automations/sms/receipts/{receipt_rule_id} | View SMS Delivery Receipt Rule
[**view_sms_delivery_receipt_rules**](DefaultApi.md#view_sms_delivery_receipt_rules) | **GET** /v3/automations/sms/receipts | View SMS Delivery Receipt Rules
[**view_sms_history**](DefaultApi.md#view_sms_history) | **GET** /v3/sms/history | View SMS History
[**view_sms_inbound_automation**](DefaultApi.md#view_sms_inbound_automation) | **GET** /v3/automations/sms/inbound/{inbound_rule_id} | View SMS Inbound Automation
[**view_sms_inbound_automations**](DefaultApi.md#view_sms_inbound_automations) | **GET** /v3/automations/sms/inbound | View SMS Inbound Automations
[**view_sms_receipts**](DefaultApi.md#view_sms_receipts) | **GET** /v3/sms/receipts | View SMS Receipts
[**view_sms_statistics**](DefaultApi.md#view_sms_statistics) | **GET** /v3/statistics/sms | View SMS Statistics
[**view_sms_templates**](DefaultApi.md#view_sms_templates) | **GET** /v3/sms/templates | View SMS Templates
[**view_specific_client_account**](DefaultApi.md#view_specific_client_account) | **GET** /v3/reseller/accounts/{client_user_id} | View Specific Client Account
[**view_specific_fax_receipt**](DefaultApi.md#view_specific_fax_receipt) | **GET** /v3/fax/receipts/{message_id} | View Specific Fax Receipt
[**view_specific_list**](DefaultApi.md#view_specific_list) | **GET** /v3/lists/{list_id} | View Specific List
[**view_specific_return_address**](DefaultApi.md#view_specific_return_address) | **GET** /v3/post/return-addresses/{return_address_id} | View Specific Return Address
[**view_specific_sms_campaign**](DefaultApi.md#view_specific_sms_campaign) | **GET** /v3/sms-campaigns/{sms_campaign_id} | View Specific SMS Campaign
[**view_specific_sms_receipt**](DefaultApi.md#view_specific_sms_receipt) | **GET** /v3/sms/receipts/{message_id} | View Specific SMS Receipt
[**view_specific_subaccount**](DefaultApi.md#view_specific_subaccount) | **GET** /v3/subaccounts/{subaccount_id} | View Specific Subaccount
[**view_specific_transaction**](DefaultApi.md#view_specific_transaction) | **GET** /v3/recharge/transactions/{transaction_id} | View Specific Transaction
[**view_stripped_string_rule**](DefaultApi.md#view_stripped_string_rule) | **GET** /v3/sms/email-sms-stripped-strings/{rule_id} | View Stripped String Rule
[**view_stripped_string_rules**](DefaultApi.md#view_stripped_string_rules) | **GET** /v3/sms/email-sms-stripped-strings | View Stripped String Rules
[**view_subaccounts**](DefaultApi.md#view_subaccounts) | **GET** /v3/subaccounts | View Subaccounts
[**view_template_categories**](DefaultApi.md#view_template_categories) | **GET** /v3/email/master-templates-categories | View Template Categories
[**view_template_category**](DefaultApi.md#view_template_category) | **GET** /v3/email/master-templates-categories/{category_id} | View Template Category
[**view_templates_in_category**](DefaultApi.md#view_templates_in_category) | **GET** /v3/email/master-templates-categories/{category_id}/master-templates | View Templates in Category
[**view_voice_delivery_receipt_rule**](DefaultApi.md#view_voice_delivery_receipt_rule) | **GET** /v3/automations/voice/receipts/{receipt_rule_id} | View Voice Delivery Receipt Rule
[**view_voice_delivery_receipt_rules**](DefaultApi.md#view_voice_delivery_receipt_rules) | **GET** /v3/automations/voice/receipts | View Voice Delivery Receipt Rules
[**view_voice_languages**](DefaultApi.md#view_voice_languages) | **GET** /v3/voice/lang | View Voice Languages
[**view_voice_receipts**](DefaultApi.md#view_voice_receipts) | **GET** /v3/voice/receipts | View Voice Receipts
[**view_voice_statistics**](DefaultApi.md#view_voice_statistics) | **GET** /v3/statistics/voice | View Voice Statistics
[**view_your_numbers**](DefaultApi.md#view_your_numbers) | **GET** /v3/numbers | View Your Numbers
[**view_your_return_addresses**](DefaultApi.md#view_your_return_addresses) | **GET** /v3/post/return-addresses | View Your Return Addresses


# **add_allowed_email**
> AddAllowedEmail add_allowed_email(content_type=content_type, add_allowed_email_request=add_allowed_email_request)

Add Allowed Email

_Create email to sms allowed address_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| email_address | string | true | none | Your email address |
| from | string | false | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.add_allowed_email import AddAllowedEmail
from clicksend.models.add_allowed_email_request import AddAllowedEmailRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    add_allowed_email_request = clicksend.AddAllowedEmailRequest() # AddAllowedEmailRequest |  (optional)

    try:
        # Add Allowed Email
        api_response = api_instance.add_allowed_email(content_type=content_type, add_allowed_email_request=add_allowed_email_request)
        print("The response of DefaultApi->add_allowed_email:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->add_allowed_email: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **add_allowed_email_request** | [**AddAllowedEmailRequest**](AddAllowedEmailRequest.md)|  | [optional] 

### Return type

[**AddAllowedEmail**](AddAllowedEmail.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **agree_to_rules_and_regulation**
> AgreeToRulesAndRegulation agree_to_rules_and_regulation()

Agree to rules and regulation

_Update Country Rule_

To agree on rules and regulations of selected countries and confirm selection.

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| country_list_ids | number | true | none | Country list ID's |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.agree_to_rules_and_regulation import AgreeToRulesAndRegulation
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)

    try:
        # Agree to rules and regulation
        api_response = api_instance.agree_to_rules_and_regulation()
        print("The response of DefaultApi->agree_to_rules_and_regulation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->agree_to_rules_and_regulation: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**AgreeToRulesAndRegulation**](AgreeToRulesAndRegulation.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **calculate_email_campaign_price**
> CalculateEmailCampaignPrice calculate_email_campaign_price(content_type=content_type, calculate_email_campaign_price_request=calculate_email_campaign_price_request)

Calculate Email Campaign Price

_Calculate email campaign price_

Calculate email campaign price

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| name | string | true | none | Your campaign name. |
| subject | string | true | none | Your campaign subject. |
| body | string | true | none | Your campaign message. |
| from_email_address_id | number | true | none | The allowed email address id. |
| from_name | string | true | none | Your name or business name. |
| template_id | number | false | none | Your template id. |
| list_id | number | true | none | Your contact list id. |
| schedule | integer(int32) | false | none | Your schedule timestamp. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_email_campaign_price import CalculateEmailCampaignPrice
from clicksend.models.calculate_email_campaign_price_request import CalculateEmailCampaignPriceRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    calculate_email_campaign_price_request = clicksend.CalculateEmailCampaignPriceRequest() # CalculateEmailCampaignPriceRequest |  (optional)

    try:
        # Calculate Email Campaign Price
        api_response = api_instance.calculate_email_campaign_price(content_type=content_type, calculate_email_campaign_price_request=calculate_email_campaign_price_request)
        print("The response of DefaultApi->calculate_email_campaign_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->calculate_email_campaign_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **calculate_email_campaign_price_request** | [**CalculateEmailCampaignPriceRequest**](CalculateEmailCampaignPriceRequest.md)|  | [optional] 

### Return type

[**CalculateEmailCampaignPrice**](CalculateEmailCampaignPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **calculate_email_price**
> CalculateEmailPrice calculate_email_price(content_type=content_type, calculate_email_price_request=calculate_email_price_request)

Calculate Email Price

_Get transactional email price_

Get transactional email price

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| to | array | true | none | Array of To Recipient items. (array of names and emails) |
| cc | array | false | none | Array of Cc Recipient items. (array of names and emails) |
| bcc | array | false | none | Array of Bcc Recipient items. (array of names and emails) |
| from | object | true | none | From Email object. (object containing name and email) |
| body | string | true | none | Body of the email. |
| attachments | array | false | none | Array of Attachment items. |
| schedule | number | false | none | Schedule. |
| name | string | false | none | Name of person email belongs to |
| email | string | true | none | Email to be used. |
| content | string | true | none | The base64-encoded contents of the file. |
| type | string | true | none | The type of file being attached. |
| filename | string | true | none | The name of the file being attached. |
| disposition | string | true | none | Inline for content that can be displayed within the email, or attachment for any other files. |
| content_id | string | true | none | An ID for the content. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_email_price import CalculateEmailPrice
from clicksend.models.calculate_email_price_request import CalculateEmailPriceRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    calculate_email_price_request = clicksend.CalculateEmailPriceRequest() # CalculateEmailPriceRequest |  (optional)

    try:
        # Calculate Email Price
        api_response = api_instance.calculate_email_price(content_type=content_type, calculate_email_price_request=calculate_email_price_request)
        print("The response of DefaultApi->calculate_email_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->calculate_email_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **calculate_email_price_request** | [**CalculateEmailPriceRequest**](CalculateEmailPriceRequest.md)|  | [optional] 

### Return type

[**CalculateEmailPrice**](CalculateEmailPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **calculate_fax_price**
> CalculateFaxPrice calculate_fax_price(content_type=content_type, calculate_fax_price_request=calculate_fax_price_request)

Calculate Fax Price

_Calculate Total Price for Fax Messages sent_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| file_url | string | true | none | URL of file to send |
| source | string | true | none | Your method of sending e.g. 'wordpress', 'php', 'c#'. |
| to | string | true | none | Recipient fax number in [E.164](https://en.wikipedia.org/wiki/E.164) format. |
| list_id | integer(int32) | false | none | Your list ID if sending to a whole list. Can be used instead of 'to'. |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id. Must be a valid fax number. |
| schedule | integer(int32) | false | none | Leave blank for immediate delivery. Your schedule time in unix format [http://help.clicksend.com/what-is-a-unix-timestamp](http://help.clicksend.com/what-is-a-unix-timestamp) |
| custom_string | string | false | none | Your reference. Will be passed back with all replies and delivery reports. |
| country | string | false | none | ISO alpha-2 character country code e.g. 'US', we use this to format the recipient number if it's not in international format. |
| from_email | string | false | none | An email address where the reply should be emailed to. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_fax_price import CalculateFaxPrice
from clicksend.models.calculate_fax_price_request import CalculateFaxPriceRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    calculate_fax_price_request = clicksend.CalculateFaxPriceRequest() # CalculateFaxPriceRequest |  (optional)

    try:
        # Calculate Fax Price
        api_response = api_instance.calculate_fax_price(content_type=content_type, calculate_fax_price_request=calculate_fax_price_request)
        print("The response of DefaultApi->calculate_fax_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->calculate_fax_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **calculate_fax_price_request** | [**CalculateFaxPriceRequest**](CalculateFaxPriceRequest.md)|  | [optional] 

### Return type

[**CalculateFaxPrice**](CalculateFaxPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **calculate_letter_price**
> CalculateLetterPrice calculate_letter_price(content_type=content_type, calculate_letter_price_request=calculate_letter_price_request)

Calculate Letter Price

_Calculate letter price_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| file_url | string | true | none | URL of file to send |
| address_name | string | true | none | Name of address |
| address_line_1 | string | true | none | First line of address |
| address_line_2 | string | true | none | Second line of address |
| address_city | string | true | none | City |
| address_state | string | true | none | State |
| address_postal_code | string | true | none | Postal code |
| address_country | string | true | none | Country |
| return_address_id | integer(int32) | true | none | ID of return address to use |
| schedule | integer(int32) | false | none | When to send letter (0/null=now) |
| template_used | integer(int1) | false | none | Whether using our letter template. Flag value must be 1 for yes or 0 for no. |
| duplex | integer(int1) | false | none | Whether letter is duplex. Flag value must be 1 for yes or 0 for no. |
| colour | integer(int1) | false | none | Whether letter is in colour. Flag value must be 1 for yes or 0 for no. |
| priority_post | integer(int1) | false | none | Whether letter is priority. Flag value must be 1 for yes or 0 for no. |
| source | string | false | none | Source being sent from |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_letter_price import CalculateLetterPrice
from clicksend.models.calculate_letter_price_request import CalculateLetterPriceRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    calculate_letter_price_request = clicksend.CalculateLetterPriceRequest() # CalculateLetterPriceRequest |  (optional)

    try:
        # Calculate Letter Price
        api_response = api_instance.calculate_letter_price(content_type=content_type, calculate_letter_price_request=calculate_letter_price_request)
        print("The response of DefaultApi->calculate_letter_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->calculate_letter_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **calculate_letter_price_request** | [**CalculateLetterPriceRequest**](CalculateLetterPriceRequest.md)|  | [optional] 

### Return type

[**CalculateLetterPrice**](CalculateLetterPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **calculate_mms_campaign_price**
> CalculateMmsCampaignPrice calculate_mms_campaign_price(content_type=content_type, body=body)

Calculate MMS Campaign Price

_Calculate price for mms campaign_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| list_id | integer(int32) | true | none | Your list id. |
| name | string | true | none | Your campaign name. |
| body | string | true | none | Your campaign message. |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id |
| schedule | integer(int32) | false | none | Your schedule timestamp. |
| subject | string | true | none | Subject of MMS campaign. |
| media_file | string | true | none | URL pointing to media file. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_mms_campaign_price import CalculateMmsCampaignPrice
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    body = None # object |  (optional)

    try:
        # Calculate MMS Campaign Price
        api_response = api_instance.calculate_mms_campaign_price(content_type=content_type, body=body)
        print("The response of DefaultApi->calculate_mms_campaign_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->calculate_mms_campaign_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

[**CalculateMmsCampaignPrice**](CalculateMmsCampaignPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **calculate_mms_price**
> CalculateMmsPrice calculate_mms_price(content_type=content_type, calculate_mms_price_request=calculate_mms_price_request)

Calculate MMS Price

_Get Price for MMS sent_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| media_file | string | true | none | Media file you want to send |
| to | string | true | none | Recipient phone number in [E.164](https://en.wikipedia.org/wiki/E.164) format |
| body | string | true | none | Your message |
| subject | string | true | none | Subject line (max 20 characters) |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_mms_price import CalculateMmsPrice
from clicksend.models.calculate_mms_price_request import CalculateMmsPriceRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    calculate_mms_price_request = clicksend.CalculateMmsPriceRequest() # CalculateMmsPriceRequest |  (optional)

    try:
        # Calculate MMS Price
        api_response = api_instance.calculate_mms_price(content_type=content_type, calculate_mms_price_request=calculate_mms_price_request)
        print("The response of DefaultApi->calculate_mms_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->calculate_mms_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **calculate_mms_price_request** | [**CalculateMmsPriceRequest**](CalculateMmsPriceRequest.md)|  | [optional] 

### Return type

[**CalculateMmsPrice**](CalculateMmsPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **calculate_postcard_price**
> CalculatePostcardPrice calculate_postcard_price(content_type=content_type, send_postcard_request=send_postcard_request)

Calculate Postcard Price

_Calculate price for sending one or more postcards_

For `file_urls` field. You can attach at least 1 and max of 2 PDF file urls.

- Supply a single pdf with 2 pages (front and back)
- Supply 2 urls to seperate PDFs
    

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| file_urls | \[string\] | true | none | Postcard file URLs |
| address_name | string | true | none | Name of address |
| address_line_1 | string | true | none | First line of address |
| address_line_2 | string | true | none | Second line of address |
| address_city | string | true | none | City |
| address_state | string | true | none | State |
| address_postal_code | string | true | none | Postal code |
| address_country | string | true | none | Country |
| return_address_id | integer(int32) | true | none | ID of return address to use |
| schedule | integer(int32) | false | none | When to send letter (0/null=now) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_postcard_price import CalculatePostcardPrice
from clicksend.models.send_postcard_request import SendPostcardRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_postcard_request = clicksend.SendPostcardRequest() # SendPostcardRequest |  (optional)

    try:
        # Calculate Postcard Price
        api_response = api_instance.calculate_postcard_price(content_type=content_type, send_postcard_request=send_postcard_request)
        print("The response of DefaultApi->calculate_postcard_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->calculate_postcard_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_postcard_request** | [**SendPostcardRequest**](SendPostcardRequest.md)|  | [optional] 

### Return type

[**CalculatePostcardPrice**](CalculatePostcardPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **calculate_sms_campaign_price**
> CalculateSmsCampaignPrice calculate_sms_campaign_price(content_type=content_type, calculate_sms_campaign_price_request=calculate_sms_campaign_price_request)

Calculate SMS Campaign Price

_Calculate price for sms campaign_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| list_id | integer(int32) | true | none | Your list id. |
| name | string | true | none | Your campaign name. |
| body | string | true | none | Your campaign message. |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id |
| schedule | integer(int32) | false | none | Your schedule timestamp. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_sms_campaign_price import CalculateSmsCampaignPrice
from clicksend.models.calculate_sms_campaign_price_request import CalculateSmsCampaignPriceRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    calculate_sms_campaign_price_request = clicksend.CalculateSmsCampaignPriceRequest() # CalculateSmsCampaignPriceRequest |  (optional)

    try:
        # Calculate SMS Campaign Price
        api_response = api_instance.calculate_sms_campaign_price(content_type=content_type, calculate_sms_campaign_price_request=calculate_sms_campaign_price_request)
        print("The response of DefaultApi->calculate_sms_campaign_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->calculate_sms_campaign_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **calculate_sms_campaign_price_request** | [**CalculateSmsCampaignPriceRequest**](CalculateSmsCampaignPriceRequest.md)|  | [optional] 

### Return type

[**CalculateSmsCampaignPrice**](CalculateSmsCampaignPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **calculate_sms_price**
> CalculateSmsPrice calculate_sms_price(content_type=content_type, calculate_sms_price_request=calculate_sms_price_request)

Calculate SMS Price

Use this endpoint to calculate the price of sending messages. The cost of sending messages varies based on the <a href="https://help.clicksend.com/article/h474eseq3a-how-many-characters-can-i-send-in-an-sms" target="_blank">type</a> and length of the message.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_sms_price import CalculateSmsPrice
from clicksend.models.calculate_sms_price_request import CalculateSmsPriceRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    calculate_sms_price_request = {"messages":[{"source":"php","body":"Jelly liquorice marshmallow candy carrot cake 4Eyffjs1vL.","to":"+61411111111"},{"source":"php","body":"Chocolate bar icing icing oat cake carrot cake jelly cotton MWEvciEPIr.","to":"+61422222222"}]} # CalculateSmsPriceRequest |  (optional)

    try:
        # Calculate SMS Price
        api_response = api_instance.calculate_sms_price(content_type=content_type, calculate_sms_price_request=calculate_sms_price_request)
        print("The response of DefaultApi->calculate_sms_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->calculate_sms_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **calculate_sms_price_request** | [**CalculateSmsPriceRequest**](CalculateSmsPriceRequest.md)|  | [optional] 

### Return type

[**CalculateSmsPrice**](CalculateSmsPrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **calculate_voice_price**
> CalculateVoicePrice calculate_voice_price(content_type=content_type, calculate_voice_price_request=calculate_voice_price_request)

Calculate Voice Price

_Calculate voice price_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| to | string | true | none | Your phone number in [E.164](https://en.wikipedia.org/wiki/E.164) format. |
| body | string | true | none | Biscuit uv3nlCOjRk croissant chocolate lollipop chocolate muffin. |
| voice | string | true | none | Either 'female' or 'male'. |
| custom_string | string | true | none | Your reference. Will be passed back with all replies and delivery reports. |
| country | string | true | none | The country of the recipient. |
| source | string | false | none | Your method of sending e.g. 'wordpress', 'php', 'c#'. |
| list_id | integer(int32) | false | none | Your list ID if sending to a whole list. Can be used instead of 'to'. |
| lang | string | false | none | au (string, required) - See section on available languages. |
| schedule | integer(int32) | false | none | Leave blank for immediate delivery. Your schedule time in unix format [http://help.clicksend.com/what-is-a-unix-timestamp](http://help.clicksend.com/what-is-a-unix-timestamp) |
| require_input | integer(int1) | false | none | Recieve a keypress from the recipient. Flag value must be 1 for yes or 0 for no. |
| machine_detection | integer(int1) | false | none | Detect answering machine or voicemail and leave a message. Flag value must be 1 for yes or 0 for no. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_voice_price import CalculateVoicePrice
from clicksend.models.calculate_voice_price_request import CalculateVoicePriceRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    calculate_voice_price_request = clicksend.CalculateVoicePriceRequest() # CalculateVoicePriceRequest |  (optional)

    try:
        # Calculate Voice Price
        api_response = api_instance.calculate_voice_price(content_type=content_type, calculate_voice_price_request=calculate_voice_price_request)
        print("The response of DefaultApi->calculate_voice_price:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->calculate_voice_price: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **calculate_voice_price_request** | [**CalculateVoicePriceRequest**](CalculateVoicePriceRequest.md)|  | [optional] 

### Return type

[**CalculateVoicePrice**](CalculateVoicePrice.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cancel_all_sms**
> CancelAllSms cancel_all_sms(content_type=content_type, cancel_all_sms_request=cancel_all_sms_request)

Cancel All SMS

Use this endpoint to cancel all scheduled SMS. To cancel only one scheduled SMS, use the **Cancel SMS** endpoint.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.cancel_all_sms import CancelAllSms
from clicksend.models.cancel_all_sms_request import CancelAllSmsRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    cancel_all_sms_request = clicksend.CancelAllSmsRequest() # CancelAllSmsRequest |  (optional)

    try:
        # Cancel All SMS
        api_response = api_instance.cancel_all_sms(content_type=content_type, cancel_all_sms_request=cancel_all_sms_request)
        print("The response of DefaultApi->cancel_all_sms:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->cancel_all_sms: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **cancel_all_sms_request** | [**CancelAllSmsRequest**](CancelAllSmsRequest.md)|  | [optional] 

### Return type

[**CancelAllSms**](CancelAllSms.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cancel_all_voice_messages**
> CancelAllVoiceMessages cancel_all_voice_messages(content_type=content_type, body=body)

Cancel All Voice Messages

_Update all voice messages as cancelled_

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.cancel_all_voice_messages import CancelAllVoiceMessages
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/x-www-form-urlencoded' # str |  (optional)
    body = None # object |  (optional)

    try:
        # Cancel All Voice Messages
        api_response = api_instance.cancel_all_voice_messages(content_type=content_type, body=body)
        print("The response of DefaultApi->cancel_all_voice_messages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->cancel_all_voice_messages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

[**CancelAllVoiceMessages**](CancelAllVoiceMessages.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cancel_email_campaign**
> CancelEmailCampaign cancel_email_campaign(email_campaign_id, content_type=content_type, cancel_email_campaign_request=cancel_email_campaign_request)

Cancel Email Campaign

_Cancel email campaign_

Cancel email campaign

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| email_campaign_id | path | integer(int32) | true | Allowed email campaign id |
| date_from | query | integer(int32) | false | Start date (Unix Timestamp e.g. 1436849372) |
| date_to | query | integer(int32) | false | End date (Unix Timestamp e.g. 1436879372) |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.cancel_email_campaign import CancelEmailCampaign
from clicksend.models.cancel_email_campaign_request import CancelEmailCampaignRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    email_campaign_id = 'email_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    cancel_email_campaign_request = clicksend.CancelEmailCampaignRequest() # CancelEmailCampaignRequest |  (optional)

    try:
        # Cancel Email Campaign
        api_response = api_instance.cancel_email_campaign(email_campaign_id, content_type=content_type, cancel_email_campaign_request=cancel_email_campaign_request)
        print("The response of DefaultApi->cancel_email_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->cancel_email_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **cancel_email_campaign_request** | [**CancelEmailCampaignRequest**](CancelEmailCampaignRequest.md)|  | [optional] 

### Return type

[**CancelEmailCampaign**](CancelEmailCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cancel_mms_campaign**
> CancelMmsCampaign cancel_mms_campaign(mms_campaign_id, content_type=content_type, calculate_sms_campaign_price_request=calculate_sms_campaign_price_request)

Cancel MMS Campaign

_Cancel mms campaign_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| mms_campaign_id | path | integer(int32) | true | ID of MMS Campaign to cancel |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_sms_campaign_price_request import CalculateSmsCampaignPriceRequest
from clicksend.models.cancel_mms_campaign import CancelMmsCampaign
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    mms_campaign_id = 'mms_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    calculate_sms_campaign_price_request = clicksend.CalculateSmsCampaignPriceRequest() # CalculateSmsCampaignPriceRequest |  (optional)

    try:
        # Cancel MMS Campaign
        api_response = api_instance.cancel_mms_campaign(mms_campaign_id, content_type=content_type, calculate_sms_campaign_price_request=calculate_sms_campaign_price_request)
        print("The response of DefaultApi->cancel_mms_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->cancel_mms_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mms_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **calculate_sms_campaign_price_request** | [**CalculateSmsCampaignPriceRequest**](CalculateSmsCampaignPriceRequest.md)|  | [optional] 

### Return type

[**CancelMmsCampaign**](CancelMmsCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cancel_scheduled_letter**
> CancelScheduledLetter cancel_scheduled_letter(message_id)

Cancel Scheduled Letter

_Cancel scheduled letter_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| message_id | query | string | true | Message ID of the scheduled letter that is to be cancelled. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example


```python
import clicksend
from clicksend.models.cancel_scheduled_letter import CancelScheduledLetter
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)


# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    message_id = 'message_id_example' # str | 

    try:
        # Cancel Scheduled Letter
        api_response = api_instance.cancel_scheduled_letter(message_id)
        print("The response of DefaultApi->cancel_scheduled_letter:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->cancel_scheduled_letter: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_id** | **str**|  | 

### Return type

[**CancelScheduledLetter**](CancelScheduledLetter.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cancel_scheduled_postcard**
> CancelScheduledPostcard cancel_scheduled_postcard(message_id)

Cancel Scheduled Postcard

_Cancel scheduled postcard_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| message_id | query | string | true | Message ID of the scheduled postcard that is to be cancelled. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example


```python
import clicksend
from clicksend.models.cancel_scheduled_postcard import CancelScheduledPostcard
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)


# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    message_id = 'message_id_example' # str | 

    try:
        # Cancel Scheduled Postcard
        api_response = api_instance.cancel_scheduled_postcard(message_id)
        print("The response of DefaultApi->cancel_scheduled_postcard:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->cancel_scheduled_postcard: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_id** | **str**|  | 

### Return type

[**CancelScheduledPostcard**](CancelScheduledPostcard.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cancel_sms**
> CancelSms cancel_sms(message_id, content_type=content_type)

Cancel SMS

Use this endpoint to cancel a specific scheduled SMS. Unlike the **Cancel All SMS** endpoint, which cancels all scheduled SMS, this endpoint only cancels one specified scheduled SMS. 
Specify the scheduled SMS to cancel by providing its _message_id_.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.cancel_sms import CancelSms
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    message_id = 'message_id_example' # str | The _message_id_ of the scheduled SMS to cancel.
    content_type = 'application/json' # str |  (optional)

    try:
        # Cancel SMS
        api_response = api_instance.cancel_sms(message_id, content_type=content_type)
        print("The response of DefaultApi->cancel_sms:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->cancel_sms: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_id** | **str**| The _message_id_ of the scheduled SMS to cancel. | 
 **content_type** | **str**|  | [optional] 

### Return type

[**CancelSms**](CancelSms.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cancel_sms_campaign**
> CancelSmsCampaign cancel_sms_campaign(sms_campaign_id, content_type=content_type)

Cancel SMS Campaign

Use this endpoint to cancel a scheduled SMS campaign.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.cancel_sms_campaign import CancelSmsCampaign
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    sms_campaign_id = 'sms_campaign_id_example' # str | ID of the scheduled SMS campaign to cancel.
    content_type = 'application/json' # str |  (optional)

    try:
        # Cancel SMS Campaign
        api_response = api_instance.cancel_sms_campaign(sms_campaign_id, content_type=content_type)
        print("The response of DefaultApi->cancel_sms_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->cancel_sms_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sms_campaign_id** | **str**| ID of the scheduled SMS campaign to cancel. | 
 **content_type** | **str**|  | [optional] 

### Return type

[**CancelSmsCampaign**](CancelSmsCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **cancel_voice_message**
> CancelVoiceMessage cancel_voice_message(message_id, content_type=content_type, body=body)

Cancel Voice Message

_Update voice message status as cancelled_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| message_id | path | string | true | Your voice message id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.cancel_voice_message import CancelVoiceMessage
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    message_id = 'message_id_example' # str | 
    content_type = 'application/x-www-form-urlencoded' # str |  (optional)
    body = None # object |  (optional)

    try:
        # Cancel Voice Message
        api_response = api_instance.cancel_voice_message(message_id, content_type=content_type, body=body)
        print("The response of DefaultApi->cancel_voice_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->cancel_voice_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

[**CancelVoiceMessage**](CancelVoiceMessage.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **copy_contact_to_list**
> CopyContactToList copy_contact_to_list(from_list_id, contact_id, to_list_id, content_type=content_type, body=body)

Copy Contact to List

_Copy contact to another list_

Copy contact to another list

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| from_list_id | path | integer(int32) | true | List ID for list that contains contact. |
| contact_id | path | integer(int32) | true | Contact ID |
| to_list_id | path | integer(int32) | true | List ID for list you want to copy contact to. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.copy_contact_to_list import CopyContactToList
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    from_list_id = 'from_list_id_example' # str | 
    contact_id = 'contact_id_example' # str | 
    to_list_id = 'to_list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    body = None # object |  (optional)

    try:
        # Copy Contact to List
        api_response = api_instance.copy_contact_to_list(from_list_id, contact_id, to_list_id, content_type=content_type, body=body)
        print("The response of DefaultApi->copy_contact_to_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->copy_contact_to_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **from_list_id** | **str**|  | 
 **contact_id** | **str**|  | 
 **to_list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

[**CopyContactToList**](CopyContactToList.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_allowed_email_address**
> CreateAllowedEmailAddress create_allowed_email_address(content_type=content_type, create_allowed_email_address_request=create_allowed_email_address_request)

Create Allowed Email Address

_Create allowed Email Address_

Create allowed Email Address

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| body | body | string | true | Email to be allowed. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_allowed_email_address import CreateAllowedEmailAddress
from clicksend.models.create_allowed_email_address_request import CreateAllowedEmailAddressRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_allowed_email_address_request = clicksend.CreateAllowedEmailAddressRequest() # CreateAllowedEmailAddressRequest |  (optional)

    try:
        # Create Allowed Email Address
        api_response = api_instance.create_allowed_email_address(content_type=content_type, create_allowed_email_address_request=create_allowed_email_address_request)
        print("The response of DefaultApi->create_allowed_email_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_allowed_email_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_allowed_email_address_request** | [**CreateAllowedEmailAddressRequest**](CreateAllowedEmailAddressRequest.md)|  | [optional] 

### Return type

[**CreateAllowedEmailAddress**](CreateAllowedEmailAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_default_sender**
> CreateDefaultSender create_default_sender(content_type=content_type, create_default_sender_request=create_default_sender_request)

Create Default Sender

Creates a new default sender configuration to automate the selection of compliant SenderIDs.
By configuring a default sender you no longer need to define the `sender_id` string when sending SMS messages. The default sender will be picked up automatically.

For more information on Sender IDs, please refer to [What is a Sender ID or Sender Number?](https://help.clicksend.com/article/4kgj7krx00-what-is-a-sender-id-or-sender-number)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_default_sender import CreateDefaultSender
from clicksend.models.create_default_sender_request import CreateDefaultSenderRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_default_sender_request = clicksend.CreateDefaultSenderRequest() # CreateDefaultSenderRequest |  (optional)

    try:
        # Create Default Sender
        api_response = api_instance.create_default_sender(content_type=content_type, create_default_sender_request=create_default_sender_request)
        print("The response of DefaultApi->create_default_sender:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_default_sender: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_default_sender_request** | [**CreateDefaultSenderRequest**](CreateDefaultSenderRequest.md)|  | [optional] 

### Return type

[**CreateDefaultSender**](CreateDefaultSender.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |
**400** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_delivery_issue**
> CreateDeliveryIssue create_delivery_issue(content_type=content_type, create_delivery_issue_request=create_delivery_issue_request)

Create Delivery Issues

_Create delivery Issue_

Create delivery Issue

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| message_id | string | false | none | The message id of the message. |
| type | string | true | none | The type of message, must be one of the following values SMS, MMS, VOICE, EMAIL_MARKETING, EMAIL_TRANSACTIONAL, FAX, POST. |
| description | string | true | none | The description of the message. |
| client_comments | string | false | none | The user's comments. |
| email-address | string | true | none | The user's email address. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_delivery_issue import CreateDeliveryIssue
from clicksend.models.create_delivery_issue_request import CreateDeliveryIssueRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_delivery_issue_request = clicksend.CreateDeliveryIssueRequest() # CreateDeliveryIssueRequest |  (optional)

    try:
        # Create Delivery Issues
        api_response = api_instance.create_delivery_issue(content_type=content_type, create_delivery_issue_request=create_delivery_issue_request)
        print("The response of DefaultApi->create_delivery_issue:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_delivery_issue: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_delivery_issue_request** | [**CreateDeliveryIssueRequest**](CreateDeliveryIssueRequest.md)|  | [optional] 

### Return type

[**CreateDeliveryIssue**](CreateDeliveryIssue.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_email_delivery_receipt_rule**
> CreateEmailDeliveryReceiptRule create_email_delivery_receipt_rule(content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)

Create Email Delivery Receipt Rule

_Create email delivery receipt automations_

Create email delivery receipt automations

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| rule_name | string | true | none | Rule Name. |
| match_type | number | true | none | Match Type. 0=All reports. |
| action | string | true | none | Action to be taken (AUTO_REPLY, EMAIL_USER, EMAIL_FIXED, URL, SMS, POLL, GROUP_SMS, MOVE_CONTACT, CREATE_CONTACT, CREATE_CONTACT_PLUS_EMAIL, CREATE_CONTACT_PLUS_NAME_EMAIL CREATE_CONTACT_PLUS_NAME, SMPP, NONE). |
| action_address | string | true | none | Action address. |
| enabled | number | true | none | Enabled: Disabled=0 or Enabled=1. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_email_delivery_receipt_rule import CreateEmailDeliveryReceiptRule
from clicksend.models.create_sms_delivery_receipt_rule_request import CreateSmsDeliveryReceiptRuleRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_sms_delivery_receipt_rule_request = clicksend.CreateSmsDeliveryReceiptRuleRequest() # CreateSmsDeliveryReceiptRuleRequest |  (optional)

    try:
        # Create Email Delivery Receipt Rule
        api_response = api_instance.create_email_delivery_receipt_rule(content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)
        print("The response of DefaultApi->create_email_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_email_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_sms_delivery_receipt_rule_request** | [**CreateSmsDeliveryReceiptRuleRequest**](CreateSmsDeliveryReceiptRuleRequest.md)|  | [optional] 

### Return type

[**CreateEmailDeliveryReceiptRule**](CreateEmailDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_email_template**
> CreateEmailTemplate create_email_template(content_type=content_type, create_email_template_request=create_email_template_request)

Create Email Template

_Create email template_

Create email template

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| template_name | string | true | none | The intended name for the new template. |
| template_id_master | number | true | none | The ID of the master template you want to base on. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_email_template import CreateEmailTemplate
from clicksend.models.create_email_template_request import CreateEmailTemplateRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_email_template_request = clicksend.CreateEmailTemplateRequest() # CreateEmailTemplateRequest |  (optional)

    try:
        # Create Email Template
        api_response = api_instance.create_email_template(content_type=content_type, create_email_template_request=create_email_template_request)
        print("The response of DefaultApi->create_email_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_email_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_email_template_request** | [**CreateEmailTemplateRequest**](CreateEmailTemplateRequest.md)|  | [optional] 

### Return type

[**CreateEmailTemplate**](CreateEmailTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_fax_delivery_receipt_rule**
> CreateFaxDeliveryReceiptRule create_fax_delivery_receipt_rule(content_type=content_type, create_fax_delivery_receipt_rule_request=create_fax_delivery_receipt_rule_request)

Create FAX Delivery Receipt Rule

_Create fax delivery receipt automations_

Create fax delivery receipt automations

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| rule_name | string | true | none | Rule Name. |
| match_type | number | true | none | Match Type. 0=All reports. |
| action | string | true | none | Action to be taken (AUTO_REPLY, EMAIL_USER, EMAIL_FIXED, URL, SMS, POLL, GROUP_SMS, MOVE_CONTACT, CREATE_CONTACT, CREATE_CONTACT_PLUS_EMAIL, CREATE_CONTACT_PLUS_NAME_EMAIL CREATE_CONTACT_PLUS_NAME, SMPP, NONE). |
| action_address | string | true | none | Action address. |
| enabled | number | true | none | Enabled: Disabled=0 or Enabled=1. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_fax_delivery_receipt_rule import CreateFaxDeliveryReceiptRule
from clicksend.models.create_fax_delivery_receipt_rule_request import CreateFaxDeliveryReceiptRuleRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_fax_delivery_receipt_rule_request = clicksend.CreateFaxDeliveryReceiptRuleRequest() # CreateFaxDeliveryReceiptRuleRequest |  (optional)

    try:
        # Create FAX Delivery Receipt Rule
        api_response = api_instance.create_fax_delivery_receipt_rule(content_type=content_type, create_fax_delivery_receipt_rule_request=create_fax_delivery_receipt_rule_request)
        print("The response of DefaultApi->create_fax_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_fax_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_fax_delivery_receipt_rule_request** | [**CreateFaxDeliveryReceiptRuleRequest**](CreateFaxDeliveryReceiptRuleRequest.md)|  | [optional] 

### Return type

[**CreateFaxDeliveryReceiptRule**](CreateFaxDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_fax_inbound_rule**
> CreateFaxInboundRule create_fax_inbound_rule(content_type=content_type, create_fax_inbound_rule_request=create_fax_inbound_rule_request)

Create Fax Inbound Rule

_Create new inbound fax automation_

Create new inbound fax automation

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| dedicated_number | string | true | none | Dedicated Number. Can be '\*' to apply to all numbers. |
| rule_name | string | true | none | Rule Name. |
| action | string | true | none | Action to be taken (AUTO_REPLY, EMAIL_USER, EMAIL_FIXED, URL, SMS, POLL, GROUP_SMS, MOVE_CONTACT, CREATE_CONTACT, CREATE_CONTACT_PLUS_EMAIL, CREATE_CONTACT_PLUS_NAME_EMAIL CREATE_CONTACT_PLUS_NAME, SMPP, NONE). |
| action_address | string | true | none | Action address. |
| enabled | number | true | none | Enabled: Disabled=0 or Enabled=1. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_fax_inbound_rule import CreateFaxInboundRule
from clicksend.models.create_fax_inbound_rule_request import CreateFaxInboundRuleRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_fax_inbound_rule_request = clicksend.CreateFaxInboundRuleRequest() # CreateFaxInboundRuleRequest |  (optional)

    try:
        # Create Fax Inbound Rule
        api_response = api_instance.create_fax_inbound_rule(content_type=content_type, create_fax_inbound_rule_request=create_fax_inbound_rule_request)
        print("The response of DefaultApi->create_fax_inbound_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_fax_inbound_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_fax_inbound_rule_request** | [**CreateFaxInboundRuleRequest**](CreateFaxInboundRuleRequest.md)|  | [optional] 

### Return type

[**CreateFaxInboundRule**](CreateFaxInboundRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_list**
> CreateList create_list(content_type=content_type, create_list_request=create_list_request)

Create List

_Create new contact list_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_name | body | string | true | Your contact list name |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_list import CreateList
from clicksend.models.create_list_request import CreateListRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_list_request = clicksend.CreateListRequest() # CreateListRequest |  (optional)

    try:
        # Create List
        api_response = api_instance.create_list(content_type=content_type, create_list_request=create_list_request)
        print("The response of DefaultApi->create_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_list_request** | [**CreateListRequest**](CreateListRequest.md)|  | [optional] 

### Return type

[**CreateList**](CreateList.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_new_contact**
> CreateNewContact create_new_contact(list_id, content_type=content_type, create_new_contact_request=create_new_contact_request)

Create New Contact

_Create new contact_

### parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | List id |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| phone_number | string | true | none | Your phone number in\_[E.164](https://en.wikipedia.org/wiki/E.164)\_format. Must be provided if no fax number or email. |
| email | string | false | none | Your email. Must be provided if no phone number or fax number. |
| fax_number | string | false | none | Your fax number. Must be provided if no phone number or email. |
| first_name | string | false | none | Your first name. |
| address_line_1 | string | false | none | Your street address |
| address_line_2 | string | false | none | none |
| address_city | string | false | none | Your nearest city |
| address_state | string | false | none | Your current state |
| address_postal_code | string | false | none | Your current postcode |
| address_country | string | false | none | Your current country |
| organization_name | string | false | none | Your organisation name |
| custom_1 | string | true | none | none |
| custom_2 | string | false | none | none |
| custom_3 | string | false | none | none |
| custom_4 | string | false | none | none |
| last_name | string | false | none | Your last name |


Refer to [Status
Codes](/#status-codes) for
definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_new_contact import CreateNewContact
from clicksend.models.create_new_contact_request import CreateNewContactRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    list_id = 'list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    create_new_contact_request = clicksend.CreateNewContactRequest() # CreateNewContactRequest |  (optional)

    try:
        # Create New Contact
        api_response = api_instance.create_new_contact(list_id, content_type=content_type, create_new_contact_request=create_new_contact_request)
        print("The response of DefaultApi->create_new_contact:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_new_contact: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **create_new_contact_request** | [**CreateNewContactRequest**](CreateNewContactRequest.md)|  | [optional] 

### Return type

[**CreateNewContact**](CreateNewContact.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_reseller_account**
> CreateResellerAccount create_reseller_account(content_type=content_type, create_reseller_account_request=create_reseller_account_request)

Create Reseller Account

_Create reseller account_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| username | string | true | none | Account username |
| password | string | true | none | Account password (unhashed) |
| user_email | string | true | none | Account email |
| user_phone | string | true | none | Account phone number |
| user_first_name | string | true | none | Account owner first name |
| user_last_name | string | true | none | Account owner last name |
| account_name | string | true | none | Account name (usually company name) |
| country | string | true | none | Country of account holder |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_reseller_account import CreateResellerAccount
from clicksend.models.create_reseller_account_request import CreateResellerAccountRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_reseller_account_request = clicksend.CreateResellerAccountRequest() # CreateResellerAccountRequest |  (optional)

    try:
        # Create Reseller Account
        api_response = api_instance.create_reseller_account(content_type=content_type, create_reseller_account_request=create_reseller_account_request)
        print("The response of DefaultApi->create_reseller_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_reseller_account: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_reseller_account_request** | [**CreateResellerAccountRequest**](CreateResellerAccountRequest.md)|  | [optional] 

### Return type

[**CreateResellerAccount**](CreateResellerAccount.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_return_address**
> CreateReturnAddress create_return_address(content_type=content_type, create_return_address_request=create_return_address_request)

Create Return Address

_Create post return address_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| address_name | string | true | none | Your address name. |
| address_line_1 | string | true | none | Your address line 1 |
| address_city | string | true | none | Your city |
| address_postal_code | string | true | none | Your postal code |
| address_country | string | true | none | Your country |
| address_line_2 | string | false | none | Your address line 2 |
| address_state | string | false | none | Your state |


 Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


 <div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_return_address import CreateReturnAddress
from clicksend.models.create_return_address_request import CreateReturnAddressRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_return_address_request = clicksend.CreateReturnAddressRequest() # CreateReturnAddressRequest |  (optional)

    try:
        # Create Return Address
        api_response = api_instance.create_return_address(content_type=content_type, create_return_address_request=create_return_address_request)
        print("The response of DefaultApi->create_return_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_return_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_return_address_request** | [**CreateReturnAddressRequest**](CreateReturnAddressRequest.md)|  | [optional] 

### Return type

[**CreateReturnAddress**](CreateReturnAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_sms_delivery_receipt_rule**
> CreateSmsDeliveryReceiptRule create_sms_delivery_receipt_rule(content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)

Create SMS Delivery Receipt Rule

_Create sms delivery receipt automations_

Create sms delivery receipt automations

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| rule_name | string | true | none | Rule Name. |
| match_type | number | true | none | Match Type. 0=All reports. |
| action | string | true | none | Action to be taken (AUTO_REPLY, EMAIL_USER, EMAIL_FIXED, URL, SMS, POLL, GROUP_SMS, MOVE_CONTACT, CREATE_CONTACT, CREATE_CONTACT_PLUS_EMAIL, CREATE_CONTACT_PLUS_NAME_EMAIL CREATE_CONTACT_PLUS_NAME, SMPP, NONE). |
| action_address | string | true | none | Action address. |
| enabled | number | true | none | Enabled: Disabled=0 or Enabled=1. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_sms_delivery_receipt_rule import CreateSmsDeliveryReceiptRule
from clicksend.models.create_sms_delivery_receipt_rule_request import CreateSmsDeliveryReceiptRuleRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_sms_delivery_receipt_rule_request = clicksend.CreateSmsDeliveryReceiptRuleRequest() # CreateSmsDeliveryReceiptRuleRequest |  (optional)

    try:
        # Create SMS Delivery Receipt Rule
        api_response = api_instance.create_sms_delivery_receipt_rule(content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)
        print("The response of DefaultApi->create_sms_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_sms_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_sms_delivery_receipt_rule_request** | [**CreateSmsDeliveryReceiptRuleRequest**](CreateSmsDeliveryReceiptRuleRequest.md)|  | [optional] 

### Return type

[**CreateSmsDeliveryReceiptRule**](CreateSmsDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_sms_inbound_automation**
> CreateSmsInboundAutomation create_sms_inbound_automation(content_type=content_type, create_sms_inbound_automation_request=create_sms_inbound_automation_request)

Create SMS Inbound Automation

_Create new inbound sms automation_

Create new inbound sms automation

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| dedicated_number | string | true | none | Decicated Number. Can be '\*' to apply to all numbers. |
| rule_name | string | true | none | Rule Name. |
| message_search_type | number | true | none | Message Search Type: 0=Any message, 1=starts with, 2=contains, 3=does not contain. |
| message_search_term | string | true | none | Message search term. |
| action | string | true | none | Action to be taken (AUTO_REPLY, EMAIL_USER, EMAIL_FIXED, URL, SMS, POLL, GROUP_SMS, MOVE_CONTACT, CREATE_CONTACT, CREATE_CONTACT_PLUS_EMAIL, CREATE_CONTACT_PLUS_NAME_EMAIL CREATE_CONTACT_PLUS_NAME, SMPP, NONE). |
| action_address | string | true | none | Action address. |
| enabled | number | true | none | Enabled: Disabled=0 or Enabled=1. |
| webhook_type | string | false | Required when action = URL only | Set as post, get, or json to change the format of the request sent. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_sms_inbound_automation import CreateSmsInboundAutomation
from clicksend.models.create_sms_inbound_automation_request import CreateSmsInboundAutomationRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_sms_inbound_automation_request = clicksend.CreateSmsInboundAutomationRequest() # CreateSmsInboundAutomationRequest |  (optional)

    try:
        # Create SMS Inbound Automation
        api_response = api_instance.create_sms_inbound_automation(content_type=content_type, create_sms_inbound_automation_request=create_sms_inbound_automation_request)
        print("The response of DefaultApi->create_sms_inbound_automation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_sms_inbound_automation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_sms_inbound_automation_request** | [**CreateSmsInboundAutomationRequest**](CreateSmsInboundAutomationRequest.md)|  | [optional] 

### Return type

[**CreateSmsInboundAutomation**](CreateSmsInboundAutomation.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_sms_template**
> CreateSmsTemplate create_sms_template(content_type=content_type, create_sms_template_request=create_sms_template_request)

Create SMS Template

Use this endpoint to create a SMS template that you can use for sending SMS.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_sms_template import CreateSmsTemplate
from clicksend.models.create_sms_template_request import CreateSmsTemplateRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_sms_template_request = clicksend.CreateSmsTemplateRequest() # CreateSmsTemplateRequest |  (optional)

    try:
        # Create SMS Template
        api_response = api_instance.create_sms_template(content_type=content_type, create_sms_template_request=create_sms_template_request)
        print("The response of DefaultApi->create_sms_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_sms_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_sms_template_request** | [**CreateSmsTemplateRequest**](CreateSmsTemplateRequest.md)|  | [optional] 

### Return type

[**CreateSmsTemplate**](CreateSmsTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_stripped_string_rule**
> CreateStrippedStringRule create_stripped_string_rule(content_type=content_type, create_stripped_string_rule_request=create_stripped_string_rule_request)

Create Stripped String Rule

_Create email to sms stripped string rule_

Create email to sms stripped string rules

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| stripped-string | body | string | true | String to be stripped. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_stripped_string_rule import CreateStrippedStringRule
from clicksend.models.create_stripped_string_rule_request import CreateStrippedStringRuleRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_stripped_string_rule_request = clicksend.CreateStrippedStringRuleRequest() # CreateStrippedStringRuleRequest |  (optional)

    try:
        # Create Stripped String Rule
        api_response = api_instance.create_stripped_string_rule(content_type=content_type, create_stripped_string_rule_request=create_stripped_string_rule_request)
        print("The response of DefaultApi->create_stripped_string_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_stripped_string_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_stripped_string_rule_request** | [**CreateStrippedStringRuleRequest**](CreateStrippedStringRuleRequest.md)|  | [optional] 

### Return type

[**CreateStrippedStringRule**](CreateStrippedStringRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_subaccount**
> CreateSubaccount create_subaccount(content_type=content_type, create_subaccount_request=create_subaccount_request)

Create Subaccount

_Create new subaccount_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| api_username | string | true | none | Your new api username. |
| password | string | true | none | Your new password |
| email | string | true | none | Your new email. |
| phone_number | string | true | none | Your phone number in [E.164](https://en.wikipedia.org/wiki/E.164) format. |
| first_name | string | true | none | Your firstname |
| last_name | string | true | none | Your lastname |
| access_users | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |
| access_billing | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |
| access_reporting | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |
| access_contacts | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |
| access_settings | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_subaccount import CreateSubaccount
from clicksend.models.create_subaccount_request import CreateSubaccountRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_subaccount_request = clicksend.CreateSubaccountRequest() # CreateSubaccountRequest |  (optional)

    try:
        # Create Subaccount
        api_response = api_instance.create_subaccount(content_type=content_type, create_subaccount_request=create_subaccount_request)
        print("The response of DefaultApi->create_subaccount:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_subaccount: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_subaccount_request** | [**CreateSubaccountRequest**](CreateSubaccountRequest.md)|  | [optional] 

### Return type

[**CreateSubaccount**](CreateSubaccount.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_test_inbound_sms**
> CreateTestInboundSms create_test_inbound_sms(content_type=content_type, create_test_inbound_sms_request=create_test_inbound_sms_request)

Create Test Inbound SMS

Use this endpoint to generate and send a test <a href="https://help.clicksend.com/article/ik4hw5xu35-can-i-receive-inbound-sms-to-my-url" target="_blank">inbound SMS</a> to your webhook URL. Inbound SMS are messages sent by your recipient to you. 
This test endpoint allows you to verify that the inbound SMS is correctly sent to your webhook URL.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_test_inbound_sms import CreateTestInboundSms
from clicksend.models.create_test_inbound_sms_request import CreateTestInboundSmsRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_test_inbound_sms_request = clicksend.CreateTestInboundSmsRequest() # CreateTestInboundSmsRequest |  (optional)

    try:
        # Create Test Inbound SMS
        api_response = api_instance.create_test_inbound_sms(content_type=content_type, create_test_inbound_sms_request=create_test_inbound_sms_request)
        print("The response of DefaultApi->create_test_inbound_sms:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_test_inbound_sms: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_test_inbound_sms_request** | [**CreateTestInboundSmsRequest**](CreateTestInboundSmsRequest.md)|  | [optional] 

### Return type

[**CreateTestInboundSms**](CreateTestInboundSms.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_test_sms_receipt**
> CreateTestSmsReceipt create_test_sms_receipt(content_type=content_type, create_test_sms_receipt_request=create_test_sms_receipt_request)

Create Test SMS Receipt

Use this endpoint to generate and send a test <a href="https://help.clicksend.com/article/49eq1qdcui-how-do-i-receive-sms-delivery-receipts-delivery-status-updates" target="_blank">SMS delivery receipt</a> to your webhook URL. When you send an SMS, a delivery receipt is generated and can be received at your webhook URL. This test endpoint allows you to verify that the receipt is correctly sent to your webhook URL.

Additionally, you can obtain SMS receipts by setting the webhook URL to **poll** and periodically calling the **View SMS Receipt** endpoint to check for new receipts. This process is known as _polling_.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_test_sms_receipt import CreateTestSmsReceipt
from clicksend.models.create_test_sms_receipt_request import CreateTestSmsReceiptRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_test_sms_receipt_request = clicksend.CreateTestSmsReceiptRequest() # CreateTestSmsReceiptRequest |  (optional)

    try:
        # Create Test SMS Receipt
        api_response = api_instance.create_test_sms_receipt(content_type=content_type, create_test_sms_receipt_request=create_test_sms_receipt_request)
        print("The response of DefaultApi->create_test_sms_receipt:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_test_sms_receipt: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_test_sms_receipt_request** | [**CreateTestSmsReceiptRequest**](CreateTestSmsReceiptRequest.md)|  | [optional] 

### Return type

[**CreateTestSmsReceipt**](CreateTestSmsReceipt.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_voice_delivery_receipt_rule**
> CreateVoiceDeliveryReceiptRule create_voice_delivery_receipt_rule(content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)

Create Voice Delivery Receipt Rule

_Create voice delivery receipt automations_

Create voice delivery receipt automations

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| rule_name | string | true | none | Rule Name. |
| match_type | number | true | none | Match Type. 0=All reports. |
| action | string | true | none | Action to be taken (AUTO_REPLY, EMAIL_USER, EMAIL_FIXED, URL, SMS, POLL, GROUP_SMS, MOVE_CONTACT, CREATE_CONTACT, CREATE_CONTACT_PLUS_EMAIL, CREATE_CONTACT_PLUS_NAME_EMAIL CREATE_CONTACT_PLUS_NAME, SMPP, NONE). |
| action_address | string | true | none | Action address. |
| enabled | number | true | none | Enabled: Disabled=0 or Enabled=1. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_sms_delivery_receipt_rule_request import CreateSmsDeliveryReceiptRuleRequest
from clicksend.models.create_voice_delivery_receipt_rule import CreateVoiceDeliveryReceiptRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    create_sms_delivery_receipt_rule_request = clicksend.CreateSmsDeliveryReceiptRuleRequest() # CreateSmsDeliveryReceiptRuleRequest |  (optional)

    try:
        # Create Voice Delivery Receipt Rule
        api_response = api_instance.create_voice_delivery_receipt_rule(content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)
        print("The response of DefaultApi->create_voice_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->create_voice_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **create_sms_delivery_receipt_rule_request** | [**CreateSmsDeliveryReceiptRuleRequest**](CreateSmsDeliveryReceiptRuleRequest.md)|  | [optional] 

### Return type

[**CreateVoiceDeliveryReceiptRule**](CreateVoiceDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **current_payment_info**
> CurrentPaymentInfo current_payment_info(content_type=content_type)

Current Payment Info

_Get current payment info_

This endpoint returns your current payment info, we do not store credit card numbers, only a card token for security reasons.

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.current_payment_info import CurrentPaymentInfo
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # Current Payment Info
        api_response = api_instance.current_payment_info(content_type=content_type)
        print("The response of DefaultApi->current_payment_info:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->current_payment_info: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**CurrentPaymentInfo**](CurrentPaymentInfo.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_allowed_email_address**
> DeleteAllowedEmailAddress delete_allowed_email_address(email_address_id, content_type=content_type)

Delete Allowed Email Address

_Delete specific email address_

Delete specific email address

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| email_address_id | path | integer(int32) | true | Allowed email address id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_allowed_email_address import DeleteAllowedEmailAddress
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    email_address_id = 'email_address_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Allowed Email Address
        api_response = api_instance.delete_allowed_email_address(email_address_id, content_type=content_type)
        print("The response of DefaultApi->delete_allowed_email_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_allowed_email_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_address_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteAllowedEmailAddress**](DeleteAllowedEmailAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_alpha_tag**
> delete_alpha_tag(alpha_tag_id, content_type=content_type)

Delete Alpha Tag

_Delete a specific alpha tag._

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| alpha_tag_id | path | uuid | true | ID of the alpha tag |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    alpha_tag_id = 'alpha_tag_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Alpha Tag
        api_instance.delete_alpha_tag(alpha_tag_id, content_type=content_type)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_alpha_tag: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **alpha_tag_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_contact**
> DeleteContact delete_contact(list_id, contact_id, content_type=content_type)

Delete Contact

_Delete a contact_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | List ID |
| contact_id | path | integer(int32) | true | Contact ID |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_contact import DeleteContact
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    list_id = 'list_id_example' # str | 
    contact_id = 'contact_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Contact
        api_response = api_instance.delete_contact(list_id, contact_id, content_type=content_type)
        print("The response of DefaultApi->delete_contact:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_contact: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **contact_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteContact**](DeleteContact.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_default_sender**
> delete_default_sender(default_sender_id, content_type=content_type)

Delete Default Sender

Removes a specified default sender setting. 
If you don't configure a default sender and leave the `sender_id` string blank when sending an SMS,
Smart Assign will pick the best suitable, compliant, available SenderID for you.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    default_sender_id = 'default_sender_id_example' # str | The ID of the default sender to delete
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Default Sender
        api_instance.delete_default_sender(default_sender_id, content_type=content_type)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_default_sender: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **default_sender_id** | **str**| The ID of the default sender to delete | 
 **content_type** | **str**|  | [optional] 

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Successful response (No Content) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_email_delivery_receipt_rule**
> DeleteEmailDeliveryReceiptRule delete_email_delivery_receipt_rule(receipt_rule_id, content_type=content_type)

Delete Email Delivery Receipt Rule

_Delete email delivery receipt automation_

Delete email delivery receipt automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| receipt_rule_id | path | integer(int32) | true | Receipt rule id |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_email_delivery_receipt_rule import DeleteEmailDeliveryReceiptRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Email Delivery Receipt Rule
        api_response = api_instance.delete_email_delivery_receipt_rule(receipt_rule_id, content_type=content_type)
        print("The response of DefaultApi->delete_email_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_email_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteEmailDeliveryReceiptRule**](DeleteEmailDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_email_template**
> DeleteEmailTemplate delete_email_template(template_id, content_type=content_type)

Delete Email Template

_Delete user email template_

Delete user email template

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| template_id | path | integer(int32) | true | Email template id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_email_template import DeleteEmailTemplate
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    template_id = 'template_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Email Template
        api_response = api_instance.delete_email_template(template_id, content_type=content_type)
        print("The response of DefaultApi->delete_email_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_email_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteEmailTemplate**](DeleteEmailTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_fax_delivery_receipt_rule**
> DeleteFaxDeliveryReceiptRule delete_fax_delivery_receipt_rule(receipt_rule_id, content_type=content_type)

Delete FAX Delivery Receipt Rule

_Delete fax delivery receipt automation_

Delete fax delivery receipt automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| receipt_rule_id | path | integer(int32) | true | Receipt rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_fax_delivery_receipt_rule import DeleteFaxDeliveryReceiptRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete FAX Delivery Receipt Rule
        api_response = api_instance.delete_fax_delivery_receipt_rule(receipt_rule_id, content_type=content_type)
        print("The response of DefaultApi->delete_fax_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_fax_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteFaxDeliveryReceiptRule**](DeleteFaxDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_fax_inbound_rule**
> DeleteFaxInboundRule delete_fax_inbound_rule(inbound_rule_id, content_type=content_type)

Delete Fax Inbound Rule

_Delete inbound fax automation_

Delete inbound fax automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| inbound_rule_id | path | integer(int32) | true | Inbound rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_fax_inbound_rule import DeleteFaxInboundRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    inbound_rule_id = 'inbound_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Fax Inbound Rule
        api_response = api_instance.delete_fax_inbound_rule(inbound_rule_id, content_type=content_type)
        print("The response of DefaultApi->delete_fax_inbound_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_fax_inbound_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inbound_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteFaxInboundRule**](DeleteFaxInboundRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_list**
> DeleteList delete_list(list_id, content_type=content_type)

Delete List

_ListsByListIdDelete_

Delete a specific contact list

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | List ID |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_list import DeleteList
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    list_id = 'list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete List
        api_response = api_instance.delete_list(list_id, content_type=content_type)
        print("The response of DefaultApi->delete_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteList**](DeleteList.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_own_number**
> OwnNumber delete_own_number(own_number_id, content_type=content_type)

Delete Own Number

_Delete a specific own numbers._

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| own_number_id | path | uuid | true | ID of the own number |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.own_number import OwnNumber
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    own_number_id = 'own_number_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Own Number
        api_response = api_instance.delete_own_number(own_number_id, content_type=content_type)
        print("The response of DefaultApi->delete_own_number:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_own_number: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **own_number_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**OwnNumber**](OwnNumber.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_return_address**
> DeleteReturnAddress delete_return_address(return_address_id, content_type=content_type)

Delete Return Address

_Delete specific post return address_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| return_address_id | path | integer(int32) | true | Return address ID |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_return_address import DeleteReturnAddress
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    return_address_id = 'return_address_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Return Address
        api_response = api_instance.delete_return_address(return_address_id, content_type=content_type)
        print("The response of DefaultApi->delete_return_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_return_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **return_address_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteReturnAddress**](DeleteReturnAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_sms_delivery_receipt_rule**
> DeleteSmsDeliveryReceiptRule delete_sms_delivery_receipt_rule(receipt_rule_id, content_type=content_type)

Delete SMS Delivery Receipt Rule

_Delete sms delivery receipt automation_

Delete sms delivery receipt automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| receipt_rule_id | path | integer(int32) | true | Receipt rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_sms_delivery_receipt_rule import DeleteSmsDeliveryReceiptRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete SMS Delivery Receipt Rule
        api_response = api_instance.delete_sms_delivery_receipt_rule(receipt_rule_id, content_type=content_type)
        print("The response of DefaultApi->delete_sms_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_sms_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteSmsDeliveryReceiptRule**](DeleteSmsDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_sms_inbound_automation**
> DeleteSmsInboundAutomation delete_sms_inbound_automation(inbound_rule_id, content_type=content_type)

Delete SMS Inbound Automation

_Delete inbound sms automation_

Delete inbound sms automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| inbound_rule_id | path | integer(int32) | true | Inbound rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_sms_inbound_automation import DeleteSmsInboundAutomation
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    inbound_rule_id = 'inbound_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete SMS Inbound Automation
        api_response = api_instance.delete_sms_inbound_automation(inbound_rule_id, content_type=content_type)
        print("The response of DefaultApi->delete_sms_inbound_automation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_sms_inbound_automation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inbound_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteSmsInboundAutomation**](DeleteSmsInboundAutomation.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_sms_template**
> DeleteSmsTemplate delete_sms_template(template_id, content_type=content_type)

Delete SMS Template

Use this endpoint to delete a <a href="https://help.clicksend.com/article/9z9uloaz8y-sms-templates-for-different-industries" target="_blank">SMS template</a>. Specify the SMS template to delete by providing its _template_id_.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_sms_template import DeleteSmsTemplate
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    template_id = 'template_id_example' # str | The ID of the template to delete.
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete SMS Template
        api_response = api_instance.delete_sms_template(template_id, content_type=content_type)
        print("The response of DefaultApi->delete_sms_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_sms_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**| The ID of the template to delete. | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteSmsTemplate**](DeleteSmsTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_stripped_string_rule**
> DeleteStrippedStringRule delete_stripped_string_rule(rule_id, content_type=content_type)

Delete Stripped String Rule

_Delete email to sms stripped string rule_

Delete email to sms stripped string rule

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| rule_id | path | integer(int32) | true | Your rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_stripped_string_rule import DeleteStrippedStringRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    rule_id = 'rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Stripped String Rule
        api_response = api_instance.delete_stripped_string_rule(rule_id, content_type=content_type)
        print("The response of DefaultApi->delete_stripped_string_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_stripped_string_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteStrippedStringRule**](DeleteStrippedStringRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_subaccount**
> DeleteSubaccount delete_subaccount(subaccount_id, content_type=content_type)

Delete Subaccount

_Delete a subaccount_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| subaccount_id | path | integer(int32) | true | ID of subaccount to delete |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_subaccount import DeleteSubaccount
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    subaccount_id = 'subaccount_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Subaccount
        api_response = api_instance.delete_subaccount(subaccount_id, content_type=content_type)
        print("The response of DefaultApi->delete_subaccount:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_subaccount: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subaccount_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteSubaccount**](DeleteSubaccount.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_voice_delivery_receipt_rule**
> DeleteVoiceDeliveryReceiptRule delete_voice_delivery_receipt_rule(receipt_rule_id, content_type=content_type)

Delete Voice Delivery Receipt Rule

_Delete voice delivery receipt automation_

Delete voice delivery receipt automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| receipt_rule_id | path | integer(int32) | true | Receipt rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.delete_voice_delivery_receipt_rule import DeleteVoiceDeliveryReceiptRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Delete Voice Delivery Receipt Rule
        api_response = api_instance.delete_voice_delivery_receipt_rule(receipt_rule_id, content_type=content_type)
        print("The response of DefaultApi->delete_voice_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->delete_voice_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**DeleteVoiceDeliveryReceiptRule**](DeleteVoiceDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **detect_address**
> DetectAddress detect_address(content_type=content_type, body=body)

Detect Address

_Detects address in uploaded file._

The `detect-address` endpoint accepts either a letter in PDF format or an address string and attempts to convert it to a standard address format. Note that the PDF should be in standard address format, having the recipient's name and address listed at the top.

The endpoint accepts two types of data: 1. A PDF file in `base64` encoding. In this case, submit the `base64`\-encoded PDF file contents in the `content` field of the request body. 2. An address string. In this case, submit the address in a string using the `address` field of the request body.

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| convert | query | string | true | none |
| content | body | string | true | Base64-encoded file contents |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.detect_address import DetectAddress
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    body = None # object |  (optional)

    try:
        # Detect Address
        api_response = api_instance.detect_address(content_type=content_type, body=body)
        print("The response of DefaultApi->detect_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->detect_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

[**DetectAddress**](DetectAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **export_email_campaign_history**
> export_email_campaign_history(email_campaign_id, content_type=content_type)

Export Email Campaign History

_Export specific email campaign history_

Export specific email campaign history

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| email_campaign_id | path | integer(int32) | true | Allowed email campaign id |
| date_from | query | integer(int32) | false | Start date (Unix Timestamp e.g. 1436849372) |
| date_to | query | integer(int32) | false | End date (Unix Timestamp e.g. 1436879372) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    email_campaign_id = 'email_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Export Email Campaign History
        api_instance.export_email_campaign_history(email_campaign_id, content_type=content_type)
    except Exception as e:
        print("Exception when calling DefaultApi->export_email_campaign_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **export_email_history**
> ExportEmailHistory export_email_history(content_type=content_type)

Export Email History

_Export all Transactional Email history_

Export all Transactional Email history

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| filename | query | string | true | Filename to download history as |
| date_from | query | integer(int32) | false | Start date (Unix Timestamp e.g. 1436849372) |
| date_to | query | integer(int32) | false | End date (Unix Timestamp e.g. 1436879372) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.export_email_history import ExportEmailHistory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # Export Email History
        api_response = api_instance.export_email_history(content_type=content_type)
        print("The response of DefaultApi->export_email_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->export_email_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ExportEmailHistory**](ExportEmailHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **export_letter_history**
> ExportLetterHistory export_letter_history(content_type=content_type, filename=filename, q=q, order_by=order_by, date_from=date_from, date_to=date_to, limit=limit)

Export Letter History

_export letter history_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| filename | query | string | true | Filename to export to |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.export_letter_history import ExportLetterHistory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    filename = 'Post_history.csv' # str |  (optional)
    q = 'q_example' # str |  (optional)
    order_by = 'date_added:desc' # str |  (optional)
    date_from = 'date_from_example' # str |  (optional)
    date_to = 'date_to_example' # str |  (optional)
    limit = 50000 # int |  (optional)

    try:
        # Export Letter History
        api_response = api_instance.export_letter_history(content_type=content_type, filename=filename, q=q, order_by=order_by, date_from=date_from, date_to=date_to, limit=limit)
        print("The response of DefaultApi->export_letter_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->export_letter_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **filename** | **str**|  | [optional] 
 **q** | **str**|  | [optional] 
 **order_by** | **str**|  | [optional] 
 **date_from** | **str**|  | [optional] 
 **date_to** | **str**|  | [optional] 
 **limit** | **int**|  | [optional] 

### Return type

[**ExportLetterHistory**](ExportLetterHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **export_mms_history**
> ExportMmsHistory export_mms_history(content_type=content_type, filename=filename, q=q, order_by=order_by, date_from=date_from, date_to=date_to, limit=limit)

Export MMS History

_Export all mms history_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| filename | query | string | true | Filename to download history as |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.export_mms_history import ExportMmsHistory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    filename = 'MMS_history.csv' # str |  (optional)
    q = 'q_example' # str |  (optional)
    order_by = 'date_added:desc' # str |  (optional)
    date_from = 'date_from_example' # str |  (optional)
    date_to = 'date_to_example' # str |  (optional)
    limit = 50000 # int |  (optional)

    try:
        # Export MMS History
        api_response = api_instance.export_mms_history(content_type=content_type, filename=filename, q=q, order_by=order_by, date_from=date_from, date_to=date_to, limit=limit)
        print("The response of DefaultApi->export_mms_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->export_mms_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **filename** | **str**|  | [optional] 
 **q** | **str**|  | [optional] 
 **order_by** | **str**|  | [optional] 
 **date_from** | **str**|  | [optional] 
 **date_to** | **str**|  | [optional] 
 **limit** | **int**|  | [optional] 

### Return type

[**ExportMmsHistory**](ExportMmsHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **export_postcard_history**
> ExportPostcardHistory export_postcard_history(content_type=content_type)

Export Postcard History

_Export postcard history to a CSV file_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| filename | query | string | true | Filename to export to |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.export_postcard_history import ExportPostcardHistory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # Export Postcard History
        api_response = api_instance.export_postcard_history(content_type=content_type)
        print("The response of DefaultApi->export_postcard_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->export_postcard_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ExportPostcardHistory**](ExportPostcardHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **export_sms_history**
> ExportSmsHistory export_sms_history(content_type=content_type, filename=filename, page=page, limit=limit, q=q, order_by=order_by, date_from=date_from, date_to=date_to)

Export SMS History

Use this endpoint to create a download link of your SMS history. You can filter the SMS history result using the query parameters.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.export_sms_history import ExportSmsHistory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    filename = 'export.csv' # str | The filename of the result. It should be in the .csv format. (optional) (default to 'export.csv')
    page = 1 # int | The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. (optional) (default to 1)
    limit = 15 # int | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. (optional) (default to 15)
    q = 'field_name' # str | Allows filtering of results based on your search criteria. The query should be in the format `field_name:value`.  1. **Field Name**: The field within the SMS history you want to filter by. You can use the following fields:          - _Status_: The status of the SMS. Available values for status are: Queued, Completed, Scheduled, WaitApproval, Failed, Cancelled, CancelledAfterReview, Received, Sent.              - _To_: The recipient of the SMS.              - _from_: The sender of the SMS.              - _subaccount_id_: The sub-account identifier.              - _message_id_: The ID of your SMS.          2. **Value**: The text or keyword you're searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.             For example, if you are searching for a SMS with the status of _Scheduled_, the final query would look like this:    `q=status:Scheduled`  <div class=\"info-box\">   <h4><i class=\"fas fa-info-circle\"></i> Note:</h4>   <div>   <p>Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:<br/></p>     <ul>       <li>q=from:%2B61437085284</li>     </ul>     <p>You can use the <a href=\"https://www.urlencoder.org/\" target=\"_blank\">URL encoder</a> to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.</p>   </div> </div> (optional) (default to 'field_name')
    order_by = 'date:asc' # str | Specifies the field and order to sort the results by. The value is composed of the field name followed by a colon and the sort direction (asc for ascending or desc for descending).  The default sort order is by date in ascending order. You can use the following fields:    - _date_    - _username_   - _from_    - _to_   - _status_    - _body_  For example, if you want to order by the most recently sent SMS, you should sort by date in descending order. The query would look like this:    `order_by=date:desc` (optional) (default to 'date:asc')
    date_from = 56 # int | Start date to filter results. It should be in <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>. (optional)
    date_to = 56 # int | End date to filter results. It should be in <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>. (optional)

    try:
        # Export SMS History
        api_response = api_instance.export_sms_history(content_type=content_type, filename=filename, page=page, limit=limit, q=q, order_by=order_by, date_from=date_from, date_to=date_to)
        print("The response of DefaultApi->export_sms_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->export_sms_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **filename** | **str**| The filename of the result. It should be in the .csv format. | [optional] [default to &#39;export.csv&#39;]
 **page** | **int**| The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. | [optional] [default to 1]
 **limit** | **int**| The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. | [optional] [default to 15]
 **q** | **str**| Allows filtering of results based on your search criteria. The query should be in the format &#x60;field_name:value&#x60;.  1. **Field Name**: The field within the SMS history you want to filter by. You can use the following fields:          - _Status_: The status of the SMS. Available values for status are: Queued, Completed, Scheduled, WaitApproval, Failed, Cancelled, CancelledAfterReview, Received, Sent.              - _To_: The recipient of the SMS.              - _from_: The sender of the SMS.              - _subaccount_id_: The sub-account identifier.              - _message_id_: The ID of your SMS.          2. **Value**: The text or keyword you&#39;re searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.             For example, if you are searching for a SMS with the status of _Scheduled_, the final query would look like this:    &#x60;q&#x3D;status:Scheduled&#x60;  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;div&gt;   &lt;p&gt;Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:&lt;br/&gt;&lt;/p&gt;     &lt;ul&gt;       &lt;li&gt;q&#x3D;from:%2B61437085284&lt;/li&gt;     &lt;/ul&gt;     &lt;p&gt;You can use the &lt;a href&#x3D;\&quot;https://www.urlencoder.org/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;URL encoder&lt;/a&gt; to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.&lt;/p&gt;   &lt;/div&gt; &lt;/div&gt; | [optional] [default to &#39;field_name&#39;]
 **order_by** | **str**| Specifies the field and order to sort the results by. The value is composed of the field name followed by a colon and the sort direction (asc for ascending or desc for descending).  The default sort order is by date in ascending order. You can use the following fields:    - _date_    - _username_   - _from_    - _to_   - _status_    - _body_  For example, if you want to order by the most recently sent SMS, you should sort by date in descending order. The query would look like this:    &#x60;order_by&#x3D;date:desc&#x60; | [optional] [default to &#39;date:asc&#39;]
 **date_from** | **int**| Start date to filter results. It should be in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
 **date_to** | **int**| End date to filter results. It should be in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 

### Return type

[**ExportSmsHistory**](ExportSmsHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **export_voice_history**
> ExportVoiceHistory export_voice_history(content_type=content_type, filename=filename, q=q, order_by=order_by, date_from=date_from, date_to=date_to, limit=limit)

Export Voice History

_Export voice history_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| filename | query | string | true | Filename to export to |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.export_voice_history import ExportVoiceHistory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    filename = 'Voice_history.csv' # str |  (optional)
    q = 'q_example' # str |  (optional)
    order_by = 'date_added:desc' # str |  (optional)
    date_from = 'date_from_example' # str |  (optional)
    date_to = 'date_to_example' # str |  (optional)
    limit = 50000 # int |  (optional)

    try:
        # Export Voice History
        api_response = api_instance.export_voice_history(content_type=content_type, filename=filename, q=q, order_by=order_by, date_from=date_from, date_to=date_to, limit=limit)
        print("The response of DefaultApi->export_voice_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->export_voice_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **filename** | **str**|  | [optional] 
 **q** | **str**|  | [optional] 
 **order_by** | **str**|  | [optional] 
 **date_from** | **str**|  | [optional] 
 **date_to** | **str**|  | [optional] 
 **limit** | **int**|  | [optional] 

### Return type

[**ExportVoiceHistory**](ExportVoiceHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **forgot_password**
> ForgotPassword forgot_password(content_type=content_type, forgot_password_request=forgot_password_request)

Forgot Password

_Forgot password_

A user can send their username to this endpoint to be sent an email with their registered email address that will have a verification code.

Once you have this verification email containing the code you can send it to the [forgotten-password/verify](/#verify-forgot-password) endpoint along with a new password and the ID of that subaccount.

_Ask your administrator if you do not know your subaccount id._

### Properties

| **Name** | **Type** | **Required** | **Restrictions** | **Description** |
| --- | --- | --- | --- | --- |
| username | string | true | none | Username belonging to account |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #6BBD5B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint does not require authentication</span> 
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.forgot_password import ForgotPassword
from clicksend.models.forgot_password_request import ForgotPasswordRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    forgot_password_request = clicksend.ForgotPasswordRequest() # ForgotPasswordRequest |  (optional)

    try:
        # Forgot Password
        api_response = api_instance.forgot_password(content_type=content_type, forgot_password_request=forgot_password_request)
        print("The response of DefaultApi->forgot_password:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->forgot_password: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **forgot_password_request** | [**ForgotPasswordRequest**](ForgotPasswordRequest.md)|  | [optional] 

### Return type

[**ForgotPassword**](ForgotPassword.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **forgot_username**
> ForgotUsername forgot_username(content_type=content_type, forgot_username_request=forgot_username_request)

Forgot Username

_Forgot username_

Requires the user to pass either the email registered to an account or the phone number, **not** both

### Properties

| **Name** | **Type** | **Required** | **Restrictions** | **Description** |
| --- | --- | --- | --- | --- |
| email | string | true | none | Email belonging to account |
| phone_number | string | true | none | Phone belonging to account |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #6BBD5B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint does not require authentication</span> 
</div>   

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.forgot_username import ForgotUsername
from clicksend.models.forgot_username_request import ForgotUsernameRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    forgot_username_request = clicksend.ForgotUsernameRequest() # ForgotUsernameRequest |  (optional)

    try:
        # Forgot Username
        api_response = api_instance.forgot_username(content_type=content_type, forgot_username_request=forgot_username_request)
        print("The response of DefaultApi->forgot_username:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->forgot_username: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **forgot_username_request** | [**ForgotUsernameRequest**](ForgotUsernameRequest.md)|  | [optional] 

### Return type

[**ForgotUsername**](ForgotUsername.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **generate_new_api_key**
> GenerateNewApiKey generate_new_api_key(subaccount_id, content_type=content_type, generate_new_api_key_request=generate_new_api_key_request)

Generate New API Key

_Regenerate an API Key_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| subaccount_id | path | integer(int32) | true | ID of subaccount to regenerate API key for |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.generate_new_api_key import GenerateNewApiKey
from clicksend.models.generate_new_api_key_request import GenerateNewApiKeyRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    subaccount_id = 'subaccount_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    generate_new_api_key_request = clicksend.GenerateNewApiKeyRequest() # GenerateNewApiKeyRequest |  (optional)

    try:
        # Generate New API Key
        api_response = api_instance.generate_new_api_key(subaccount_id, content_type=content_type, generate_new_api_key_request=generate_new_api_key_request)
        print("The response of DefaultApi->generate_new_api_key:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->generate_new_api_key: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subaccount_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **generate_new_api_key_request** | [**GenerateNewApiKeyRequest**](GenerateNewApiKeyRequest.md)|  | [optional] 

### Return type

[**GenerateNewApiKey**](GenerateNewApiKey.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_all_delivery_issues**
> GetAllDeliveryIssues get_all_delivery_issues(content_type=content_type)

Get All Delivery Issues

_Get all delivery issues_

Get all delivery issues

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | Page number |
| limit | query | integer(int32) | false | Number of records per page |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.get_all_delivery_issues import GetAllDeliveryIssues
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # Get All Delivery Issues
        api_response = api_instance.get_all_delivery_issues(content_type=content_type)
        print("The response of DefaultApi->get_all_delivery_issues:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->get_all_delivery_issues: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**GetAllDeliveryIssues**](GetAllDeliveryIssues.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_alpha_tag**
> AlphaTag get_alpha_tag(alpha_tag_id, content_type=content_type)

Get Alpha Tag

_Get a specific alpha tag._

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| alpha_tag_id | path | uuid | true | ID of the alpha tag |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

 This endpoint requires authentication, [more info...](/#authentication)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.alpha_tag import AlphaTag
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    alpha_tag_id = 'alpha_tag_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Get Alpha Tag
        api_response = api_instance.get_alpha_tag(alpha_tag_id, content_type=content_type)
        print("The response of DefaultApi->get_alpha_tag:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->get_alpha_tag: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **alpha_tag_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**AlphaTag**](AlphaTag.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_countries_for_global_sending**
> GetCountriesForGlobalSending get_countries_for_global_sending()

Get Countries for Global Sending

_Get Countries for global sending_

Get the list of selected countries.

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.get_countries_for_global_sending import GetCountriesForGlobalSending
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)

    try:
        # Get Countries for Global Sending
        api_response = api_instance.get_countries_for_global_sending()
        print("The response of DefaultApi->get_countries_for_global_sending:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->get_countries_for_global_sending: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**GetCountriesForGlobalSending**](GetCountriesForGlobalSending.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_default_sender_details**
> GetDefaultSenderDetails get_default_sender_details(default_sender_id, content_type=content_type)

Get Default Sender Details

Retrieve detailed information about a specific default sender configuration

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.get_default_sender_details import GetDefaultSenderDetails
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    default_sender_id = 'default_sender_id_example' # str | The ID of the default sender to retrieve
    content_type = 'application/json' # str |  (optional)

    try:
        # Get Default Sender Details
        api_response = api_instance.get_default_sender_details(default_sender_id, content_type=content_type)
        print("The response of DefaultApi->get_default_sender_details:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->get_default_sender_details: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **default_sender_id** | **str**| The ID of the default sender to retrieve | 
 **content_type** | **str**|  | [optional] 

### Return type

[**GetDefaultSenderDetails**](GetDefaultSenderDetails.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_default_senders_list**
> GetDefaultSendersList get_default_senders_list(content_type=content_type, offset=offset, per_page=per_page, sort_by=sort_by, sort_direction=sort_direction)

Get List of Default Senders

Retrieve a list of default senders for the current user

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.get_default_senders_list import GetDefaultSendersList
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    offset = 'offset_example' # str | Page (offset) to be used for pagination (optional)
    per_page = 10 # int | Size of the page in pagination (optional) (default to 10)
    sort_by = 'created_timestamp' # str | Parameter to sort the results by (optional) (default to 'created_timestamp')
    sort_direction = desc # str | Direction of sorting (optional) (default to desc)

    try:
        # Get List of Default Senders
        api_response = api_instance.get_default_senders_list(content_type=content_type, offset=offset, per_page=per_page, sort_by=sort_by, sort_direction=sort_direction)
        print("The response of DefaultApi->get_default_senders_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->get_default_senders_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **offset** | **str**| Page (offset) to be used for pagination | [optional] 
 **per_page** | **int**| Size of the page in pagination | [optional] [default to 10]
 **sort_by** | **str**| Parameter to sort the results by | [optional] [default to &#39;created_timestamp&#39;]
 **sort_direction** | **str**| Direction of sorting | [optional] [default to desc]

### Return type

[**GetDefaultSendersList**](GetDefaultSendersList.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_own_number_detail**
> OwnNumber get_own_number_detail(own_number_id, content_type=content_type)

Get Own Number Detail

_Get a specific own numbers._

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| own_number_id | path | uuid | true | ID of the own number |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.own_number import OwnNumber
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    own_number_id = 'own_number_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Get Own Number Detail
        api_response = api_instance.get_own_number_detail(own_number_id, content_type=content_type)
        print("The response of DefaultApi->get_own_number_detail:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->get_own_number_detail: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **own_number_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**OwnNumber**](OwnNumber.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_specific_contact**
> GetSpecificContact get_specific_contact(list_id, contact_id, content_type=content_type)

Get Specific Contact

_Get a specific contact_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | Your contact list id you want to access. |
| contact_id | path | integer(int32) | true | Your contact id you want to access. |


Refer to [Status
Codes](/#status-codes) for
definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.get_specific_contact import GetSpecificContact
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    list_id = 'list_id_example' # str | 
    contact_id = 'contact_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # Get Specific Contact
        api_response = api_instance.get_specific_contact(list_id, contact_id, content_type=content_type)
        print("The response of DefaultApi->get_specific_contact:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->get_specific_contact: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **contact_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**GetSpecificContact**](GetSpecificContact.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_voice_history**
> GetVoiceHistory get_voice_history(content_type=content_type, date_to=date_to, limit=limit, operator=operator, order_by=order_by, page=page)

Get Voice History

_Get all voice history_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| date_from | query | integer(int32) | false | Start date (Unix Timestamp e.g. 1436849372) |
| date_to | query | integer(int32) | false | End date (Unix Timestamp e.g. 1436879372) |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.get_voice_history import GetVoiceHistory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    date_to = 'date_to_example' # str |  (optional)
    limit = 20 # int |  (optional)
    operator = 'AND' # str |  (optional)
    order_by = 'date_added:desc' # str |  (optional)
    page = 1 # int |  (optional)

    try:
        # Get Voice History
        api_response = api_instance.get_voice_history(content_type=content_type, date_to=date_to, limit=limit, operator=operator, order_by=order_by, page=page)
        print("The response of DefaultApi->get_voice_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->get_voice_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **date_to** | **str**|  | [optional] 
 **limit** | **int**|  | [optional] 
 **operator** | **str**|  | [optional] 
 **order_by** | **str**|  | [optional] 
 **page** | **int**|  | [optional] 

### Return type

[**GetVoiceHistory**](GetVoiceHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **import_contacts**
> ImportContacts import_contacts(list_id, content_type=content_type, import_contacts_request=import_contacts_request)

Import Contacts

_Import contacts to list_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | Your contact list id you want to access. |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| file_url | string | true | none | URL of file to process |
| field_order | \[string\] | true | none | Order of fields in file |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.import_contacts import ImportContacts
from clicksend.models.import_contacts_request import ImportContactsRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    list_id = 'list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    import_contacts_request = clicksend.ImportContactsRequest() # ImportContactsRequest |  (optional)

    try:
        # Import Contacts
        api_response = api_instance.import_contacts(list_id, content_type=content_type, import_contacts_request=import_contacts_request)
        print("The response of DefaultApi->import_contacts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->import_contacts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **import_contacts_request** | [**ImportContactsRequest**](ImportContactsRequest.md)|  | [optional] 

### Return type

[**ImportContacts**](ImportContacts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_alpha_tags**
> ListAlphaTags list_alpha_tags(sort_direction=sort_direction, page_size=page_size)

List Alpha Tags



### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.list_alpha_tags import ListAlphaTags
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    sort_direction = asc # str | The sort direction for the results. The default value is asc. (optional) (default to asc)
    page_size = 10 # int | The number of items to return per page. This parameter controls the size of each page of results. The default value is 10. (optional) (default to 10)

    try:
        # List Alpha Tags
        api_response = api_instance.list_alpha_tags(sort_direction=sort_direction, page_size=page_size)
        print("The response of DefaultApi->list_alpha_tags:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->list_alpha_tags: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sort_direction** | **str**| The sort direction for the results. The default value is asc. | [optional] [default to asc]
 **page_size** | **int**| The number of items to return per page. This parameter controls the size of each page of results. The default value is 10. | [optional] [default to 10]

### Return type

[**ListAlphaTags**](ListAlphaTags.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_compliant_sender_types**
> ListCompliantSenderTypes200Response list_compliant_sender_types(filter_product_type, filter_country_code_index=filter_country_code_index)

List Compliant Sender Types

Retrieves the list of compliant sender types for specific countries

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.list_compliant_sender_types200_response import ListCompliantSenderTypes200Response
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    filter_product_type = 'SMS' # str | Type of the product
    filter_country_code_index = ['filter_country_code_index_example'] # List[str] | Array of recipient country codes (ISO 3166-1 alpha-2). If not specified, will get all compliant sender types for all countries. Replace `{index}` with the appropriate index value.  <small>Example:</small> <small><code style=\"color: #424242;\">filter[country_code][0]=US&filter[country_code][1]=AU</code></small>  (optional)

    try:
        # List Compliant Sender Types
        api_response = api_instance.list_compliant_sender_types(filter_product_type, filter_country_code_index=filter_country_code_index)
        print("The response of DefaultApi->list_compliant_sender_types:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->list_compliant_sender_types: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filter_product_type** | **str**| Type of the product | 
 **filter_country_code_index** | [**List[str]**](str.md)| Array of recipient country codes (ISO 3166-1 alpha-2). If not specified, will get all compliant sender types for all countries. Replace &#x60;{index}&#x60; with the appropriate index value.  &lt;small&gt;Example:&lt;/small&gt; &lt;small&gt;&lt;code style&#x3D;\&quot;color: #424242;\&quot;&gt;filter[country_code][0]&#x3D;US&amp;filter[country_code][1]&#x3D;AU&lt;/code&gt;&lt;/small&gt;  | [optional] 

### Return type

[**ListCompliantSenderTypes200Response**](ListCompliantSenderTypes200Response.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_countries**
> ListCountries list_countries()

International Messaging

_List of countries_

List of countries with IDs that can be used in selecting countries for Global sending.

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.list_countries import ListCountries
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)

    try:
        # International Messaging
        api_response = api_instance.list_countries()
        print("The response of DefaultApi->list_countries:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->list_countries: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ListCountries**](ListCountries.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_own_numbers**
> ListOwnNumbers list_own_numbers(content_type=content_type)

List Own Numbers

_List own numbers._

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| offset | query | uuid | false | Page(offset) to be used for pagination. Example: `offset=f99872cc-11a6-48ba-a9f2-bcfb6dd1e3d4#8fa5ebc2-777b-45db-a448-ec76a40d4384` |
| page_size | query | integer | false | Number of records per page. Default: 10. Range \[1..500\] |
| filter\[status\]\[\] | query | string | false | Filter by statuses. Value must be in enum \[`PENDING`, `APPROVED`, `REJECTED`\]. For example: `filter[status][0]=PENDING&filter[status][1]=APPROVED` . |
| sort_by | query | string | false | Sort by parameter. Default: `created_timestamp` |
| sort_direction | query | string | false | Direction of sorting. Default: `asc`. Value must be in enum \[`asc`, `desc`\]. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

 This endpoint requires authentication, [more info...](/#authentication)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.list_own_numbers import ListOwnNumbers
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # List Own Numbers
        api_response = api_instance.list_own_numbers(content_type=content_type)
        print("The response of DefaultApi->list_own_numbers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->list_own_numbers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ListOwnNumbers**](ListOwnNumbers.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **mark_inbound_sms_as_read**
> MarkInboundSmsAsRead mark_inbound_sms_as_read(content_type=content_type, mark_sms_receipt_as_read_request=mark_sms_receipt_as_read_request)

Mark Inbound SMS as Read

Use this endpoint to mark all <a href="https://help.clicksend.com/article/ik4hw5xu35-can-i-receive-inbound-sms-to-my-url" target="_blank">inbound SMS</a> as read. Inbound SMS that has been marked as read won’t be shown in the **View Inbound SMS** endpoint. You can still use the **View Specific Inbound SMS** endpoint to view inbound SMS marked as read. 
In the request, you can optionally add a _date_before_ parameter to only mark inbound SMS sent before that date as read.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.mark_inbound_sms_as_read import MarkInboundSmsAsRead
from clicksend.models.mark_sms_receipt_as_read_request import MarkSmsReceiptAsReadRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    mark_sms_receipt_as_read_request = clicksend.MarkSmsReceiptAsReadRequest() # MarkSmsReceiptAsReadRequest |  (optional)

    try:
        # Mark Inbound SMS as Read
        api_response = api_instance.mark_inbound_sms_as_read(content_type=content_type, mark_sms_receipt_as_read_request=mark_sms_receipt_as_read_request)
        print("The response of DefaultApi->mark_inbound_sms_as_read:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->mark_inbound_sms_as_read: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **mark_sms_receipt_as_read_request** | [**MarkSmsReceiptAsReadRequest**](MarkSmsReceiptAsReadRequest.md)|  | [optional] 

### Return type

[**MarkInboundSmsAsRead**](MarkInboundSmsAsRead.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **mark_sms_receipt_as_read**
> MarkSmsReceiptAsRead mark_sms_receipt_as_read(content_type=content_type, mark_sms_receipt_as_read_request=mark_sms_receipt_as_read_request)

Mark SMS Receipt As Read

Use this endpoint to mark all <a target="_blank" href="https://help.clicksend.com/article/49eq1qdcui-how-do-i-receive-sms-delivery-receipts-delivery-status-updates">SMS delivery receipts</a> as read. Delivery receipts that have been marked as read won’t be shown in the **View SMS Receipts** endpoint. 
You can still use the **View Specific SMS Receipt** endpoint to view delivery receipts marked as read. In the request, you can optionally add a _date_before_ parameter to only mark receipts sent before that date as read

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.mark_sms_receipt_as_read import MarkSmsReceiptAsRead
from clicksend.models.mark_sms_receipt_as_read_request import MarkSmsReceiptAsReadRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    mark_sms_receipt_as_read_request = clicksend.MarkSmsReceiptAsReadRequest() # MarkSmsReceiptAsReadRequest |  (optional)

    try:
        # Mark SMS Receipt As Read
        api_response = api_instance.mark_sms_receipt_as_read(content_type=content_type, mark_sms_receipt_as_read_request=mark_sms_receipt_as_read_request)
        print("The response of DefaultApi->mark_sms_receipt_as_read:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->mark_sms_receipt_as_read: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **mark_sms_receipt_as_read_request** | [**MarkSmsReceiptAsReadRequest**](MarkSmsReceiptAsReadRequest.md)|  | [optional] 

### Return type

[**MarkSmsReceiptAsRead**](MarkSmsReceiptAsRead.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **mark_specific_inbound_sms_message_as_read**
> MarkSpecificInboundSmsMessageAsRead mark_specific_inbound_sms_message_as_read(message_id, content_type=content_type)

Mark Specific Inbound SMS Message As Read

Use this endpoint to mark a specific <a href="https://help.clicksend.com/article/ik4hw5xu35-can-i-receive-inbound-sms-to-my-url" target="_blank">inbound SMS</a> as read. Unlike the **View Inbound SMS** endpoint, which marks all inbound SMS as read, 
this endpoint only marks one specified inbound SMS. Specify the SMS to be marked as read by providing its _message_id_.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.mark_specific_inbound_sms_message_as_read import MarkSpecificInboundSmsMessageAsRead
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    message_id = 'message_id_example' # str | The message_id of the inbound SMS to mark as read.  <div class=\"info-box\">   <h4><i class=\"fas fa-info-circle\"></i> Note:</h4>   <p>     When you receive an inbound message, you will get two parameters: <em>original_message_id</em> and <em>message_id</em>:   </p>   <ul>     <li><em>original_message_id</em>: This is the ID of the outbound message sent to the recipient</li>     <li><em>message_id</em>: This is the ID of the inbound message sent by the recipient.</li>   </ul> </div>
    content_type = 'application/json' # str |  (optional)

    try:
        # Mark Specific Inbound SMS Message As Read
        api_response = api_instance.mark_specific_inbound_sms_message_as_read(message_id, content_type=content_type)
        print("The response of DefaultApi->mark_specific_inbound_sms_message_as_read:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->mark_specific_inbound_sms_message_as_read: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_id** | **str**| The message_id of the inbound SMS to mark as read.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;     When you receive an inbound message, you will get two parameters: &lt;em&gt;original_message_id&lt;/em&gt; and &lt;em&gt;message_id&lt;/em&gt;:   &lt;/p&gt;   &lt;ul&gt;     &lt;li&gt;&lt;em&gt;original_message_id&lt;/em&gt;: This is the ID of the outbound message sent to the recipient&lt;/li&gt;     &lt;li&gt;&lt;em&gt;message_id&lt;/em&gt;: This is the ID of the inbound message sent by the recipient.&lt;/li&gt;   &lt;/ul&gt; &lt;/div&gt; | 
 **content_type** | **str**|  | [optional] 

### Return type

[**MarkSpecificInboundSmsMessageAsRead**](MarkSpecificInboundSmsMessageAsRead.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **purchase_dedicated_number**
> PurchaseDedicatedNumber purchase_dedicated_number(dedicated_number, buy_number_request, content_type=content_type, type=type)

Purchase Dedicated Number

_Buy dedicated number_

This endpoint allows you to purchase a dedicated phone number for messaging services. You can optionally include registration data for compliance purposes.

### Request Body

| Field | Type | Required | Description |
| --- | --- | --- | --- |
| dedicated_number | string | true | Phone number to purchase |
| type | string | true | Service type (sms, mms) |
| registration_data | object | false | Registration data for compliance (AU SMS/MMS numbers only) |

#### Registration Data Fields (Optional)

| Field | Type | Required | Description |
| --- | --- | --- | --- |
| business_name | string | true | Name of the business (2 - 100 characters) |
| business_address | string | true | Business address (5 - 150 characters) |
| suburb | string | true | Suburb/City (2 - 50 characters) |
| postcode | string | true | Postal code (2 - 20 characters) |
| state | string | true | State/Province (2 - 50 characters) |
| contact_name | string | true | Contact person name (2 - 100 characters) |
| contact_number | string | true | Contact phone number (valid local or international phone number) |
| country | string | true | Country code (ISO 3166-1 alpha-2) |


### Path Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| dedicated_number | path | string | true | Phone number to purchase |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.buy_number_request import BuyNumberRequest
from clicksend.models.purchase_dedicated_number import PurchaseDedicatedNumber
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    dedicated_number = '+614197651956' # str | Phone number to purchase
    buy_number_request = clicksend.BuyNumberRequest() # BuyNumberRequest | 
    content_type = 'application/json' # str |  (optional)
    type = 'sms' # str |  (optional)

    try:
        # Purchase Dedicated Number
        api_response = api_instance.purchase_dedicated_number(dedicated_number, buy_number_request, content_type=content_type, type=type)
        print("The response of DefaultApi->purchase_dedicated_number:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->purchase_dedicated_number: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dedicated_number** | **str**| Phone number to purchase | 
 **buy_number_request** | [**BuyNumberRequest**](BuyNumberRequest.md)|  | 
 **content_type** | **str**|  | [optional] 
 **type** | **str**|  | [optional] 

### Return type

[**PurchaseDedicatedNumber**](PurchaseDedicatedNumber.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **purchase_recharge_package**
> PurchaseRechargePackage purchase_recharge_package(package_id, content_type=content_type)

Purchase Recharge Package

_Purchase a package_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| package_id | path | integer(int32) | true | ID of package to purchase |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.purchase_recharge_package import PurchaseRechargePackage
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    package_id = 'package_id_example' # str | 
    content_type = 'application/x-www-form-urlencoded' # str |  (optional)

    try:
        # Purchase Recharge Package
        api_response = api_instance.purchase_recharge_package(package_id, content_type=content_type)
        print("The response of DefaultApi->purchase_recharge_package:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->purchase_recharge_package: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **package_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**PurchaseRechargePackage**](PurchaseRechargePackage.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **register_numbers**
> RegisterNumbers register_numbers(number_type, country_code, content_type=content_type, register_numbers_request=register_numbers_request)

Register Numbers

<div style="background-color: #e8f4ff; padding: 15px; border-radius: 4px; border-left: 4px solid #0066cc;">
This endpoint is currently only available for <b>Canada 10DLC</b> number registration.
</div>

Registers a number that requires additional verification information. This endpoint facilitates the registration process for numbers requiring special compliance documentation.

After submission, ClickSend's compliance team will review the registration and notify you of the approval status.

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.
<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.register_numbers import RegisterNumbers
from clicksend.models.register_numbers_request import RegisterNumbersRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    number_type = '10dlc' # str | The type of number being registered
    country_code = 'US, CA' # str | Two-character ISO country code
    content_type = 'application/json' # str |  (optional)
    register_numbers_request = clicksend.RegisterNumbersRequest() # RegisterNumbersRequest |  (optional)

    try:
        # Register Numbers
        api_response = api_instance.register_numbers(number_type, country_code, content_type=content_type, register_numbers_request=register_numbers_request)
        print("The response of DefaultApi->register_numbers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->register_numbers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **number_type** | **str**| The type of number being registered | 
 **country_code** | **str**| Two-character ISO country code | 
 **content_type** | **str**|  | [optional] 
 **register_numbers_request** | [**RegisterNumbersRequest**](RegisterNumbersRequest.md)|  | [optional] 

### Return type

[**RegisterNumbers**](RegisterNumbers.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |
**400** | Bad request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **remove_duplicate_contacts**
> RemoveDuplicateContacts remove_duplicate_contacts(list_id, content_type=content_type, remove_duplicate_contacts_request=remove_duplicate_contacts_request)

Remove Duplicate Contacts

_Remove duplicate contacts_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | Your list id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.remove_duplicate_contacts import RemoveDuplicateContacts
from clicksend.models.remove_duplicate_contacts_request import RemoveDuplicateContactsRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    list_id = 'list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    remove_duplicate_contacts_request = clicksend.RemoveDuplicateContactsRequest() # RemoveDuplicateContactsRequest |  (optional)

    try:
        # Remove Duplicate Contacts
        api_response = api_instance.remove_duplicate_contacts(list_id, content_type=content_type, remove_duplicate_contacts_request=remove_duplicate_contacts_request)
        print("The response of DefaultApi->remove_duplicate_contacts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->remove_duplicate_contacts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **remove_duplicate_contacts_request** | [**RemoveDuplicateContactsRequest**](RemoveDuplicateContactsRequest.md)|  | [optional] 

### Return type

[**RemoveDuplicateContacts**](RemoveDuplicateContacts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **remove_opted_out_contacts**
> RemoveOptedOutContacts remove_opted_out_contacts(list_id, opt_out_list_id, content_type=content_type, body=body)

Remove Opted Out Contacts

_Remove all opted out contacts_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | Your list id |
| opt_out_list_id | path | integer(int32) | true | Your opt out list id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.remove_opted_out_contacts import RemoveOptedOutContacts
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    list_id = 'list_id_example' # str | 
    opt_out_list_id = 'opt_out_list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    body = None # object |  (optional)

    try:
        # Remove Opted Out Contacts
        api_response = api_instance.remove_opted_out_contacts(list_id, opt_out_list_id, content_type=content_type, body=body)
        print("The response of DefaultApi->remove_opted_out_contacts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->remove_opted_out_contacts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **opt_out_list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

[**RemoveOptedOutContacts**](RemoveOptedOutContacts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **request_alpha_tag**
> AlphaTag request_alpha_tag(content_type=content_type, request_alpha_tag_request=request_alpha_tag_request)

Request Alpha Tag

_Request to register an alpha tag. After requested, the alpha tag will be reviewed by ClickSend and either approved or rejected. Some countries (e.g Australia) require you to submit additional fields due to government mandated compliance checks._

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| alpha_tag | string | true | [yes](https://help.clicksend.com/article/1qxfxkcwm2-global-generic-alpha-tags) | The alpha tag name. Length must be between 3 - 11 characters, can only contain a-z A-Z 0-9 + and must contain at least one non numeric. |
| reason | string | false | none | Must be one of the following: `Sole Trader Name`, `Company Name`, `Partnership Name`, `Registered Trust Name`, `Co-Operative Name`, `Indigenous Corporation Name`, `Registered Organisation Name`, `Personal Name`, `Trademark`, `Government Agency or Entity`, `Product or Service Name`, `Acronym/Initialism`, `Contraction of Name`, `Third Party`. In case of `Third Party`, we will contact you to collect the relevant information. |
| countries | array of strings | false | none | List of country codes (e.g., "AU", "US") where the alpha tag is requested. Only supported and required for AU. |
| businesses | array of objects | false | none | List of business details required for alpha tag registration. Each object contains country, business information, ... Required if `countries` is provided. When `business_relationship` is `ENTITY_ASSOCIATE`, the following partner fields are also **required**: `partner_business_name`, `partner_abn`, `partner_business_info`, `partner_business_address`, `partner_representative`. These fields are **forbidden** for any other `business_relationship` value. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

_This endpoint requires authentication,_ [more info...](/#authentication)


### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.alpha_tag import AlphaTag
from clicksend.models.request_alpha_tag_request import RequestAlphaTagRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    request_alpha_tag_request = {"alpha_tag":"MyCompany","reason":"Company Name"} # RequestAlphaTagRequest |  (optional)

    try:
        # Request Alpha Tag
        api_response = api_instance.request_alpha_tag(content_type=content_type, request_alpha_tag_request=request_alpha_tag_request)
        print("The response of DefaultApi->request_alpha_tag:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->request_alpha_tag: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **request_alpha_tag_request** | [**RequestAlphaTagRequest**](RequestAlphaTagRequest.md)|  | [optional] 

### Return type

[**AlphaTag**](AlphaTag.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **request_own_number_verification_otp**
> RequestOwnNumberVerificationOtp request_own_number_verification_otp(content_type=content_type, request_own_number_verification_otp_request=request_own_number_verification_otp_request)

Request Own Number Verification OTP

_Request to generate own number verification OTP_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| label | string | false | none | Custom label for phone number. Length must be between 1 - 200 characters. |
| phone_number | string | true | none | Phone number. |
| country | string | false | none | Country code. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.request_own_number_verification_otp import RequestOwnNumberVerificationOtp
from clicksend.models.request_own_number_verification_otp_request import RequestOwnNumberVerificationOtpRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    request_own_number_verification_otp_request = clicksend.RequestOwnNumberVerificationOtpRequest() # RequestOwnNumberVerificationOtpRequest |  (optional)

    try:
        # Request Own Number Verification OTP
        api_response = api_instance.request_own_number_verification_otp(content_type=content_type, request_own_number_verification_otp_request=request_own_number_verification_otp_request)
        print("The response of DefaultApi->request_own_number_verification_otp:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->request_own_number_verification_otp: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **request_own_number_verification_otp_request** | [**RequestOwnNumberVerificationOtpRequest**](RequestOwnNumberVerificationOtpRequest.md)|  | [optional] 

### Return type

[**RequestOwnNumberVerificationOtp**](RequestOwnNumberVerificationOtp.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **reseller_transfer_credit**
> ResellerTransferCredit reseller_transfer_credit(content_type=content_type, update_payment_info_request=update_payment_info_request)

Reseller Transfer Credit

_Transfer Credit_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| client_user_id | integer(int32) | true | none | User ID of client |
| balance | integer(int32) | true | none | Balance to transfer |
| currency | string | true | none | Currency of balance to transfer |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.reseller_transfer_credit import ResellerTransferCredit
from clicksend.models.update_payment_info_request import UpdatePaymentInfoRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/x-www-form-urlencoded' # str |  (optional)
    update_payment_info_request = clicksend.UpdatePaymentInfoRequest() # UpdatePaymentInfoRequest |  (optional)

    try:
        # Reseller Transfer Credit
        api_response = api_instance.reseller_transfer_credit(content_type=content_type, update_payment_info_request=update_payment_info_request)
        print("The response of DefaultApi->reseller_transfer_credit:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->reseller_transfer_credit: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **update_payment_info_request** | [**UpdatePaymentInfoRequest**](UpdatePaymentInfoRequest.md)|  | [optional] 

### Return type

[**ResellerTransferCredit**](ResellerTransferCredit.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **select_countries_for_global_sending**
> SelectCountriesForGlobalSending select_countries_for_global_sending(select_countries_for_global_sending_request=select_countries_for_global_sending_request)

Select Countries for Global Sending

_Select Countries_

Use this endpoint to select countries that you intend to send sms / mms to. To remove / unselect a country, just remove the country id from the array in the payload.

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| country_list_ids | number | true | none | Country list ID's |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.select_countries_for_global_sending import SelectCountriesForGlobalSending
from clicksend.models.select_countries_for_global_sending_request import SelectCountriesForGlobalSendingRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    select_countries_for_global_sending_request = clicksend.SelectCountriesForGlobalSendingRequest() # SelectCountriesForGlobalSendingRequest |  (optional)

    try:
        # Select Countries for Global Sending
        api_response = api_instance.select_countries_for_global_sending(select_countries_for_global_sending_request=select_countries_for_global_sending_request)
        print("The response of DefaultApi->select_countries_for_global_sending:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->select_countries_for_global_sending: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **select_countries_for_global_sending_request** | [**SelectCountriesForGlobalSendingRequest**](SelectCountriesForGlobalSendingRequest.md)|  | [optional] 

### Return type

[**SelectCountriesForGlobalSending**](SelectCountriesForGlobalSending.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_email**
> SendEmail send_email(content_type=content_type, send_email_request=send_email_request)

Send Email

_Send transactional email_

Send transactional email

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| to | array | true | none | Array of To Recipient items. (array of names and emails) |
| cc | array | false | none | Array of Cc Recipient items. (array of names and emails) |
| bcc | array | false | none | Array of Bcc Recipient items. (array of names and emails) |
| from | object | true | none | From Email object. (object containing name and email) |
| body | string | true | none | Body of the email. |
| attachments | array | false | none | Array of Attachment items. |
| schedule | number | false | none | Schedule. |
| name | string | false | none | Name of person email belongs to |
| email | string | true | none | Email to be used. |
| content | string | true | none | The base64-encoded contents of the file. |
| type | string | true | none | The type of file being attached. |
| filename | string | true | none | The name of the file being attached. |
| disposition | string | true | none | Inline for content that can be displayed within the email, or attachment for any other files. |
| content_id | string | true | none | An ID for the content. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_email import SendEmail
from clicksend.models.send_email_request import SendEmailRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_email_request = clicksend.SendEmailRequest() # SendEmailRequest |  (optional)

    try:
        # Send Email
        api_response = api_instance.send_email(content_type=content_type, send_email_request=send_email_request)
        print("The response of DefaultApi->send_email:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->send_email: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_email_request** | [**SendEmailRequest**](SendEmailRequest.md)|  | [optional] 

### Return type

[**SendEmail**](SendEmail.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_email_campaign**
> SendEmailCampaign send_email_campaign(content_type=content_type, send_email_campaign_request=send_email_campaign_request)

Send Email Campaign

_Send email campaign_

Send email campaign

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| name | string | true | none | Your campaign name. |
| subject | string | true | none | Your campaign subject. |
| body | string | true | none | Your campaign message. |
| from_email_address_id | number | true | none | The allowed email address id. |
| from_name | string | true | none | Your name or business name. |
| template_id | number | false | none | Your template id. |
| list_id | number | true | none | Your contact list id. |
| schedule | integer(int32) | false | none | Your schedule timestamp. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_email_campaign import SendEmailCampaign
from clicksend.models.send_email_campaign_request import SendEmailCampaignRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_email_campaign_request = clicksend.SendEmailCampaignRequest() # SendEmailCampaignRequest |  (optional)

    try:
        # Send Email Campaign
        api_response = api_instance.send_email_campaign(content_type=content_type, send_email_campaign_request=send_email_campaign_request)
        print("The response of DefaultApi->send_email_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->send_email_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_email_campaign_request** | [**SendEmailCampaignRequest**](SendEmailCampaignRequest.md)|  | [optional] 

### Return type

[**SendEmailCampaign**](SendEmailCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_email_verification_token**
> SendEmailVerificationToken send_email_verification_token(email_address_id, content_type=content_type, send_email_verification_token_request=send_email_verification_token_request)

Send Email Verification Token

_Send verification token_

Send verification token

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| email_address_id | path | integer(int32) | true | Allowed email address id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_email_verification_token import SendEmailVerificationToken
from clicksend.models.send_email_verification_token_request import SendEmailVerificationTokenRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    email_address_id = 'email_address_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    send_email_verification_token_request = clicksend.SendEmailVerificationTokenRequest() # SendEmailVerificationTokenRequest |  (optional)

    try:
        # Send Email Verification Token
        api_response = api_instance.send_email_verification_token(email_address_id, content_type=content_type, send_email_verification_token_request=send_email_verification_token_request)
        print("The response of DefaultApi->send_email_verification_token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->send_email_verification_token: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_address_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **send_email_verification_token_request** | [**SendEmailVerificationTokenRequest**](SendEmailVerificationTokenRequest.md)|  | [optional] 

### Return type

[**SendEmailVerificationToken**](SendEmailVerificationToken.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_fax**
> SendFax send_fax(content_type=content_type, send_fax_request=send_fax_request)

Send Fax

### **Supported File Types**

- Supported file types are listed below. If you need to convert a file to a supported format, it can be first passed to our uploads endpoint: `/uploads?convert=fax`
- This will return a URL to the converted pdf file that can be used in the /fax/send endpoint.
- Contact us to add support for any other file type.
    

### Documents

| File type | Required to be passed to uploads endpoint first? |
| --- | --- |
| pdf | No |
| docx | Yes |
| doc | Yes |
| rtf | Yes |

_Send a fax using supplied supported file-types._

### **Letter File Options**

### Use existing URL

With this option, you can use an existing URL to a `pdf` document. For example, you might generate the `pdf` on your server.

When using an existing url make sure that it is publicly accessible as it will not work if it is private.

### Upload File to Our Server

With this option, you can use the [/uploads](/#upload-media-file) endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/fax/send` endpoint.

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| file_url | string | true | none | URL of file to send |
| source | string | true | none | Your method of sending e.g. 'wordpress', 'php', 'c#'. |
| to | string | true | none | Recipient fax number in [E.164](https://en.wikipedia.org/wiki/E.164) format. |
| list_id | integer(int32) | false | none | Your list ID if sending to a whole list. Can be used instead of 'to'. |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id. Must be a valid fax number. |
| schedule | integer(int32) | false | none | Leave blank for immediate delivery. Your schedule time in unix format [http://help.clicksend.com/what-is-a-unix-timestamp](http://help.clicksend.com/what-is-a-unix-timestamp) |
| custom_string | string | false | none | Your reference. Will be passed back with all replies and delivery reports. |
| country | string | false | none | ISO alpha-2 character country code e.g. 'US', we use this to format the recipient number if it's not in international format. |
| from_email | string | false | none | An email address where the reply should be emailed to. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_fax import SendFax
from clicksend.models.send_fax_request import SendFaxRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_fax_request = clicksend.SendFaxRequest() # SendFaxRequest |  (optional)

    try:
        # Send Fax
        api_response = api_instance.send_fax(content_type=content_type, send_fax_request=send_fax_request)
        print("The response of DefaultApi->send_fax:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->send_fax: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_fax_request** | [**SendFaxRequest**](SendFaxRequest.md)|  | [optional] 

### Return type

[**SendFax**](SendFax.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_letter**
> SendLetter send_letter(content_type=content_type, send_letter_request=send_letter_request)

Send Letter

### Send letter

### **Supported File Types**

We support `pdf`, `docx` and `doc` files. Contact us to add support for any other file type. If you're using `docx` or `doc` files, you'll need to convert the file first using our uploads endpoint with the querystring parameter `convert=post` e.g. `POST https://rest.clicksend.com/v3/uploads?convert=post`. This will return a URL to the converted pdf file that can be used in the `/post/letters/send` endpoint.

### **Letter Specification Guide**

Follow our [Letter specification guide](https://help.clicksend.com/article/wcpkkoou6c-post-letter-template) to ensure correct sending and letter template information.

### **Letter File Options**

### Use existing URL

With this option, you can use an existing URL to a `pdf` document. For example, you might generate the `pdf` on your server.

When using an existing url make sure that it is publicly accessible as it will not work if it is private.

### Upload File to Our Server

With this option, you can use the [/uploads](/#upload-media-file) endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/post/letters/send` endpoint.

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| file_url | string | true | none | URL of file to send |
| address_name | string | true | none | Name of address |
| address_line_1 | string | true | none | First line of address |
| address_line_2 | string | true | none | Second line of address |
| address_city | string | true | none | City |
| address_state | string | true | none | State |
| address_postal_code | string | true | none | Postal code |
| address_country | string | true | none | Country |
| return_address_id | integer(int32) | true | none | ID of return address to use |
| schedule | integer(int32) | false | none | When to send letter (0/null=now) |
| template_used | integer(int1) | false | none | Whether using our letter template. Flag value must be 1 for yes or 0 for no. |
| duplex | integer(int1) | false | none | Whether letter is duplex. Flag value must be 1 for yes or 0 for no. |
| colour | integer(int1) | false | none | Whether letter is in colour. Flag value must be 1 for yes or 0 for no. |
| priority_post | integer(int1) | false | none | Whether letter is priority, Flag value must be 1 for yes or 0 for no. |
| source | string | false | none | Source being sent from |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_letter import SendLetter
from clicksend.models.send_letter_request import SendLetterRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_letter_request = clicksend.SendLetterRequest() # SendLetterRequest |  (optional)

    try:
        # Send Letter
        api_response = api_instance.send_letter(content_type=content_type, send_letter_request=send_letter_request)
        print("The response of DefaultApi->send_letter:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->send_letter: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_letter_request** | [**SendLetterRequest**](SendLetterRequest.md)|  | [optional] 

### Return type

[**SendLetter**](SendLetter.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_mms**
> SendMms send_mms(content_type=content_type, send_mms_request=send_mms_request)

Send MMS

_Send MMS_

You can post **up to 1000 messages** with each API call. You can send to a mix of contacts and contact lists, as long as the total number of recipients is up to 1000. The response contains a status and details for each recipient.

Refer to [<b>Application Status Codes</b>](/#application-status-codes) for the possible response message status strings.

### **How many characters can I send in a message?**

### Standard MMS Message

1500 characters

### Unicode MMS Message

500 characters

If a message is longer the allowed number of characters it will be truncated. If a message contains any characters that aren't in the GSM 03.38 character set, the message type will be treated as unicode. ([https://en.wikipedia.org/wiki/GSM_03.38](https://en.wikipedia.org/wiki/GSM_03.38))

### Maximum File Size

You can send a single attachment with a size of up to 250 kB. Some older devices can only accept attachments with up to 30 kB.

### Supported File Types

- Supported file types are listed below. If you need to convert a file to a supported format, it can be first passed to our uploads endpoint: `/uploads?convert=mms`
- This will return a URL to the converted image file that can be used in the /mms/send endpoint.
- Contact us to add support for any other file type.
    

### Images

| File type | Required to be passed to uploads endpoint first? |
| --- | --- |
| `jpg` | No |
| `gif` | No |
| `jpeg` | Yes |
| `png` | Yes |
| `bmp` | Yes |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| media_file | string | true | none | Media file you want to send |
| to | string | true | none | Recipient phone number in [E.164](https://en.wikipedia.org/wiki/E.164) format |
| body | string | true | none | Your message |
| subject | string | true | none | Subject line (max 20 characters) |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_mms import SendMms
from clicksend.models.send_mms_request import SendMmsRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_mms_request = clicksend.SendMmsRequest() # SendMmsRequest |  (optional)

    try:
        # Send MMS
        api_response = api_instance.send_mms(content_type=content_type, send_mms_request=send_mms_request)
        print("The response of DefaultApi->send_mms:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->send_mms: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_mms_request** | [**SendMmsRequest**](SendMmsRequest.md)|  | [optional] 

### Return type

[**SendMms**](SendMms.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_mms_campaign**
> SendMmsCampaign send_mms_campaign(content_type=content_type, send_mms_campaign_request=send_mms_campaign_request)

Send MMS Campaign

_Create mms campaign_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| list_id | integer(int32) | true | none | Your list id. |
| name | string | true | none | Your campaign name. |
| body | string | true | none | Your campaign message. |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id |
| schedule | integer(int32) | false | none | Your schedule timestamp. |
| subject | string | true | none | Subject of MMS campaign. |
| media_file | string | true | none | URL pointing to media file. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_mms_campaign import SendMmsCampaign
from clicksend.models.send_mms_campaign_request import SendMmsCampaignRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_mms_campaign_request = clicksend.SendMmsCampaignRequest() # SendMmsCampaignRequest |  (optional)

    try:
        # Send MMS Campaign
        api_response = api_instance.send_mms_campaign(content_type=content_type, send_mms_campaign_request=send_mms_campaign_request)
        print("The response of DefaultApi->send_mms_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->send_mms_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_mms_campaign_request** | [**SendMmsCampaignRequest**](SendMmsCampaignRequest.md)|  | [optional] 

### Return type

[**SendMmsCampaign**](SendMmsCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_postcard**
> SendPostcard send_postcard(content_type=content_type, send_postcard_request=send_postcard_request)

Send Postcard

_Send one or more postcards_

### **Supported File Types**

We support PDF, docx, doc, jpg, gif, png, and bmp. Contact us to add support for any other file type. If you're using docx, doc, jpg, gif, png, or bmp files, you'll need to convert the file first using our uploads endpoint with the querystring parameter ?convert=postcard. e.g. POST /uploads?convert=postcard. This will return a URL to the converted pdf file that can be used in the /post/postcards/send endpoint.

### **Postcard Specification Guide**

Follow our [Postcard specification guide](https://help.clicksend.com/article/ysyql7bsr1-postcard-template) to ensure correct sending and postcard template information.

### **Postcard File Options**

### Use existing URL

With this option, you can use an existing URL to a `pdf` document. For example, you might generate the `pdf` on your server.

When using an existing url make sure that it is publicly accessible as it will not work if it is private.

For `file_urls` field. You can attach at least 1 and max of 2 PDF file urls.

- Supply a single pdf with 2 pages (front and back)
- Supply 2 urls to seperate PDFs
    

### Upload File to Our Server

With this option, you can use the [/uploads](/#upload-media-file) endpoint to upload the document. The `/uploads` endpoint returns a URL that can be used in the `/post/postcards/send` endpoint.

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| file_urls | \[string\] | true | none | Postcard file URLs |
| address_name | string | true | none | Name of address |
| address_line_1 | string | true | none | First line of address |
| address_line_2 | string | true | none | Second line of address |
| address_city | string | true | none | City |
| address_state | string | true | none | State |
| address_postal_code | string | true | none | Postal code |
| address_country | string | true | none | Country |
| return_address_id | integer(int32) | true | none | ID of return address to use |
| schedule | integer(int32) | false | none | When to send letter (0/null=now) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_postcard import SendPostcard
from clicksend.models.send_postcard_request import SendPostcardRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_postcard_request = clicksend.SendPostcardRequest() # SendPostcardRequest |  (optional)

    try:
        # Send Postcard
        api_response = api_instance.send_postcard(content_type=content_type, send_postcard_request=send_postcard_request)
        print("The response of DefaultApi->send_postcard:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->send_postcard: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_postcard_request** | [**SendPostcardRequest**](SendPostcardRequest.md)|  | [optional] 

### Return type

[**SendPostcard**](SendPostcard.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_sms**
> SendSms send_sms(content_type=content_type, send_sms_request=send_sms_request)

Send SMS

Use this endpoint to send messages to your recipients, either as phone numbers or contacts from your contact list. 
The sender of the message (<a href="https://help.clicksend.com/article/4kgj7krx00-what-is-a-sender-id-or-sender-number" target="_blank"><strong>Sender ID</strong></a>) can be a shared number, a dedicated number, alpha tag (business name), or your own number. 
You can send messages both locally and globally, subject to the country restrictions. The cost of sending messages varies based on the <a href="https://help.clicksend.com/article/h474eseq3a-how-many-characters-can-i-send-in-an-sms" target="_blank">type</a> and length of the message.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_sms import SendSms
from clicksend.models.send_sms_request import SendSmsRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_sms_request = {"messages":[{"source":"php","body":"Jelly liquorice marshmallow candy carrot cake 4Eyffjs1vL.","to":"+61411111111"},{"source":"php","body":"Chocolate bar icing icing oat cake carrot cake jelly cotton MWEvciEPIr.","to":"+61422222222"}]} # SendSmsRequest |  (optional)

    try:
        # Send SMS
        api_response = api_instance.send_sms(content_type=content_type, send_sms_request=send_sms_request)
        print("The response of DefaultApi->send_sms:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->send_sms: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_sms_request** | [**SendSmsRequest**](SendSmsRequest.md)|  | [optional] 

### Return type

[**SendSms**](SendSms.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_sms_campaign**
> SendSmsCampaign send_sms_campaign(content_type=content_type, send_sms_campaign_request=send_sms_campaign_request)

Send SMS Campaign

### _SMS Campaign Endpoint_

You can post to a list with `up to 20000 recipients` with each API call. You can only send to a single list containing up to 20,000 recipients. The response is far less detailed than the normal Send SMS endpoint. Use the [SMS Send](/#send-sms) endpoint if you would like to send to less than 1000 recipients at once.
You are required to add an opt-out message to the end of your message body if you are sending marketing message. This can be in the form of asking users to reply STOP to opt-out or by including `StopMsg.me/xxxxx` which is a placeholder that will add a link that can be clicked to out-out.
Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.
<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_sms_campaign import SendSmsCampaign
from clicksend.models.send_sms_campaign_request import SendSmsCampaignRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_sms_campaign_request = clicksend.SendSmsCampaignRequest() # SendSmsCampaignRequest |  (optional)

    try:
        # Send SMS Campaign
        api_response = api_instance.send_sms_campaign(content_type=content_type, send_sms_campaign_request=send_sms_campaign_request)
        print("The response of DefaultApi->send_sms_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->send_sms_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_sms_campaign_request** | [**SendSmsCampaignRequest**](SendSmsCampaignRequest.md)|  | [optional] 

### Return type

[**SendSmsCampaign**](SendSmsCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **send_voice_message**
> SendVoiceMessage send_voice_message(content_type=content_type, send_voice_message_request=send_voice_message_request)

Send Voice Message

_Send voice message(s)_

Send TTS (Text-to-speech) voice calls

### How many messages can I send?

You can post **up to 1000 messages** with each API call. You can send to a mix of contacts and contact lists, as long as the total number of recipients is up to 1000. The response contains a status and details for each recipient.

### How many characters can I send in a message?

If a message is longer than 4 message parts, it will be truncated (see below). If a message contains any characters that aren't in the GSM 03.38 character set, the message type will be treated as unicode. (`https://en.wikipedia.org/wiki/GSM_03.38`)

### _Standard English Characters:_

| Number of Characters | Message Credits |
| --- | --- |
| 1 - 300 | 1 |
| 301 - 600 | 2 |
| 601 - 900 | 3 |
| 901 - 1200 | 4 |

### _Non-GSM (Unicode) characters:_

| Number of Characters | Message Credits |
| --- | --- |
| 1 - 150 | 1 |
| 151 - 300 | 2 |
| 301 - 450 | 3 |
| 451 - 600 | 4 |

### _Allowed Languages_

| Language, Locale | lang | voice |
| --- | --- | --- |
| `English`, US | en-us | female (default) / male |
| `English`, Australia | en-au | female (default) / male |
| `English`, UK | en-gb | female (default) / male |
| `English`, India | en-in | female |
| `English`, Wales | en-gb-wls | female (default) / male |
| `Celtic`, Wales | cy-gb-wls | female (default) / male |
| `German`, Germany | de-de | female (default) / male |
| `Spanish`, Spain | es-es | female (default) / male |
| `Spanish`, US | es-us | female (default) / male |
| `French`, Canada | fr-ca | female |
| `French`, France | fr-fr | female (default) / male |
| `Icelandic`, Iceland | is-is | female (default) / male |
| `Italian`, Italy | it-it | female (default) / male |
| `Danish`, Denmark | da-dk | female (default) / male |
| `Dutch`, Netherlands | nl-nl | female (default) / male |
| `Norwegian`, Norway | nb-no | female |
| `Polish`, Poland | pl-pl | female (default) / male |
| `Portuguese`, Portugal | pt-pt | male |
| `Portuguese`, Brazil | pt-br | female (default) / male |
| `Romanian`, Romania | ro-ro | female |
| `Russian`, Russia | ru-ru | female (default) / male |
| `Swedish`, Sweden | sv-se | female |
| `Turkish`, Turkey | tr-tr | female |

_Tips_

To introduce a small delay between words or digits you can use a comma (,).

For example: `Please enter your activation code 9, 0, 9, 0, in the next 20 minutes.`

We support some SSML tags allowing custom breaks or pauses to be entered, and the readout rate to be altered.

[More info...](https://help.clicksend.com/en/articles/42982-customising-text-to-voice-output)

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| to | string | true | none | Your phone number in [E.164](https://en.wikipedia.org/wiki/E.164) format. |
| body | string | true | none | Biscuit uv3nlCOjRk croissant chocolate lollipop chocolate muffin. |
| voice | string | true | none | Either 'female' or 'male'. |
| custom_string | string | true | none | Your reference. Will be passed back with all replies and delivery reports. |
| country | string | true | none | The country of the recipient. |
| source | string | false | none | Your method of sending e.g. 'wordpress', 'php', 'c#'. |
| list_id | integer(int32) | false | none | Your list ID if sending to a whole list. Can be used instead of 'to'. |
| lang | string | false | none | au (string, required) - See section on available languages. |
| schedule | integer(int32) | false | none | Leave blank for immediate delivery. Your schedule time in unix format [http://help.clicksend.com/what-is-a-unix-timestamp](http://help.clicksend.com/what-is-a-unix-timestamp) |
| require_input | integer(int1) | false | none | Recieve a keypress from the recipient. Flag value must be 1 for yes or 0 for no. |
| machine_detection | integer(int1) | false | none | Detect answering machine or voicemail and leave a message. Flag value must be 1 for yes or 0 for no. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.send_voice_message import SendVoiceMessage
from clicksend.models.send_voice_message_request import SendVoiceMessageRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    send_voice_message_request = clicksend.SendVoiceMessageRequest() # SendVoiceMessageRequest |  (optional)

    try:
        # Send Voice Message
        api_response = api_instance.send_voice_message(content_type=content_type, send_voice_message_request=send_voice_message_request)
        print("The response of DefaultApi->send_voice_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->send_voice_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **send_voice_message_request** | [**SendVoiceMessageRequest**](SendVoiceMessageRequest.md)|  | [optional] 

### Return type

[**SendVoiceMessage**](SendVoiceMessage.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **short_url_get_statistics**
> GetStatistics short_url_get_statistics(source, source_id, content_type=content_type)

Get Statistics

Use this endpoint to get the aggregated statistics for a shortened URL. This allows you to track the total number of clicks on the link. You can gather details such as the device type and where it was opened from as well.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.get_statistics import GetStatistics
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    source = 'source_example' # str | Source of the request.
    source_id = 'source_id_example' # str | ID of the source (e.g. message ID).
    content_type = 'application/json' # str |  (optional)

    try:
        # Get Statistics
        api_response = api_instance.short_url_get_statistics(source, source_id, content_type=content_type)
        print("The response of DefaultApi->short_url_get_statistics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->short_url_get_statistics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **source** | **str**| Source of the request. | 
 **source_id** | **str**| ID of the source (e.g. message ID). | 
 **content_type** | **str**|  | [optional] 

### Return type

[**GetStatistics**](GetStatistics.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **short_url_get_tracking**
> GetTracking short_url_get_tracking(long_url_id, content_type=content_type)

Get Tracking

Use this endpoint to track how individual recipients interact with the link.  It returns data from the most recent click, including statistics such as how many times they’ve visited the link and when it was last opened. To use this endpoint, reference the _long_url_id_ provided in the [GET /short-url/statistics](/messaging/url-shortening/other/short-url-get-statistics) endpoint.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.get_tracking import GetTracking
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    long_url_id = 'long_url_id_example' # str | ID of the long URL (uniquely defined by the source, source ID, and long URL). Obtained from the GET statistics endpoint.
    content_type = 'application/json' # str |  (optional)

    try:
        # Get Tracking
        api_response = api_instance.short_url_get_tracking(long_url_id, content_type=content_type)
        print("The response of DefaultApi->short_url_get_tracking:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->short_url_get_tracking: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **long_url_id** | **str**| ID of the long URL (uniquely defined by the source, source ID, and long URL). Obtained from the GET statistics endpoint. | 
 **content_type** | **str**|  | [optional] 

### Return type

[**GetTracking**](GetTracking.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **timezones**
> Timezones timezones(content_type=content_type)

Timezones

_Get supported list of timezones._

Get supported list of timezones.

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | Page number |
| limit | query | integer(int32) | false | Number of records per page |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.timezones import Timezones
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # Timezones
        api_response = api_instance.timezones(content_type=content_type)
        print("The response of DefaultApi->timezones:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->timezones: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**Timezones**](Timezones.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **transfer_contact_to_list**
> TransferContactToList transfer_contact_to_list(from_list_id, contact_id, to_list_id, content_type=content_type, body=body)

Transfer Contact to List

_Transfer contact to another list_

Transfer contact to another list

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| from_list_id | path | integer(int32) | true | List ID for list that contains contact. |
| contact_id | path | integer(int32) | true | Contact ID |
| to_list_id | path | integer(int32) | true | List ID for list you want to transfer contact to. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.transfer_contact_to_list import TransferContactToList
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    from_list_id = 'from_list_id_example' # str | 
    contact_id = 'contact_id_example' # str | 
    to_list_id = 'to_list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    body = None # object |  (optional)

    try:
        # Transfer Contact to List
        api_response = api_instance.transfer_contact_to_list(from_list_id, contact_id, to_list_id, content_type=content_type, body=body)
        print("The response of DefaultApi->transfer_contact_to_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->transfer_contact_to_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **from_list_id** | **str**|  | 
 **contact_id** | **str**|  | 
 **to_list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

[**TransferContactToList**](TransferContactToList.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_client_account**
> UpdateClientAccount update_client_account(client_user_id, content_type=content_type, update_payment_info_request=update_payment_info_request)

Update Client Account

_Update Reseller clients Account_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| client_user_id | path | integer(int32) | true | User ID of client |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| username | string | true | none | Account username |
| password | string | true | none | Account password (unhashed) |
| user_email | string | true | none | Account email |
| user_phone | string | true | none | Account phone number |
| user_first_name | string | true | none | Account owner first name |
| user_last_name | string | true | none | Account owner last name |
| account_name | string | true | none | Account name (usually company name) |
| country | string | true | none | Country of account holder |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.update_client_account import UpdateClientAccount
from clicksend.models.update_payment_info_request import UpdatePaymentInfoRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    client_user_id = 'client_user_id_example' # str | 
    content_type = 'application/x-www-form-urlencoded' # str |  (optional)
    update_payment_info_request = clicksend.UpdatePaymentInfoRequest() # UpdatePaymentInfoRequest |  (optional)

    try:
        # Update Client Account
        api_response = api_instance.update_client_account(client_user_id, content_type=content_type, update_payment_info_request=update_payment_info_request)
        print("The response of DefaultApi->update_client_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_client_account: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **client_user_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **update_payment_info_request** | [**UpdatePaymentInfoRequest**](UpdatePaymentInfoRequest.md)|  | [optional] 

### Return type

[**UpdateClientAccount**](UpdateClientAccount.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_contact**
> UpdateContact update_contact(list_id, contact_id, content_type=content_type, create_new_contact_request=create_new_contact_request)

Update Contact

_Update specific contact_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | Contact list id |
| contact_id | path | integer(int32) | true | Contact ID |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| phone_number | string | true | none | Your phone number in [E.164](https://en.wikipedia.org/wiki/E.164) format. Must be provided if no fax number or email. |
| email | string | false | none | Your email. Must be provided if no phone number or fax number. |
| fax_number | string | false | none | Your fax number. Must be provided if no phone number or email. |
| first_name | string | false | none | Your first name. |
| address_line_1 | string | false | none | Your street address |
| address_line_2 | string | false | none | none |
| address_city | string | false | none | Your nearest city |
| address_state | string | false | none | Your current state |
| address_postal_code | string | false | none | Your current postcode |
| address_country | string | false | none | Your current country |
| organization_name | string | false | none | Your organisation name |
| custom_1 | string | true | none | none |
| custom_2 | string | false | none | none |
| custom_3 | string | false | none | none |
| custom_4 | string | false | none | none |
| last_name | string | false | none | Your last name |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_new_contact_request import CreateNewContactRequest
from clicksend.models.update_contact import UpdateContact
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    list_id = 'list_id_example' # str | 
    contact_id = 'contact_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    create_new_contact_request = clicksend.CreateNewContactRequest() # CreateNewContactRequest |  (optional)

    try:
        # Update Contact
        api_response = api_instance.update_contact(list_id, contact_id, content_type=content_type, create_new_contact_request=create_new_contact_request)
        print("The response of DefaultApi->update_contact:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_contact: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **contact_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **create_new_contact_request** | [**CreateNewContactRequest**](CreateNewContactRequest.md)|  | [optional] 

### Return type

[**UpdateContact**](UpdateContact.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_default_sender**
> UpdateDefaultSender update_default_sender(default_sender_id, content_type=content_type, update_default_sender_request=update_default_sender_request)

Update Default Sender

Updates the details of an existing default sender configuration.

For more information on Sender IDs, please refer to [What is a Sender ID or Sender Number?](https://help.clicksend.com/article/4kgj7krx00-what-is-a-sender-id-or-sender-number)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.update_default_sender import UpdateDefaultSender
from clicksend.models.update_default_sender_request import UpdateDefaultSenderRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    default_sender_id = 'default_sender_id_example' # str | The ID of the default sender to update
    content_type = 'application/json' # str |  (optional)
    update_default_sender_request = clicksend.UpdateDefaultSenderRequest() # UpdateDefaultSenderRequest |  (optional)

    try:
        # Update Default Sender
        api_response = api_instance.update_default_sender(default_sender_id, content_type=content_type, update_default_sender_request=update_default_sender_request)
        print("The response of DefaultApi->update_default_sender:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_default_sender: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **default_sender_id** | **str**| The ID of the default sender to update | 
 **content_type** | **str**|  | [optional] 
 **update_default_sender_request** | [**UpdateDefaultSenderRequest**](UpdateDefaultSenderRequest.md)|  | [optional] 

### Return type

[**UpdateDefaultSender**](UpdateDefaultSender.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |
**400** | Bad request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_email_campaign**
> UpdateEmailCampaign update_email_campaign(email_campaign_id, content_type=content_type, update_email_campaign_request=update_email_campaign_request)

Update Email Campaign

_Edit email campaign_

Edit email campaign

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| email_campaign_id | path | integer(int32) | true | Allowed email campaign id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.update_email_campaign import UpdateEmailCampaign
from clicksend.models.update_email_campaign_request import UpdateEmailCampaignRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    email_campaign_id = 'email_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    update_email_campaign_request = clicksend.UpdateEmailCampaignRequest() # UpdateEmailCampaignRequest |  (optional)

    try:
        # Update Email Campaign
        api_response = api_instance.update_email_campaign(email_campaign_id, content_type=content_type, update_email_campaign_request=update_email_campaign_request)
        print("The response of DefaultApi->update_email_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_email_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **update_email_campaign_request** | [**UpdateEmailCampaignRequest**](UpdateEmailCampaignRequest.md)|  | [optional] 

### Return type

[**UpdateEmailCampaign**](UpdateEmailCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_email_delivery_receipt_rule**
> UpdateEmailDeliveryReceiptRule update_email_delivery_receipt_rule(receipt_rule_id, content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)

Update Email Delivery Receipt Rule

_Update email delivery receipt automation_

Update email delivery receipt automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| receipt_rule_id | path | integer(int32) | true | Receipt rule id |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| rule_name | string | true | none | Rule Name. |
| match_type | number | true | none | Match Type. 0=All reports. |
| action | string | true | none | Action to be taken (AUTO_REPLY, EMAIL_USER, EMAIL_FIXED, URL, SMS, POLL, GROUP_SMS, MOVE_CONTACT, CREATE_CONTACT, CREATE_CONTACT_PLUS_EMAIL, CREATE_CONTACT_PLUS_NAME_EMAIL CREATE_CONTACT_PLUS_NAME, SMPP, NONE). |
| action_address | string | true | none | Action address. |
| enabled | number | true | none | Enabled: Disabled=0 or Enabled=1. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_sms_delivery_receipt_rule_request import CreateSmsDeliveryReceiptRuleRequest
from clicksend.models.update_email_delivery_receipt_rule import UpdateEmailDeliveryReceiptRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    create_sms_delivery_receipt_rule_request = clicksend.CreateSmsDeliveryReceiptRuleRequest() # CreateSmsDeliveryReceiptRuleRequest |  (optional)

    try:
        # Update Email Delivery Receipt Rule
        api_response = api_instance.update_email_delivery_receipt_rule(receipt_rule_id, content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)
        print("The response of DefaultApi->update_email_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_email_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **create_sms_delivery_receipt_rule_request** | [**CreateSmsDeliveryReceiptRuleRequest**](CreateSmsDeliveryReceiptRuleRequest.md)|  | [optional] 

### Return type

[**UpdateEmailDeliveryReceiptRule**](UpdateEmailDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_email_template**
> UpdateEmailTemplate update_email_template(template_id, content_type=content_type, update_email_template_request=update_email_template_request)

Update Email Template

_Update email template_

Update email template

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| template_id | path | integer(int32) | true | Email template id |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| template_name | string | false | none | The intended name for the template. |
| body | string | true | none | Your template body. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.update_email_template import UpdateEmailTemplate
from clicksend.models.update_email_template_request import UpdateEmailTemplateRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    template_id = 'template_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    update_email_template_request = clicksend.UpdateEmailTemplateRequest() # UpdateEmailTemplateRequest |  (optional)

    try:
        # Update Email Template
        api_response = api_instance.update_email_template(template_id, content_type=content_type, update_email_template_request=update_email_template_request)
        print("The response of DefaultApi->update_email_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_email_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **update_email_template_request** | [**UpdateEmailTemplateRequest**](UpdateEmailTemplateRequest.md)|  | [optional] 

### Return type

[**UpdateEmailTemplate**](UpdateEmailTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_fax_delivery_receipt_rule**
> UpdateFaxDeliveryReceiptRule update_fax_delivery_receipt_rule(receipt_rule_id, content_type=content_type, update_fax_delivery_receipt_rule_request=update_fax_delivery_receipt_rule_request)

Update FAX Delivery Receipt Rule

_Update fax delivery receipt automation_

Update fax delivery receipt automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| receipt_rule_id | path | integer(int32) | true | Receipt rule id |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| rule_name | string | true | none | Rule Name. |
| match_type | number | true | none | Match Type. 0=All reports. |
| action | string | true | none | Action to be taken (AUTO_REPLY, EMAIL_USER, EMAIL_FIXED, URL, SMS, POLL, GROUP_SMS, MOVE_CONTACT, CREATE_CONTACT, CREATE_CONTACT_PLUS_EMAIL, CREATE_CONTACT_PLUS_NAME_EMAIL CREATE_CONTACT_PLUS_NAME, SMPP, NONE). |
| action_address | string | true | none | Action address. |
| enabled | number | true | none | Enabled: Disabled=0 or Enabled=1. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.update_fax_delivery_receipt_rule import UpdateFaxDeliveryReceiptRule
from clicksend.models.update_fax_delivery_receipt_rule_request import UpdateFaxDeliveryReceiptRuleRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    update_fax_delivery_receipt_rule_request = clicksend.UpdateFaxDeliveryReceiptRuleRequest() # UpdateFaxDeliveryReceiptRuleRequest |  (optional)

    try:
        # Update FAX Delivery Receipt Rule
        api_response = api_instance.update_fax_delivery_receipt_rule(receipt_rule_id, content_type=content_type, update_fax_delivery_receipt_rule_request=update_fax_delivery_receipt_rule_request)
        print("The response of DefaultApi->update_fax_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_fax_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **update_fax_delivery_receipt_rule_request** | [**UpdateFaxDeliveryReceiptRuleRequest**](UpdateFaxDeliveryReceiptRuleRequest.md)|  | [optional] 

### Return type

[**UpdateFaxDeliveryReceiptRule**](UpdateFaxDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_fax_inbound_rule**
> UpdateFaxInboundRule update_fax_inbound_rule(inbound_rule_id, content_type=content_type, create_fax_inbound_rule_request=create_fax_inbound_rule_request)

Update Fax Inbound Rule

_Update inbound fax automation_

Update inbound fax automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| inbound_rule_id | path | integer(int32) | true | Inbound rule id |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| dedicated_number | string | true | none | Dedicated Number. Can be '\*' to apply to all numbers. |
| rule_name | string | true | none | Rule Name. |
| action | string | true | none | Action to be taken (AUTO_REPLY, EMAIL_USER, EMAIL_FIXED, URL, SMS, POLL, GROUP_SMS, MOVE_CONTACT, CREATE_CONTACT, CREATE_CONTACT_PLUS_EMAIL, CREATE_CONTACT_PLUS_NAME_EMAIL CREATE_CONTACT_PLUS_NAME, SMPP, NONE). |
| action_address | string | true | none | Action address. |
| enabled | number | true | none | Enabled: Disabled=0 or Enabled=1. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_fax_inbound_rule_request import CreateFaxInboundRuleRequest
from clicksend.models.update_fax_inbound_rule import UpdateFaxInboundRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    inbound_rule_id = 'inbound_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    create_fax_inbound_rule_request = clicksend.CreateFaxInboundRuleRequest() # CreateFaxInboundRuleRequest |  (optional)

    try:
        # Update Fax Inbound Rule
        api_response = api_instance.update_fax_inbound_rule(inbound_rule_id, content_type=content_type, create_fax_inbound_rule_request=create_fax_inbound_rule_request)
        print("The response of DefaultApi->update_fax_inbound_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_fax_inbound_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inbound_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **create_fax_inbound_rule_request** | [**CreateFaxInboundRuleRequest**](CreateFaxInboundRuleRequest.md)|  | [optional] 

### Return type

[**UpdateFaxInboundRule**](UpdateFaxInboundRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_list**
> UpdateList update_list(list_id, content_type=content_type, create_list_request=create_list_request)

Update List

_Update specific contact list_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | Your list id |
| list_name | body | string | true | Your new list name |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_list_request import CreateListRequest
from clicksend.models.update_list import UpdateList
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    list_id = 'list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    create_list_request = clicksend.CreateListRequest() # CreateListRequest |  (optional)

    try:
        # Update List
        api_response = api_instance.update_list(list_id, content_type=content_type, create_list_request=create_list_request)
        print("The response of DefaultApi->update_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **create_list_request** | [**CreateListRequest**](CreateListRequest.md)|  | [optional] 

### Return type

[**UpdateList**](UpdateList.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_mms_campaign**
> UpdateMmsCampaign update_mms_campaign(mms_campaign_id, content_type=content_type, calculate_sms_campaign_price_request=calculate_sms_campaign_price_request)

Update MMS Campaign

_Update mms campaign_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| mms_campaign_id | path | integer(int32) | true | ID of MMS campaign to update |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| list_id | integer(int32) | true | none | Your list id. |
| name | string | true | none | Your campaign name. |
| body | string | true | none | Your campaign message. |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id |
| schedule | integer(int32) | false | none | Your schedule timestamp. |
| subject | string | true | none | Subject of MMS campaign. |
| media_file | string | true | none | URL pointing to media file. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_sms_campaign_price_request import CalculateSmsCampaignPriceRequest
from clicksend.models.update_mms_campaign import UpdateMmsCampaign
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    mms_campaign_id = 'mms_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    calculate_sms_campaign_price_request = clicksend.CalculateSmsCampaignPriceRequest() # CalculateSmsCampaignPriceRequest |  (optional)

    try:
        # Update MMS Campaign
        api_response = api_instance.update_mms_campaign(mms_campaign_id, content_type=content_type, calculate_sms_campaign_price_request=calculate_sms_campaign_price_request)
        print("The response of DefaultApi->update_mms_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_mms_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mms_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **calculate_sms_campaign_price_request** | [**CalculateSmsCampaignPriceRequest**](CalculateSmsCampaignPriceRequest.md)|  | [optional] 

### Return type

[**UpdateMmsCampaign**](UpdateMmsCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_own_number**
> OwnNumber update_own_number(own_number_id)

Update Own Number

_Update details of a specific own numbers._

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| own_number_id | path | uuid | true | ID of the own number |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| label | string | false | none | Custom label for phone number. Length must be between 1 - 200 characters. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)

### Example


```python
import clicksend
from clicksend.models.own_number import OwnNumber
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)


# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    own_number_id = 'own_number_id_example' # str | 

    try:
        # Update Own Number
        api_response = api_instance.update_own_number(own_number_id)
        print("The response of DefaultApi->update_own_number:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_own_number: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **own_number_id** | **str**|  | 

### Return type

[**OwnNumber**](OwnNumber.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_payment_info**
> UpdatePaymentInfo update_payment_info(content_type=content_type, update_payment_info_request=update_payment_info_request)

Update Payment Info

_Update credit card info_

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| number | string | true | none | Credit card number |
| expiry_month | integer(int32) | true | none | Expiry month of credit card |
| expiry_year | integer(int32) | true | none | Expiry year of credit card |
| cvc | integer(int32) | true | none | CVC number of credit card |
| name | string | true | none | Name printed on credit card |
| bank_name | string | true | none | Name of bank that credit card belongs to |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.update_payment_info import UpdatePaymentInfo
from clicksend.models.update_payment_info_request import UpdatePaymentInfoRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/x-www-form-urlencoded' # str |  (optional)
    update_payment_info_request = clicksend.UpdatePaymentInfoRequest() # UpdatePaymentInfoRequest |  (optional)

    try:
        # Update Payment Info
        api_response = api_instance.update_payment_info(content_type=content_type, update_payment_info_request=update_payment_info_request)
        print("The response of DefaultApi->update_payment_info:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_payment_info: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **update_payment_info_request** | [**UpdatePaymentInfoRequest**](UpdatePaymentInfoRequest.md)|  | [optional] 

### Return type

[**UpdatePaymentInfo**](UpdatePaymentInfo.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_return_address**
> UpdateReturnAddress update_return_address(return_address_id, content_type=content_type, update_return_address_request=update_return_address_request)

Update Return Address

_Update post return address_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| return_address_id | path | integer(int32) | true | Return address ID |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| address_name | string | true | none | Your address name. |
| address_line_1 | string | true | none | Your address line 1 |
| address_city | string | true | none | Your city |
| address_postal_code | string | true | none | Your postal code |
| address_country | string | true | none | Your country |
| address_line_2 | string | false | none | Your address line 2 |
| address_state | string | false | none | Your state |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.update_return_address import UpdateReturnAddress
from clicksend.models.update_return_address_request import UpdateReturnAddressRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    return_address_id = 'return_address_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    update_return_address_request = clicksend.UpdateReturnAddressRequest() # UpdateReturnAddressRequest |  (optional)

    try:
        # Update Return Address
        api_response = api_instance.update_return_address(return_address_id, content_type=content_type, update_return_address_request=update_return_address_request)
        print("The response of DefaultApi->update_return_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_return_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **return_address_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **update_return_address_request** | [**UpdateReturnAddressRequest**](UpdateReturnAddressRequest.md)|  | [optional] 

### Return type

[**UpdateReturnAddress**](UpdateReturnAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_sms_campaign**
> UpdateSmsCampaign update_sms_campaign(sms_campaign_id, content_type=content_type, calculate_sms_campaign_price_request=calculate_sms_campaign_price_request)

Update SMS Campaign

_Update sms campaign_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| sms_campaign_id | path | integer(int32) | true | ID of SMS campaign to update |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| list_id | integer(int32) | true | none | Your list id. |
| name | string | true | none | Your campaign name. |
| body | string | true | none | Your campaign message. |
| from | string | true | [yes](http://help.clicksend.com/SMS/what-is-a-sender-id-or-sender-number) | Your sender id |
| schedule | integer(int32) | false | none | Your schedule timestamp. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.calculate_sms_campaign_price_request import CalculateSmsCampaignPriceRequest
from clicksend.models.update_sms_campaign import UpdateSmsCampaign
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    sms_campaign_id = 'sms_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    calculate_sms_campaign_price_request = clicksend.CalculateSmsCampaignPriceRequest() # CalculateSmsCampaignPriceRequest |  (optional)

    try:
        # Update SMS Campaign
        api_response = api_instance.update_sms_campaign(sms_campaign_id, content_type=content_type, calculate_sms_campaign_price_request=calculate_sms_campaign_price_request)
        print("The response of DefaultApi->update_sms_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_sms_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sms_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **calculate_sms_campaign_price_request** | [**CalculateSmsCampaignPriceRequest**](CalculateSmsCampaignPriceRequest.md)|  | [optional] 

### Return type

[**UpdateSmsCampaign**](UpdateSmsCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_sms_delivery_receipt_rule**
> UpdateSmsDeliveryReceiptRule update_sms_delivery_receipt_rule(receipt_rule_id, content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)

Update SMS Delivery Receipt Rule

_Update sms delivery receipt automation_

Update sms delivery receipt automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| receipt_rule_id | path | integer(int32) | true | Receipt rule id |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| rule_name | string | true | none | Rule Name. |
| match_type | number | true | none | Match Type. 0=All reports. |
| action | string | true | none | Action to be taken (AUTO_REPLY, EMAIL_USER, EMAIL_FIXED, URL, SMS, POLL, GROUP_SMS, MOVE_CONTACT, CREATE_CONTACT, CREATE_CONTACT_PLUS_EMAIL, CREATE_CONTACT_PLUS_NAME_EMAIL CREATE_CONTACT_PLUS_NAME, SMPP, NONE). |
| action_address | string | true | none | Action address. |
| enabled | number | true | none | Enabled: Disabled=0 or Enabled=1. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_sms_delivery_receipt_rule_request import CreateSmsDeliveryReceiptRuleRequest
from clicksend.models.update_sms_delivery_receipt_rule import UpdateSmsDeliveryReceiptRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    create_sms_delivery_receipt_rule_request = clicksend.CreateSmsDeliveryReceiptRuleRequest() # CreateSmsDeliveryReceiptRuleRequest |  (optional)

    try:
        # Update SMS Delivery Receipt Rule
        api_response = api_instance.update_sms_delivery_receipt_rule(receipt_rule_id, content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)
        print("The response of DefaultApi->update_sms_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_sms_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **create_sms_delivery_receipt_rule_request** | [**CreateSmsDeliveryReceiptRuleRequest**](CreateSmsDeliveryReceiptRuleRequest.md)|  | [optional] 

### Return type

[**UpdateSmsDeliveryReceiptRule**](UpdateSmsDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_sms_inbound_automation**
> UpdateSmsInboundAutomation update_sms_inbound_automation(inbound_rule_id, content_type=content_type, update_sms_inbound_automation_request=update_sms_inbound_automation_request)

Update SMS Inbound Automation

_Update inbound sms automation_

Update inbound sms automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| inbound_rule_id | path | integer(int32) | true | Inbound rule id |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| dedicated_number | string | true | none | Dedicated Number. Can be '\*' to apply to all numbers. |
| rule_name | string | true | none | Rule Name. |
| message_search_type | number | true | none | Message Search Type: 0=Any message, 1=starts with, 2=contains, 3=does not contain. |
| message_search_term | string | true | none | Message search term. |
| action | string | true | none | Action to be taken (AUTO_REPLY, EMAIL_USER, EMAIL_FIXED, URL, SMS, POLL, GROUP_SMS, MOVE_CONTACT, CREATE_CONTACT, CREATE_CONTACT_PLUS_EMAIL, CREATE_CONTACT_PLUS_NAME_EMAIL CREATE_CONTACT_PLUS_NAME, SMPP, NONE). |
| action_address | string | true | none | Action address. |
| enabled | number | true | none | Enabled: Disabled=0 or Enabled=1. |
| webhook_type | string | false | Required when action = URL only | Set as post, get, or json to change the format of the request sent. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.update_sms_inbound_automation import UpdateSmsInboundAutomation
from clicksend.models.update_sms_inbound_automation_request import UpdateSmsInboundAutomationRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    inbound_rule_id = 'inbound_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    update_sms_inbound_automation_request = clicksend.UpdateSmsInboundAutomationRequest() # UpdateSmsInboundAutomationRequest |  (optional)

    try:
        # Update SMS Inbound Automation
        api_response = api_instance.update_sms_inbound_automation(inbound_rule_id, content_type=content_type, update_sms_inbound_automation_request=update_sms_inbound_automation_request)
        print("The response of DefaultApi->update_sms_inbound_automation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_sms_inbound_automation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inbound_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **update_sms_inbound_automation_request** | [**UpdateSmsInboundAutomationRequest**](UpdateSmsInboundAutomationRequest.md)|  | [optional] 

### Return type

[**UpdateSmsInboundAutomation**](UpdateSmsInboundAutomation.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_sms_template**
> UpdateSmsTemplate update_sms_template(template_id, content_type=content_type, create_sms_template_request=create_sms_template_request)

Update SMS Template

Use this endpoint to update a <a href="https://help.clicksend.com/article/9z9uloaz8y-sms-templates-for-different-industries" target="_blank">SMS template</a>.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_sms_template_request import CreateSmsTemplateRequest
from clicksend.models.update_sms_template import UpdateSmsTemplate
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    template_id = 'template_id_example' # str | The ID of the template to update.
    content_type = 'application/json' # str |  (optional)
    create_sms_template_request = clicksend.CreateSmsTemplateRequest() # CreateSmsTemplateRequest |  (optional)

    try:
        # Update SMS Template
        api_response = api_instance.update_sms_template(template_id, content_type=content_type, create_sms_template_request=create_sms_template_request)
        print("The response of DefaultApi->update_sms_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_sms_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**| The ID of the template to update. | 
 **content_type** | **str**|  | [optional] 
 **create_sms_template_request** | [**CreateSmsTemplateRequest**](CreateSmsTemplateRequest.md)|  | [optional] 

### Return type

[**UpdateSmsTemplate**](UpdateSmsTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_stripped_string_rule**
> UpdateStrippedStringRule update_stripped_string_rule(rule_id, content_type=content_type, create_stripped_string_rule_request=create_stripped_string_rule_request)

Update Stripped String Rule

_Update email to sms stripped string rule_

Update email to sms stripped string rule

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| rule_id | path | integer(int32) | true | Your rule id |
| stripped-string | body | string | true | String to be stripped. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_stripped_string_rule_request import CreateStrippedStringRuleRequest
from clicksend.models.update_stripped_string_rule import UpdateStrippedStringRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    rule_id = 'rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    create_stripped_string_rule_request = clicksend.CreateStrippedStringRuleRequest() # CreateStrippedStringRuleRequest |  (optional)

    try:
        # Update Stripped String Rule
        api_response = api_instance.update_stripped_string_rule(rule_id, content_type=content_type, create_stripped_string_rule_request=create_stripped_string_rule_request)
        print("The response of DefaultApi->update_stripped_string_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_stripped_string_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **create_stripped_string_rule_request** | [**CreateStrippedStringRuleRequest**](CreateStrippedStringRuleRequest.md)|  | [optional] 

### Return type

[**UpdateStrippedStringRule**](UpdateStrippedStringRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_subaccount**
> UpdateSubaccount update_subaccount(subaccount_id, content_type=content_type, update_subaccount_request=update_subaccount_request)

Update Subaccount

_Update subaccount_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| subaccount_id | path | integer(int32) | true | ID of subaccount to update |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| api_username | string | true | none | Your new api username. |
| password | string | true | none | Your new password |
| email | string | true | none | Your new email. |
| phone_number | string | true | none | Your phone number in [E.164](https://en.wikipedia.org/wiki/E.164) format. |
| first_name | string | true | none | Your firstname |
| last_name | string | true | none | Your lastname |
| access_users | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |
| access_billing | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |
| access_reporting | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |
| access_contacts | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |
| access_settings | integer(int1) | false | none | Flag value must be 1 for yes or 0 for no. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.update_subaccount import UpdateSubaccount
from clicksend.models.update_subaccount_request import UpdateSubaccountRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    subaccount_id = 'subaccount_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    update_subaccount_request = clicksend.UpdateSubaccountRequest() # UpdateSubaccountRequest |  (optional)

    try:
        # Update Subaccount
        api_response = api_instance.update_subaccount(subaccount_id, content_type=content_type, update_subaccount_request=update_subaccount_request)
        print("The response of DefaultApi->update_subaccount:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_subaccount: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subaccount_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **update_subaccount_request** | [**UpdateSubaccountRequest**](UpdateSubaccountRequest.md)|  | [optional] 

### Return type

[**UpdateSubaccount**](UpdateSubaccount.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_voice_delivery_receipt_rule**
> UpdateVoiceDeliveryReceiptRule update_voice_delivery_receipt_rule(receipt_rule_id, content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)

Update Voice Delivery Receipt Rule

_Update voice delivery receipt automation_

Update voice delivery receipt automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| receipt_rule_id | path | integer(int32) | true | Receipt rule id |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| rule_name | string | true | none | Rule Name. |
| match_type | number | true | none | Match Type. 0=All reports. |
| action | string | true | none | Action to be taken (AUTO_REPLY, EMAIL_USER, EMAIL_FIXED, URL, SMS, POLL, GROUP_SMS, MOVE_CONTACT, CREATE_CONTACT, CREATE_CONTACT_PLUS_EMAIL, CREATE_CONTACT_PLUS_NAME_EMAIL CREATE_CONTACT_PLUS_NAME, SMPP, NONE). |
| action_address | string | true | none | Action address. |
| enabled | number | true | none | Enabled: Disabled=0 or Enabled=1. |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.create_sms_delivery_receipt_rule_request import CreateSmsDeliveryReceiptRuleRequest
from clicksend.models.update_voice_delivery_receipt_rule import UpdateVoiceDeliveryReceiptRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    create_sms_delivery_receipt_rule_request = clicksend.CreateSmsDeliveryReceiptRuleRequest() # CreateSmsDeliveryReceiptRuleRequest |  (optional)

    try:
        # Update Voice Delivery Receipt Rule
        api_response = api_instance.update_voice_delivery_receipt_rule(receipt_rule_id, content_type=content_type, create_sms_delivery_receipt_rule_request=create_sms_delivery_receipt_rule_request)
        print("The response of DefaultApi->update_voice_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->update_voice_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **create_sms_delivery_receipt_rule_request** | [**CreateSmsDeliveryReceiptRuleRequest**](CreateSmsDeliveryReceiptRuleRequest.md)|  | [optional] 

### Return type

[**UpdateVoiceDeliveryReceiptRule**](UpdateVoiceDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **upload_a_media_file**
> upload_a_media_file(content_type=content_type, body=body)

Upload Media File

The `upload` endpoint provides a method for converting files from an unsupported format to a format that one of our endpoints can handle.

Files can be submitted two ways: 1. Using `base64` encoding in an `application/json` request. In this case, submit the `base64`\-encoded file contents in the `content` field of the request body, and `convert` can be specified either also in the body or as part of the query string. 2. Using `multipart/form-data` encoding, in the same way it would be submitted using a HTML form. You may find cURL useful for this. For an example of how to do this, see one of our [SDKs](https://dashboard.clicksend.com/#/libraries-sdk/main). In this case, specify `convert` in the query string.

Note that `convert` specifies the conversion to take place. That is, what the result should be compatible with and can be any of the following:

- `fax`
- `mms`
- `csv`
- `post`
- `postcard`
    

All files will expire 10 minutes after being uploaded.

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| convert | query | string | true | none |
| content | body | string | true | Base64-encoded file contents |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    body = None # object |  (optional)

    try:
        # Upload Media File
        api_instance.upload_a_media_file(content_type=content_type, body=body)
    except Exception as e:
        print("Exception when calling DefaultApi->upload_a_media_file: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **body** | **object**|  | [optional] 

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **verify_allowed_email_address**
> VerifyAllowedEmailAddress verify_allowed_email_address(email_address_id, activation_token, content_type=content_type, verify_allowed_email_address_request=verify_allowed_email_address_request)

Verify Allowed Email Address

_Verify email address using verification token_

Verify email address using verification token

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| email_address_id | path | integer(int32) | true | Allowed email address id |
| activation_token | path | string | true | Your activation token. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.verify_allowed_email_address import VerifyAllowedEmailAddress
from clicksend.models.verify_allowed_email_address_request import VerifyAllowedEmailAddressRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    email_address_id = 'email_address_id_example' # str | 
    activation_token = 'activation_token_example' # str | 
    content_type = 'application/json' # str |  (optional)
    verify_allowed_email_address_request = clicksend.VerifyAllowedEmailAddressRequest() # VerifyAllowedEmailAddressRequest |  (optional)

    try:
        # Verify Allowed Email Address
        api_response = api_instance.verify_allowed_email_address(email_address_id, activation_token, content_type=content_type, verify_allowed_email_address_request=verify_allowed_email_address_request)
        print("The response of DefaultApi->verify_allowed_email_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->verify_allowed_email_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_address_id** | **str**|  | 
 **activation_token** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **verify_allowed_email_address_request** | [**VerifyAllowedEmailAddressRequest**](VerifyAllowedEmailAddressRequest.md)|  | [optional] 

### Return type

[**VerifyAllowedEmailAddress**](VerifyAllowedEmailAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **verify_own_number_otp**
> VerifyOwnNumberOtp verify_own_number_otp(verification_id, content_type=content_type, verify_own_number_otp_request=verify_own_number_otp_request)

Verify Own Number OTP

_Request to verify an OTP for Own Number verification_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| verification_id | path | uuid | true | ID of the Own Number verification |

### Properties

| Name | Type | Required | Restrictions | Description |
| --- | --- | --- | --- | --- |
| code | string | true | none | OTP code. Length must be 6 characters |
| phone_number | string | true | none | Phone number. |
| country | string | false | none | Country code. |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.verify_own_number_otp import VerifyOwnNumberOtp
from clicksend.models.verify_own_number_otp_request import VerifyOwnNumberOtpRequest
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    verification_id = 'verification_id_example' # str | 
    content_type = 'application/json' # str |  (optional)
    verify_own_number_otp_request = clicksend.VerifyOwnNumberOtpRequest() # VerifyOwnNumberOtpRequest |  (optional)

    try:
        # Verify Own Number OTP
        api_response = api_instance.verify_own_number_otp(verification_id, content_type=content_type, verify_own_number_otp_request=verify_own_number_otp_request)
        print("The response of DefaultApi->verify_own_number_otp:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->verify_own_number_otp: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **verification_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 
 **verify_own_number_otp_request** | [**VerifyOwnNumberOtpRequest**](VerifyOwnNumberOtpRequest.md)|  | [optional] 

### Return type

[**VerifyOwnNumberOtp**](VerifyOwnNumberOtp.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_a_specific_inbound_sms_message**
> ViewASpecificInboundSmsMessage view_a_specific_inbound_sms_message(original_message_id, content_type=content_type)

View a specific inbound SMS message

Use this endpoint to retrieve a specific inbound SMS, including those that have been marked as read. 
Inbound SMS are messages sent by your recipient to you. This endpoint enables you to retrieve those inbound SMS.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_a_specific_inbound_sms_message import ViewASpecificInboundSmsMessage
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    original_message_id = 'original_message_id_example' # str | The _original_message_id_ of the inbound SMS to view. If the recipient replied with multiple messages, this endpoint returns the first inbound SMS received.  <div class=\"info-box\">   <h4><i class=\"fas fa-info-circle\"></i> Note:</h4>   <p>     When you receive an inbound message, you will get two parameters: <em>original_message_id</em> and <em>message_id</em>:   </p>   <ul>     <li><em>original_message_id</em>: This is the ID of the outbound message sent to the recipient</li>     <li><em>message_id</em>: This is the ID of the inbound message sent by the recipient.</li>   </ul> </div>
    content_type = 'application/json' # str |  (optional)

    try:
        # View a specific inbound SMS message
        api_response = api_instance.view_a_specific_inbound_sms_message(original_message_id, content_type=content_type)
        print("The response of DefaultApi->view_a_specific_inbound_sms_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_a_specific_inbound_sms_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **original_message_id** | **str**| The _original_message_id_ of the inbound SMS to view. If the recipient replied with multiple messages, this endpoint returns the first inbound SMS received.  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;     When you receive an inbound message, you will get two parameters: &lt;em&gt;original_message_id&lt;/em&gt; and &lt;em&gt;message_id&lt;/em&gt;:   &lt;/p&gt;   &lt;ul&gt;     &lt;li&gt;&lt;em&gt;original_message_id&lt;/em&gt;: This is the ID of the outbound message sent to the recipient&lt;/li&gt;     &lt;li&gt;&lt;em&gt;message_id&lt;/em&gt;: This is the ID of the inbound message sent by the recipient.&lt;/li&gt;   &lt;/ul&gt; &lt;/div&gt; | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewASpecificInboundSmsMessage**](ViewASpecificInboundSmsMessage.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_a_specific_sms_template**
> ViewASpecificSmsTemplate view_a_specific_sms_template(template_id, content_type=content_type)

View a Specific SMS Template

Use this endpoint to retrieve a <a href="https://help.clicksend.com/article/9z9uloaz8y-sms-templates-for-different-industries" target="_blank">SMS template</a>. Specify which template to retrieve using the template ID.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_a_specific_sms_template import ViewASpecificSmsTemplate
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    template_id = 'template_id_example' # str | The ID of the template to retrieve
    content_type = 'application/json' # str |  (optional)

    try:
        # View a Specific SMS Template
        api_response = api_instance.view_a_specific_sms_template(template_id, content_type=content_type)
        print("The response of DefaultApi->view_a_specific_sms_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_a_specific_sms_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**| The ID of the template to retrieve | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewASpecificSmsTemplate**](ViewASpecificSmsTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_account_details**
> ViewAccountDetails view_account_details(content_type=content_type)

View Account Details

_Get account information_

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/#pagination" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_account_details import ViewAccountDetails
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Account Details
        api_response = api_instance.view_account_details(content_type=content_type)
        print("The response of DefaultApi->view_account_details:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_account_details: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAccountDetails**](ViewAccountDetails.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_account_usage**
> ViewAccountUsage view_account_usage(year, month, content_type=content_type)

View Account Usage

_Get account usage_

| **Name** | **Type** | **Required** | **Restrictions** | **Description** |
| --- | --- | --- | --- | --- |
| year | string | true | none | Your account usage year. Example: 2019 |
| month | string | true | none | Your account usage month. Example: 4 |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/#pagination" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_account_usage import ViewAccountUsage
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    year = 'year_example' # str | 
    month = 'month_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Account Usage
        api_response = api_instance.view_account_usage(year, month, content_type=content_type)
        print("The response of DefaultApi->view_account_usage:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_account_usage: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **str**|  | 
 **month** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAccountUsage**](ViewAccountUsage.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_all_email_campaigns**
> ViewAllEmailCampaigns view_all_email_campaigns(content_type=content_type)

View All Email Campaigns

_Get all email campaigns_

Get all email campaigns

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | Page number |
| limit | query | integer(int32) | false | Number of records per page |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_all_email_campaigns import ViewAllEmailCampaigns
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View All Email Campaigns
        api_response = api_instance.view_all_email_campaigns(content_type=content_type)
        print("The response of DefaultApi->view_all_email_campaigns:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_all_email_campaigns: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAllEmailCampaigns**](ViewAllEmailCampaigns.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_all_mms_campaigns**
> ViewAllMmsCampaigns view_all_mms_campaigns(content_type=content_type)

View All MMS Campaigns

_Get list of mms campaigns_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_all_mms_campaigns import ViewAllMmsCampaigns
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View All MMS Campaigns
        api_response = api_instance.view_all_mms_campaigns(content_type=content_type)
        print("The response of DefaultApi->view_all_mms_campaigns:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_all_mms_campaigns: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAllMmsCampaigns**](ViewAllMmsCampaigns.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_all_transactions**
> ViewAllTransactions view_all_transactions(content_type=content_type)

View All Transactions

_Purchase a package_

Get all transactions

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_all_transactions import ViewAllTransactions
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View All Transactions
        api_response = api_instance.view_all_transactions(content_type=content_type)
        print("The response of DefaultApi->view_all_transactions:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_all_transactions: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAllTransactions**](ViewAllTransactions.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_allowed_email_address**
> ViewAllowedEmailAddress view_allowed_email_address(email_address_id, content_type=content_type)

View Allowed Email Address

_Get specific email address_

Get specific email address

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| email_address_id | path | integer(int32) | true | Allowed email address id |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_allowed_email_address import ViewAllowedEmailAddress
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    email_address_id = 'email_address_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Allowed Email Address
        api_response = api_instance.view_allowed_email_address(email_address_id, content_type=content_type)
        print("The response of DefaultApi->view_allowed_email_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_allowed_email_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_address_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAllowedEmailAddress**](ViewAllowedEmailAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_allowed_email_addresses**
> ViewAllowedEmailAddresses view_allowed_email_addresses(content_type=content_type)

View Allowed Email Addresses

_Get all email addresses_

Get all email addresses

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | Page number |
| limit | query | integer(int32) | false | Number of records per page |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_allowed_email_addresses import ViewAllowedEmailAddresses
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Allowed Email Addresses
        api_response = api_instance.view_allowed_email_addresses(content_type=content_type)
        print("The response of DefaultApi->view_allowed_email_addresses:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_allowed_email_addresses: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAllowedEmailAddresses**](ViewAllowedEmailAddresses.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_allowed_emails**
> ViewAllowedEmails view_allowed_emails(content_type=content_type)

View Allowed Emails

_Get list of email to sms allowed addresses_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_allowed_emails import ViewAllowedEmails
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Allowed Emails
        api_response = api_instance.view_allowed_emails(content_type=content_type)
        print("The response of DefaultApi->view_allowed_emails:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_allowed_emails: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAllowedEmails**](ViewAllowedEmails.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_available_numbers**
> ViewAvailableNumbers view_available_numbers(country, content_type=content_type)

View Available Numbers

_Get all dedicated numbers by country_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| country | path | string | true | Country code to search |
| search | query | string | false | Your search pattern or query. |
| search_type | query | integer(int32) | false | Your strategy for searching, 0 = starts with, 1 = anywhere, 2 = ends with. |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_available_numbers import ViewAvailableNumbers
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    country = 'country_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Available Numbers
        api_response = api_instance.view_available_numbers(country, content_type=content_type)
        print("The response of DefaultApi->view_available_numbers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_available_numbers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **country** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewAvailableNumbers**](ViewAvailableNumbers.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_client_accounts**
> ViewClientAccounts view_client_accounts(content_type=content_type)

View Client Accounts

_Get list of reseller accounts_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_client_accounts import ViewClientAccounts
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Client Accounts
        api_response = api_instance.view_client_accounts(content_type=content_type)
        print("The response of DefaultApi->view_client_accounts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_client_accounts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewClientAccounts**](ViewClientAccounts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_contact_lists**
> view_contact_lists(q=q)

View Contact Lists

_Get list of searched contact list_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| q | query | string | true | Your keyword or query. |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    q = 'Test' # str |  (optional)

    try:
        # View Contact Lists
        api_instance.view_contact_lists(q=q)
    except Exception as e:
        print("Exception when calling DefaultApi->view_contact_lists: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **str**|  | [optional] 

### Return type

void (empty response body)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_countries**
> ViewCountries view_countries()

View Countries

_Get all country codes_

Get all countries


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #6BBD5B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint does not require authentication</span> 
</div>

### Example


```python
import clicksend
from clicksend.models.view_countries import ViewCountries
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)


# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)

    try:
        # View Countries
        api_response = api_instance.view_countries()
        print("The response of DefaultApi->view_countries:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_countries: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ViewCountries**](ViewCountries.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_email_campaign**
> ViewEmailCampaign view_email_campaign(email_campaign_id, content_type=content_type)

View Email Campaign

_Get specific email campaign_

Get specific email campaign

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_email_campaign import ViewEmailCampaign
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    email_campaign_id = 'email_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Email Campaign
        api_response = api_instance.view_email_campaign(email_campaign_id, content_type=content_type)
        print("The response of DefaultApi->view_email_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_email_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewEmailCampaign**](ViewEmailCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_email_campaign_history**
> ViewEmailCampaignHistory view_email_campaign_history(email_campaign_id, content_type=content_type)

View Email Campaign History

_Get specific email campaign history_

Get specific email campaign history


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_email_campaign_history import ViewEmailCampaignHistory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    email_campaign_id = 'email_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Email Campaign History
        api_response = api_instance.view_email_campaign_history(email_campaign_id, content_type=content_type)
        print("The response of DefaultApi->view_email_campaign_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_email_campaign_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewEmailCampaignHistory**](ViewEmailCampaignHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_email_delivery_receipt_rule**
> ViewEmailDeliveryReceiptRule view_email_delivery_receipt_rule(receipt_rule_id, content_type=content_type)

View Email Delivery Receipt Rule

_Get specific email delivery receipt automation_

Get specific email delivery receipt automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| receipt_rule_id | path | integer(int32) | true | Receipt rule id |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_email_delivery_receipt_rule import ViewEmailDeliveryReceiptRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Email Delivery Receipt Rule
        api_response = api_instance.view_email_delivery_receipt_rule(receipt_rule_id, content_type=content_type)
        print("The response of DefaultApi->view_email_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_email_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewEmailDeliveryReceiptRule**](ViewEmailDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_email_delivery_receipt_rules**
> ViewEmailDeliveryReceiptRules view_email_delivery_receipt_rules(content_type=content_type)

View Email Delivery Receipt Rules

_Get all email delivery receipt automations_

Get all email delivery receipt automations

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | Page number |
| limit | query | integer(int32) | false | Number of records per page |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_email_delivery_receipt_rules import ViewEmailDeliveryReceiptRules
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Email Delivery Receipt Rules
        api_response = api_instance.view_email_delivery_receipt_rules(content_type=content_type)
        print("The response of DefaultApi->view_email_delivery_receipt_rules:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_email_delivery_receipt_rules: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewEmailDeliveryReceiptRules**](ViewEmailDeliveryReceiptRules.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_email_history**
> ViewEmailHistory view_email_history(content_type=content_type)

View Email History

_Get all transactional email history_

Get all transactional email history

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| date_from | query | integer(int32) | false | Start date (Unix Timestamp e.g. 1436849372) |
| date_to | query | integer(int32) | false | End date (Unix Timestamp e.g. 1436879372) |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_email_history import ViewEmailHistory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Email History
        api_response = api_instance.view_email_history(content_type=content_type)
        print("The response of DefaultApi->view_email_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_email_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewEmailHistory**](ViewEmailHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_email_template**
> ViewEmailTemplate view_email_template(template_id, content_type=content_type)

View Email Template

_Get specific user email template_

Get specific user email templates

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| template_id | path | integer(int32) | true | Email template id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_email_template import ViewEmailTemplate
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    template_id = 'template_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Email Template
        api_response = api_instance.view_email_template(template_id, content_type=content_type)
        print("The response of DefaultApi->view_email_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_email_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewEmailTemplate**](ViewEmailTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_email_templates**
> ViewEmailTemplates view_email_templates(content_type=content_type)

View Email Templates

_Get all user email templates_

Get all user email templates

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | Page number |
| limit | query | integer(int32) | false | Number of records per page |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_email_templates import ViewEmailTemplates
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Email Templates
        api_response = api_instance.view_email_templates(content_type=content_type)
        print("The response of DefaultApi->view_email_templates:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_email_templates: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewEmailTemplates**](ViewEmailTemplates.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_fax_delivery_receipt_rule**
> ViewFaxDeliveryReceiptRule view_fax_delivery_receipt_rule(receipt_rule_id, content_type=content_type)

View FAX Delivery Receipt Rule

_Get specific fax delivery receipt automation_

Get specific fax delivery receipt automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| receipt_rule_id | path | integer(int32) | true | Receipt rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_fax_delivery_receipt_rule import ViewFaxDeliveryReceiptRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View FAX Delivery Receipt Rule
        api_response = api_instance.view_fax_delivery_receipt_rule(receipt_rule_id, content_type=content_type)
        print("The response of DefaultApi->view_fax_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_fax_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewFaxDeliveryReceiptRule**](ViewFaxDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_fax_delivery_receipt_rules**
> ViewFaxDeliveryReceiptRules view_fax_delivery_receipt_rules(content_type=content_type)

View FAX Delivery Receipt Rules

_Get all fax delivery receipt automations_

Get all fax delivery receipt automations

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | Page number |
| limit | query | integer(int32) | false | Number of records per page |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_fax_delivery_receipt_rules import ViewFaxDeliveryReceiptRules
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View FAX Delivery Receipt Rules
        api_response = api_instance.view_fax_delivery_receipt_rules(content_type=content_type)
        print("The response of DefaultApi->view_fax_delivery_receipt_rules:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_fax_delivery_receipt_rules: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewFaxDeliveryReceiptRules**](ViewFaxDeliveryReceiptRules.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_fax_history**
> ViewFaxHistory view_fax_history(content_type=content_type)

View Fax History

_Get a list of Fax History._

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| date_from | query | integer(int32) | false | Start date (Unix Timestamp e.g. 1436849372) |
| date_to | query | integer(int32) | false | End date (Unix Timestamp e.g. 1436879372) |
| q | query | string | false | Custom query Example: status:Sent,status_code:201. |
| order | query | string | false | Order result by Example: date_added:desc,list_id:desc. |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

This endpoint requires authentication, [more info...](/#authentication)


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_fax_history import ViewFaxHistory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Fax History
        api_response = api_instance.view_fax_history(content_type=content_type)
        print("The response of DefaultApi->view_fax_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_fax_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewFaxHistory**](ViewFaxHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_fax_inbound_rule**
> ViewFaxInboundRule view_fax_inbound_rule(inbound_rule_id, content_type=content_type)

View Fax Inbound Rule

_Get specific inbound fax automation_

Get specific inbound fax automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| inbound_rule_id | path | integer(int32) | true | Inbound rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_fax_inbound_rule import ViewFaxInboundRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    inbound_rule_id = 'inbound_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Fax Inbound Rule
        api_response = api_instance.view_fax_inbound_rule(inbound_rule_id, content_type=content_type)
        print("The response of DefaultApi->view_fax_inbound_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_fax_inbound_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inbound_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewFaxInboundRule**](ViewFaxInboundRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_fax_inbound_rules**
> ViewFaxInboundRules view_fax_inbound_rules(content_type=content_type)

View Fax Inbound Rules

_Get all inbound fax automations_

Get all inbound fax automations

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | Page number |
| limit | query | integer(int32) | false | Number of records per page |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_fax_inbound_rules import ViewFaxInboundRules
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Fax Inbound Rules
        api_response = api_instance.view_fax_inbound_rules(content_type=content_type)
        print("The response of DefaultApi->view_fax_inbound_rules:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_fax_inbound_rules: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewFaxInboundRules**](ViewFaxInboundRules.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_fax_receipts**
> ViewFaxReceipts view_fax_receipts(content_type=content_type)

View Fax Receipts

_Get List of Fax Receipts_

**Push Delivery Receipts**

If you prefer, we can push message replies to your server as they arrive with us.

1. Log into your account.
2. Click on your profile on the top right.
3. Then click on the Messaging Settings option.
4. Click on Fax then Delivery Reports.
5. Click the 'Add New Rule' button.
6. Select the 'URL' action.
7. Enter the URL and click 'Save'.
    

The following variables will be posted to the URL specified:

| Variable | Description |
| --- | --- |
| `timestamp_send` | Timestamp of the original send request in UNIX format. e.g 1439173980 |
| `timestamp` | Timestamp of delivery report in UNIX format. e.g 1439173981 |
| `message_id` | Message ID, returned when originally sending the message. |
| `status` | Delivered or Undelivered |
| `status_code` | Status code. Refer to 'Fax Delivery Status Codes' in docs. |
| `status_text` | Status text. |
| `error_code` | Error code. |
| `error_text` | Error text. |
| `custom_string` | A custom string used when sending the original message. |
| `user_id` | The user ID of the user who sent the message. |
| `subaccount_id` | The subaccount ID of the user who sent the message. |
| `message_type` | 'fax' (constant). |

**Pull Delivery Receipts**

Receive delivery reports by polling. You can poll our server and retrieve delivery reports at a time that suits you.

1. Log into your account.
2. Click on your profile on the top right.
3. Then click on the Messaging Settings option.
4. Click on Fax then Delivery Rules.
5. Click the 'Add New Rule' button.
6. Select the 'Poll' action.
7. Then click 'Save'.
    

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_fax_receipts import ViewFaxReceipts
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Fax Receipts
        api_response = api_instance.view_fax_receipts(content_type=content_type)
        print("The response of DefaultApi->view_fax_receipts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_fax_receipts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewFaxReceipts**](ViewFaxReceipts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_inbound_sms**
> ViewInboundSms view_inbound_sms(content_type=content_type, page=page, limit=limit)

View Inbound SMS

Use this endpoint to retrieve <a href="https://help.clicksend.com/article/49eq1qdcui-how-do-i-receive-sms-delivery-receipts-delivery-status-updates" target="_blank">SMS delivery receipts</a> sent by your recipient. 
To be able to view receipts, add a <a href="https://help.clicksend.com/article/ut4ttdrrai-incoming-reply-sms-options">inbound rule</a> with the Action set to **POLL** in the Dashboard, or use the [**Create SMS Inbound Automation**](/automations/sms/other/create-sms-inbound-automation) endpoint. 
Control [pagination](/#pagination) with the _page_ and _limit_ query parameters to specify the page of results and the number of items returned.

<div class="info-box">
  <h4><i class="fas fa-info-circle"></i> Note:</h4>
  <p>If you have multiple inbound rules set to <strong>POLL</strong>, you will receive the inbound message multiple times.</p>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_inbound_sms import ViewInboundSms
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    page = 1 # int | The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. (optional) (default to 1)
    limit = 15 # int | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. (optional) (default to 15)

    try:
        # View Inbound SMS
        api_response = api_instance.view_inbound_sms(content_type=content_type, page=page, limit=limit)
        print("The response of DefaultApi->view_inbound_sms:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_inbound_sms: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **page** | **int**| The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. | [optional] [default to 1]
 **limit** | **int**| The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. | [optional] [default to 15]

### Return type

[**ViewInboundSms**](ViewInboundSms.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_letter_history**
> ViewLetterHistory view_letter_history(content_type=content_type)

View Letter History

_Get all letter history_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_letter_history import ViewLetterHistory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Letter History
        api_response = api_instance.view_letter_history(content_type=content_type)
        print("The response of DefaultApi->view_letter_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_letter_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewLetterHistory**](ViewLetterHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_list_contacts**
> ViewListContacts view_list_contacts(list_id, content_type=content_type)

View List Contacts

_Get all contacts in a list_

### parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | Contact list ID |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |
| updated_after | query | integer(int32) | false | Get all contacts updated after a given timestamp. |


Refer to [Status
Codes](/#status-codes) for
definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_list_contacts import ViewListContacts
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    list_id = 'list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View List Contacts
        api_response = api_instance.view_list_contacts(list_id, content_type=content_type)
        print("The response of DefaultApi->view_list_contacts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_list_contacts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewListContacts**](ViewListContacts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_lists**
> ViewLists view_lists(content_type=content_type)

View Lists

_Get all contact lists_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_lists import ViewLists
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Lists
        api_response = api_instance.view_lists(content_type=content_type)
        print("The response of DefaultApi->view_lists:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_lists: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewLists**](ViewLists.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_master_email_template**
> ViewMasterEmailTemplate view_master_email_template(template_id, content_type=content_type)

View Master Email Template

_Get specific master email template_

Get specific master email template

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| template_id | path | integer(int32) | true | Email template id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_master_email_template import ViewMasterEmailTemplate
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    template_id = 'template_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Master Email Template
        api_response = api_instance.view_master_email_template(template_id, content_type=content_type)
        print("The response of DefaultApi->view_master_email_template:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_master_email_template: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **template_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewMasterEmailTemplate**](ViewMasterEmailTemplate.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_master_email_templates**
> ViewMasterEmailTemplates view_master_email_templates(content_type=content_type)

View Master Email Templates

_Get all master email templates._

Get all master email templates.

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | Page number |
| limit | query | integer(int32) | false | Number of records per page |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_master_email_templates import ViewMasterEmailTemplates
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Master Email Templates
        api_response = api_instance.view_master_email_templates(content_type=content_type)
        print("The response of DefaultApi->view_master_email_templates:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_master_email_templates: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewMasterEmailTemplates**](ViewMasterEmailTemplates.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_mms_campaign**
> ViewMmsCampaign view_mms_campaign(mms_campaign_id, content_type=content_type)

View MMS Campaign

_Get specific mms campaign_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| mms_campaign_id | path | integer(int32) | true | ID of MMS campaign to retrieve |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_mms_campaign import ViewMmsCampaign
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    mms_campaign_id = 'mms_campaign_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View MMS Campaign
        api_response = api_instance.view_mms_campaign(mms_campaign_id, content_type=content_type)
        print("The response of DefaultApi->view_mms_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_mms_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **mms_campaign_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewMmsCampaign**](ViewMmsCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_mms_history**
> ViewMmsHistory view_mms_history(content_type=content_type, limit=limit)

View MMS History

_Get all mms history_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| date_from | query | integer(int32) | false | Start date (Unix Timestamp e.g. 1436849372) |
| date_to | query | integer(int32) | false | End date (Unix Timestamp e.g. 1436879372) |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_mms_history import ViewMmsHistory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    limit = 100 # int |  (optional)

    try:
        # View MMS History
        api_response = api_instance.view_mms_history(content_type=content_type, limit=limit)
        print("The response of DefaultApi->view_mms_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_mms_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **limit** | **int**|  | [optional] 

### Return type

[**ViewMmsHistory**](ViewMmsHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_postcard_history**
> ViewPostcardHistory view_postcard_history(content_type=content_type)

View Postcard History

_Retrieve the history of postcards sent or scheduled_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_postcard_history import ViewPostcardHistory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Postcard History
        api_response = api_instance.view_postcard_history(content_type=content_type)
        print("The response of DefaultApi->view_postcard_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_postcard_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewPostcardHistory**](ViewPostcardHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_recharge_packages**
> ViewRechargePackages view_recharge_packages(content_type=content_type)

View Recharge Packages

_Get list of all packages_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| country | query | string | false | Two-letter country code ([ISO3166](https://en.wikipedia.org/wiki/ISO_3166)) |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_recharge_packages import ViewRechargePackages
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Recharge Packages
        api_response = api_instance.view_recharge_packages(content_type=content_type)
        print("The response of DefaultApi->view_recharge_packages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_recharge_packages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewRechargePackages**](ViewRechargePackages.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_referral_accounts**
> ViewReferralAccounts view_referral_accounts(content_type=content_type)

View Referral Accounts

_Get all referral accounts_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_referral_accounts import ViewReferralAccounts
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Referral Accounts
        api_response = api_instance.view_referral_accounts(content_type=content_type)
        print("The response of DefaultApi->view_referral_accounts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_referral_accounts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewReferralAccounts**](ViewReferralAccounts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_sms_campaigns**
> ViewSmsCampaigns view_sms_campaigns(content_type=content_type, page=page, limit=limit, q=q, order_by=order_by, date_from=date_from, date_to=date_to)

View SMS Campaigns

Use this endpoint to view SMS campaigns.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_sms_campaigns import ViewSmsCampaigns
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    page = 1 # int | The page number to retrieve. Use this parameter to navigate through the [pagination]/#pagination) results. The default value is 1. (optional) (default to 1)
    limit = 15 # int | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. (optional) (default to 15)
    q = 'q_example' # str | Allows filtering of results based on your search criteria. The query should be in the format `field_name:value`.  1. **Field Name**: The field within the SMS campaign you want to filter by. You can use the following fields:      - sms_campaign_id,name,user_id,subaccount_id,list_id,from,body,schedule,status,date_added,custom_string,url_to_shorten,unsubscribe_link,source   2. **Value**: The text or keyword you're searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.  For example, if you are searching for a SMS campaign with the status of _Scheduled_, the final query would look like this:    - `q=status:Scheduled`  <div class=\"info-box\">   <h4><i class=\"fas fa-info-circle\"></i> Note:</h4>   <p>   Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:<br/>    <ul>     <li>q=from:%2B61437085284</li>   </ul>    You can use the <a href=\"https://www.urlencoder.org/\" target=\"_blank\">URL encoder</a> to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.      </p> </div> (optional)
    order_by = 'order_by_example' # str | Specifies the field and order to sort the results by. The value is composed of the field name followed by a colon and the sort direction (_asc_ for ascending or _desc_ for descending).  The default sort order is by _date_added_ in ascending order. You can use the following fields:    - _name_: The name of the SMS campaign.   - _status_: The status of the SMS campaign.   - _schedule_: The schedule send date of the SMS campaign in the <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>.   - _from_: The sender of the SMS campaign.   - _date_added_: This is the date you created or updated the SMS campaign in the <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>.  For example, if you want to order by the most recently sent or scheduled SMS, you should sort by date in descending order. The query would look like this:    - `order_by=schedule:desc`  <div class=\"info-box\">   <h4><i class=\"fas fa-info-circle\"></i> Note:</h4>   <p>     You can also sort by these fields: <br/>     <ul>     <li>sms_campaign_id,user_id,subaccount_id,list_id,body,custom_string,url_to_shorten,unsubscribe_link, and source.</li>   </ul>   <br/>   But this is less common in practice.   </p> </div> (optional)
    date_from = 56 # int | Start date to filter results. It should be in <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>. (optional)
    date_to = 56 # int | End date to filter results. It should be in <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>. (optional)

    try:
        # View SMS Campaigns
        api_response = api_instance.view_sms_campaigns(content_type=content_type, page=page, limit=limit, q=q, order_by=order_by, date_from=date_from, date_to=date_to)
        print("The response of DefaultApi->view_sms_campaigns:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_sms_campaigns: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **page** | **int**| The page number to retrieve. Use this parameter to navigate through the [pagination]/#pagination) results. The default value is 1. | [optional] [default to 1]
 **limit** | **int**| The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. | [optional] [default to 15]
 **q** | **str**| Allows filtering of results based on your search criteria. The query should be in the format &#x60;field_name:value&#x60;.  1. **Field Name**: The field within the SMS campaign you want to filter by. You can use the following fields:      - sms_campaign_id,name,user_id,subaccount_id,list_id,from,body,schedule,status,date_added,custom_string,url_to_shorten,unsubscribe_link,source   2. **Value**: The text or keyword you&#39;re searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.  For example, if you are searching for a SMS campaign with the status of _Scheduled_, the final query would look like this:    - &#x60;q&#x3D;status:Scheduled&#x60;  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;   Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:&lt;br/&gt;    &lt;ul&gt;     &lt;li&gt;q&#x3D;from:%2B61437085284&lt;/li&gt;   &lt;/ul&gt;    You can use the &lt;a href&#x3D;\&quot;https://www.urlencoder.org/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;URL encoder&lt;/a&gt; to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.      &lt;/p&gt; &lt;/div&gt; | [optional] 
 **order_by** | **str**| Specifies the field and order to sort the results by. The value is composed of the field name followed by a colon and the sort direction (_asc_ for ascending or _desc_ for descending).  The default sort order is by _date_added_ in ascending order. You can use the following fields:    - _name_: The name of the SMS campaign.   - _status_: The status of the SMS campaign.   - _schedule_: The schedule send date of the SMS campaign in the &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;.   - _from_: The sender of the SMS campaign.   - _date_added_: This is the date you created or updated the SMS campaign in the &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;.  For example, if you want to order by the most recently sent or scheduled SMS, you should sort by date in descending order. The query would look like this:    - &#x60;order_by&#x3D;schedule:desc&#x60;  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;p&gt;     You can also sort by these fields: &lt;br/&gt;     &lt;ul&gt;     &lt;li&gt;sms_campaign_id,user_id,subaccount_id,list_id,body,custom_string,url_to_shorten,unsubscribe_link, and source.&lt;/li&gt;   &lt;/ul&gt;   &lt;br/&gt;   But this is less common in practice.   &lt;/p&gt; &lt;/div&gt; | [optional] 
 **date_from** | **int**| Start date to filter results. It should be in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
 **date_to** | **int**| End date to filter results. It should be in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 

### Return type

[**ViewSmsCampaigns**](ViewSmsCampaigns.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_sms_delivery_receipt_rule**
> ViewSmsDeliveryReceiptRule view_sms_delivery_receipt_rule(receipt_rule_id, content_type=content_type)

View SMS Delivery Receipt Rule

_Get specific sms delivery receipt automation_

Get specific sms delivery receipt automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| receipt_rule_id | path | integer(int32) | true | Receipt rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_sms_delivery_receipt_rule import ViewSmsDeliveryReceiptRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View SMS Delivery Receipt Rule
        api_response = api_instance.view_sms_delivery_receipt_rule(receipt_rule_id, content_type=content_type)
        print("The response of DefaultApi->view_sms_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_sms_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSmsDeliveryReceiptRule**](ViewSmsDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_sms_delivery_receipt_rules**
> ViewSmsDeliveryReceiptRules view_sms_delivery_receipt_rules(content_type=content_type)

View SMS Delivery Receipt Rules

_Get all sms delivery receipt automations_

Get all sms delivery receipt automations

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | Page number |
| limit | query | integer(int32) | false | Number of records per page |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_sms_delivery_receipt_rules import ViewSmsDeliveryReceiptRules
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View SMS Delivery Receipt Rules
        api_response = api_instance.view_sms_delivery_receipt_rules(content_type=content_type)
        print("The response of DefaultApi->view_sms_delivery_receipt_rules:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_sms_delivery_receipt_rules: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSmsDeliveryReceiptRules**](ViewSmsDeliveryReceiptRules.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_sms_history**
> ViewSmsHistory view_sms_history(content_type=content_type, page=page, limit=limit, q=q, order_by=order_by, date_from=date_from, date_to=date_to)

View SMS History

Use this endpoint to view previously sent SMS. You can filter the SMS history result using the query parameters.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_sms_history import ViewSmsHistory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    page = 1 # int | The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. (optional) (default to 1)
    limit = 15 # int | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. (optional) (default to 15)
    q = 'field_name' # str | Allows filtering of results based on your search criteria. The query should be in the format `field_name:value`.  1. **Field Name**: The field within the SMS history you want to filter by. You can use the following fields:          - _Status_: The status of the SMS. Available values for status are: Queued, Completed, Scheduled, WaitApproval, Failed, Cancelled, CancelledAfterReview, Received, Sent.              - _To_: The recipient of the SMS.              - _from_: The sender of the SMS.              - _subaccount_id_: The sub-account identifier.              - _message_id_: The ID of your SMS.          2. **Value**: The text or keyword you're searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.             For example, if you are searching for a SMS with the status of Scheduled, the final query would look like this:    `q=status:Scheduled`  <div class=\"info-box\">   <h4><i class=\"fas fa-info-circle\"></i> Note:</h4>   <div>    <p>Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:<br/></p>     <ul>       <li>q=from:%2B61437085284</li>     </ul>     <p>You can use the <a href=\"https://www.urlencoder.org/\" target=\"_blank\">URL encoder</a> to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.</p>   </div> </div> (optional) (default to 'field_name')
    order_by = 'date:asc' # str | Specifies the field and order to sort the results by. The value is composed of the field name followed by a colon and the sort direction (_asc_ for ascending or _desc_ for descending).  The default sort order is by _date_ in ascending order. You can use the following fields:    - _date_   - _username_   - _from_    - _to_   - _status_   - _body_  For example, if you want to order by the most recently sent SMS, you should sort by date in descending order. The query would look like this:    `order_by=date:desc` (optional) (default to 'date:asc')
    date_from = 56 # int | Start date to filter results. It should be in <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>. (optional)
    date_to = 56 # int | End date to filter results. It should be in <a href=\"http://help.clicksend.com/what-is-a-unix-timestamp\" target=\"_blank\">Unix format</a>. (optional)

    try:
        # View SMS History
        api_response = api_instance.view_sms_history(content_type=content_type, page=page, limit=limit, q=q, order_by=order_by, date_from=date_from, date_to=date_to)
        print("The response of DefaultApi->view_sms_history:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_sms_history: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **page** | **int**| The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. | [optional] [default to 1]
 **limit** | **int**| The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. | [optional] [default to 15]
 **q** | **str**| Allows filtering of results based on your search criteria. The query should be in the format &#x60;field_name:value&#x60;.  1. **Field Name**: The field within the SMS history you want to filter by. You can use the following fields:          - _Status_: The status of the SMS. Available values for status are: Queued, Completed, Scheduled, WaitApproval, Failed, Cancelled, CancelledAfterReview, Received, Sent.              - _To_: The recipient of the SMS.              - _from_: The sender of the SMS.              - _subaccount_id_: The sub-account identifier.              - _message_id_: The ID of your SMS.          2. **Value**: The text or keyword you&#39;re searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.             For example, if you are searching for a SMS with the status of Scheduled, the final query would look like this:    &#x60;q&#x3D;status:Scheduled&#x60;  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;div&gt;    &lt;p&gt;Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:&lt;br/&gt;&lt;/p&gt;     &lt;ul&gt;       &lt;li&gt;q&#x3D;from:%2B61437085284&lt;/li&gt;     &lt;/ul&gt;     &lt;p&gt;You can use the &lt;a href&#x3D;\&quot;https://www.urlencoder.org/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;URL encoder&lt;/a&gt; to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.&lt;/p&gt;   &lt;/div&gt; &lt;/div&gt; | [optional] [default to &#39;field_name&#39;]
 **order_by** | **str**| Specifies the field and order to sort the results by. The value is composed of the field name followed by a colon and the sort direction (_asc_ for ascending or _desc_ for descending).  The default sort order is by _date_ in ascending order. You can use the following fields:    - _date_   - _username_   - _from_    - _to_   - _status_   - _body_  For example, if you want to order by the most recently sent SMS, you should sort by date in descending order. The query would look like this:    &#x60;order_by&#x3D;date:desc&#x60; | [optional] [default to &#39;date:asc&#39;]
 **date_from** | **int**| Start date to filter results. It should be in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 
 **date_to** | **int**| End date to filter results. It should be in &lt;a href&#x3D;\&quot;http://help.clicksend.com/what-is-a-unix-timestamp\&quot; target&#x3D;\&quot;_blank\&quot;&gt;Unix format&lt;/a&gt;. | [optional] 

### Return type

[**ViewSmsHistory**](ViewSmsHistory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_sms_inbound_automation**
> ViewSmsInboundAutomation view_sms_inbound_automation(inbound_rule_id, content_type=content_type)

View SMS Inbound Automation

_Get specific inbound sms automation_

Get specific inbound sms automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| inbound_rule_id | path | integer(int32) | true | Inbound rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_sms_inbound_automation import ViewSmsInboundAutomation
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    inbound_rule_id = 'inbound_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View SMS Inbound Automation
        api_response = api_instance.view_sms_inbound_automation(inbound_rule_id, content_type=content_type)
        print("The response of DefaultApi->view_sms_inbound_automation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_sms_inbound_automation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inbound_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSmsInboundAutomation**](ViewSmsInboundAutomation.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_sms_inbound_automations**
> ViewSmsInboundAutomations view_sms_inbound_automations(content_type=content_type)

View SMS Inbound Automations

_Get all inbound sms automations_

Get all inbound sms automations

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | Page number |
| limit | query | integer(int32) | false | Number of records per page |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_sms_inbound_automations import ViewSmsInboundAutomations
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View SMS Inbound Automations
        api_response = api_instance.view_sms_inbound_automations(content_type=content_type)
        print("The response of DefaultApi->view_sms_inbound_automations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_sms_inbound_automations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSmsInboundAutomations**](ViewSmsInboundAutomations.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_sms_receipts**
> ViewSmsReceipts view_sms_receipts(content_type=content_type, page=page, limit=limit)

View SMS Receipts

Use this endpoint to retrieve <a href="https://help.clicksend.com/article/49eq1qdcui-how-do-i-receive-sms-delivery-receipts-delivery-status-updates" target="_blank">SMS delivery receipts</a> sent by your recipient. 
To be able to view receipts, add a <a href="https://help.clicksend.com/en/articles/42317-delivery-notifications-reports" target="_blank">delivery report</a> rule with the Action set to **POLL** in the Dashboard, or use the [**Create SMS Delivery Receipt Rule**](/automations/sms/other/create-sms-delivery-receipt-rule) endpoint. 
Control [pagination](/#pagination) with the _page_ and _limit_ query parameters to specify the page of results and the number of items returned.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_sms_receipts import ViewSmsReceipts
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    page = 1 # int | The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. (optional) (default to 1)
    limit = 15 # int | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. (optional) (default to 15)

    try:
        # View SMS Receipts
        api_response = api_instance.view_sms_receipts(content_type=content_type, page=page, limit=limit)
        print("The response of DefaultApi->view_sms_receipts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_sms_receipts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **page** | **int**| The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. | [optional] [default to 1]
 **limit** | **int**| The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. | [optional] [default to 15]

### Return type

[**ViewSmsReceipts**](ViewSmsReceipts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_sms_statistics**
> ViewSmsStatistics view_sms_statistics(content_type=content_type)

View SMS Statistics

_Get sms statistics_


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_sms_statistics import ViewSmsStatistics
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View SMS Statistics
        api_response = api_instance.view_sms_statistics(content_type=content_type)
        print("The response of DefaultApi->view_sms_statistics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_sms_statistics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSmsStatistics**](ViewSmsStatistics.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_sms_templates**
> ViewSmsTemplates view_sms_templates(content_type=content_type, page=page, limit=limit, q=q, order_by=order_by)

View SMS Templates

Use this endpoint to retrieve <a href="https://help.clicksend.com/article/9z9uloaz8y-sms-templates-for-different-industries" target="_blank">SMS templates</a>. You can filter the SMS templates result using the query parameters.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_sms_templates import ViewSmsTemplates
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    page = 1 # int | The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. (optional) (default to 1)
    limit = 15 # int | The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. (optional) (default to 15)
    q = 'field_name' # str | Allows filtering of results based on your search criteria. The query should be in the format `field_name:value`.  1. **Field Name**: The field within the SMS history you want to filter by. You can use the following fields:    - _template_id_ : The ID of the template   - _template_name_ : The name of the template   - _body_ : The body content of the template.          2. **Value**: The text or keyword you're searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.      For example, if you are searching for the template with the name of _sample_name_, the final query would look like this:     `q=template_name:sample_name`  <div class=\"info-box\">   <h4><i class=\"fas fa-info-circle\"></i> Note:</h4>   <div>    <p>Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:<br/></p>     <ul>       <li>q=from:%2B61437085284</li>     </ul>     <p>You can use the <a href=\"https://www.urlencoder.org/\" target=\"_blank\">URL encoder</a> to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.</p>   </div> </div> (optional) (default to 'field_name')
    order_by = 'template_id:asc' # str | Specifies the field and order to sort the results by.  The value is composed of the field name followed by a colon and the sort direction (_asc_ for ascending or _desc_ for descending).  The default sort order is by _template_id_ in ascending order. You can use the following fields:      - _template_id_ : The ID of the Template - _template_name_ : The name of the Template - _body_ : The body content of the Template  For example, if you want to order by the _template_id_ in descending order, the query would look like this:    `order_by=template_id:desc` (optional) (default to 'template_id:asc')

    try:
        # View SMS Templates
        api_response = api_instance.view_sms_templates(content_type=content_type, page=page, limit=limit, q=q, order_by=order_by)
        print("The response of DefaultApi->view_sms_templates:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_sms_templates: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **page** | **int**| The page number to retrieve. Use this parameter to navigate through the [pagination](/#pagination) results. The default value is 1. | [optional] [default to 1]
 **limit** | **int**| The number of items to return per page. This parameter controls the size of each page of results. The default value is 15. | [optional] [default to 15]
 **q** | **str**| Allows filtering of results based on your search criteria. The query should be in the format &#x60;field_name:value&#x60;.  1. **Field Name**: The field within the SMS history you want to filter by. You can use the following fields:    - _template_id_ : The ID of the template   - _template_name_ : The name of the template   - _body_ : The body content of the template.          2. **Value**: The text or keyword you&#39;re searching for within the specified field. If left empty after the colon, the filter will look for all templates with any value in the **Field Name**.      For example, if you are searching for the template with the name of _sample_name_, the final query would look like this:     &#x60;q&#x3D;template_name:sample_name&#x60;  &lt;div class&#x3D;\&quot;info-box\&quot;&gt;   &lt;h4&gt;&lt;i class&#x3D;\&quot;fas fa-info-circle\&quot;&gt;&lt;/i&gt; Note:&lt;/h4&gt;   &lt;div&gt;    &lt;p&gt;Some characters have to be encoded. For example, if you are searching for SMS sent from the phone number +61437085284, your search query q would be:&lt;br/&gt;&lt;/p&gt;     &lt;ul&gt;       &lt;li&gt;q&#x3D;from:%2B61437085284&lt;/li&gt;     &lt;/ul&gt;     &lt;p&gt;You can use the &lt;a href&#x3D;\&quot;https://www.urlencoder.org/\&quot; target&#x3D;\&quot;_blank\&quot;&gt;URL encoder&lt;/a&gt; to encode the text. If a character is not an alphanumeric character (A-Z, a-z, 0-9), it is typically either reserved or unsafe and should be encoded.&lt;/p&gt;   &lt;/div&gt; &lt;/div&gt; | [optional] [default to &#39;field_name&#39;]
 **order_by** | **str**| Specifies the field and order to sort the results by.  The value is composed of the field name followed by a colon and the sort direction (_asc_ for ascending or _desc_ for descending).  The default sort order is by _template_id_ in ascending order. You can use the following fields:      - _template_id_ : The ID of the Template - _template_name_ : The name of the Template - _body_ : The body content of the Template  For example, if you want to order by the _template_id_ in descending order, the query would look like this:    &#x60;order_by&#x3D;template_id:desc&#x60; | [optional] [default to &#39;template_id:asc&#39;]

### Return type

[**ViewSmsTemplates**](ViewSmsTemplates.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_specific_client_account**
> ViewSpecificClientAccount view_specific_client_account(client_user_id, content_type=content_type)

View Specific Client Account

_Get Reseller clients Account_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| client_user_id | path | integer(int32) | true | User ID of client |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_specific_client_account import ViewSpecificClientAccount
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    client_user_id = 'client_user_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Specific Client Account
        api_response = api_instance.view_specific_client_account(client_user_id, content_type=content_type)
        print("The response of DefaultApi->view_specific_client_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_specific_client_account: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **client_user_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSpecificClientAccount**](ViewSpecificClientAccount.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_specific_fax_receipt**
> ViewSpecificFaxReceipt view_specific_fax_receipt(message_id, content_type=content_type)

View Specific Fax Receipt

_Get a single fax receipt based on message id._

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| message_id | path | string | true | ID of the message receipt to retrieve |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_specific_fax_receipt import ViewSpecificFaxReceipt
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    message_id = 'message_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Specific Fax Receipt
        api_response = api_instance.view_specific_fax_receipt(message_id, content_type=content_type)
        print("The response of DefaultApi->view_specific_fax_receipt:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_specific_fax_receipt: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSpecificFaxReceipt**](ViewSpecificFaxReceipt.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_specific_list**
> ViewSpecificList view_specific_list(list_id, content_type=content_type)

View Specific List

_Get specific contact list_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| list_id | path | integer(int32) | true | List ID |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_specific_list import ViewSpecificList
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    list_id = 'list_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Specific List
        api_response = api_instance.view_specific_list(list_id, content_type=content_type)
        print("The response of DefaultApi->view_specific_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_specific_list: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSpecificList**](ViewSpecificList.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_specific_return_address**
> ViewSpecificReturnAddress view_specific_return_address(return_address_id, content_type=content_type)

View Specific Return Address

_Get specific post return address_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| return_address_id | path | integer(int32) | true | Return address ID |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_specific_return_address import ViewSpecificReturnAddress
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    return_address_id = 'return_address_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Specific Return Address
        api_response = api_instance.view_specific_return_address(return_address_id, content_type=content_type)
        print("The response of DefaultApi->view_specific_return_address:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_specific_return_address: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **return_address_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSpecificReturnAddress**](ViewSpecificReturnAddress.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_specific_sms_campaign**
> ViewSpecificSmsCampaign view_specific_sms_campaign(sms_campaign_id, content_type=content_type)

View Specific SMS Campaign

Use this endpoint to view a specific SMS campaign.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_specific_sms_campaign import ViewSpecificSmsCampaign
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    sms_campaign_id = 'sms_campaign_id_example' # str | ID of SMS campaign to get
    content_type = 'application/json' # str |  (optional)

    try:
        # View Specific SMS Campaign
        api_response = api_instance.view_specific_sms_campaign(sms_campaign_id, content_type=content_type)
        print("The response of DefaultApi->view_specific_sms_campaign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_specific_sms_campaign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sms_campaign_id** | **str**| ID of SMS campaign to get | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSpecificSmsCampaign**](ViewSpecificSmsCampaign.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_specific_sms_receipt**
> ViewSpecificSmsReceipt view_specific_sms_receipt(message_id, content_type=content_type)

View Specific SMS Receipt

Use this endpoint to retrieve a specific <a href="https://help.clicksend.com/article/49eq1qdcui-how-do-i-receive-sms-delivery-receipts-delivery-status-updates" target="_blank">SMS delivery receipt</a>, including those that have been marked as read. When you send an SMS, a delivery receipt is generated and can be received. 
This endpoint enables you to retrieve those receipts.

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_specific_sms_receipt import ViewSpecificSmsReceipt
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    message_id = 'message_id_example' # str | The _message_id_ of the SMS delivery receipt to retrieve
    content_type = 'application/json' # str |  (optional)

    try:
        # View Specific SMS Receipt
        api_response = api_instance.view_specific_sms_receipt(message_id, content_type=content_type)
        print("The response of DefaultApi->view_specific_sms_receipt:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_specific_sms_receipt: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **message_id** | **str**| The _message_id_ of the SMS delivery receipt to retrieve | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSpecificSmsReceipt**](ViewSpecificSmsReceipt.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_specific_subaccount**
> ViewSpecificSubaccount view_specific_subaccount(subaccount_id, content_type=content_type)

View Specific Subaccount

_Get specific subaccount_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| subaccount_id | path | integer(int32) | true | ID of subaccount to get |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_specific_subaccount import ViewSpecificSubaccount
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    subaccount_id = 'subaccount_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Specific Subaccount
        api_response = api_instance.view_specific_subaccount(subaccount_id, content_type=content_type)
        print("The response of DefaultApi->view_specific_subaccount:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_specific_subaccount: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subaccount_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSpecificSubaccount**](ViewSpecificSubaccount.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_specific_transaction**
> ViewSpecificTransaction view_specific_transaction(transaction_id, content_type=content_type)

View Specific Transaction

_Get specific Transaction_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| transaction_id | path | string | true | ID of transaction to retrieve |

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_specific_transaction import ViewSpecificTransaction
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    transaction_id = 'transaction_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Specific Transaction
        api_response = api_instance.view_specific_transaction(transaction_id, content_type=content_type)
        print("The response of DefaultApi->view_specific_transaction:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_specific_transaction: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **transaction_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSpecificTransaction**](ViewSpecificTransaction.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_stripped_string_rule**
> ViewStrippedStringRule view_stripped_string_rule(rule_id, content_type=content_type)

View Stripped String Rule

_Get email to sms stripped string rule_

Get email to sms stripped string rule

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| rule_id | path | integer(int32) | true | Your rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_stripped_string_rule import ViewStrippedStringRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    rule_id = 'rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Stripped String Rule
        api_response = api_instance.view_stripped_string_rule(rule_id, content_type=content_type)
        print("The response of DefaultApi->view_stripped_string_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_stripped_string_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewStrippedStringRule**](ViewStrippedStringRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_stripped_string_rules**
> ViewStrippedStringRules view_stripped_string_rules(content_type=content_type)

View Stripped String Rules

_Get list of email to sms stripped string rules_

Get list of email to sms stripped string rules

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | Page number |
| limit | query | integer(int32) | false | Number of records per page |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_stripped_string_rules import ViewStrippedStringRules
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Stripped String Rules
        api_response = api_instance.view_stripped_string_rules(content_type=content_type)
        print("The response of DefaultApi->view_stripped_string_rules:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_stripped_string_rules: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewStrippedStringRules**](ViewStrippedStringRules.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_subaccounts**
> ViewSubaccounts view_subaccounts(content_type=content_type)

View Subaccounts

_Get all subaccounts_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_subaccounts import ViewSubaccounts
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Subaccounts
        api_response = api_instance.view_subaccounts(content_type=content_type)
        print("The response of DefaultApi->view_subaccounts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_subaccounts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewSubaccounts**](ViewSubaccounts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_template_categories**
> ViewTemplateCategories view_template_categories(content_type=content_type)

View Template Categories

_Get all master email template categories_

Get all master email template categories

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | Page number |
| limit | query | integer(int32) | false | Number of records per page |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_template_categories import ViewTemplateCategories
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Template Categories
        api_response = api_instance.view_template_categories(content_type=content_type)
        print("The response of DefaultApi->view_template_categories:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_template_categories: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewTemplateCategories**](ViewTemplateCategories.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_template_category**
> ViewTemplateCategory view_template_category(category_id, content_type=content_type)

View Template Category

_Get specific master email template category_

Get specific master email template category

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| category_id | path | integer(int32) | true | Email category id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_template_category import ViewTemplateCategory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    category_id = 'category_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Template Category
        api_response = api_instance.view_template_category(category_id, content_type=content_type)
        print("The response of DefaultApi->view_template_category:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_template_category: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **category_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewTemplateCategory**](ViewTemplateCategory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_templates_in_category**
> ViewTemplatesInCategory view_templates_in_category(category_id, content_type=content_type)

View Templates in Category

_Get all master email templates in a category_

Get all master email templates in a category

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| category_id | path | integer(int32) | true | Email category id |
| page | query | integer(int32) | false | Page number |
| limit | query | integer(int32) | false | Number of records per page |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_templates_in_category import ViewTemplatesInCategory
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    category_id = 'category_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Templates in Category
        api_response = api_instance.view_templates_in_category(category_id, content_type=content_type)
        print("The response of DefaultApi->view_templates_in_category:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_templates_in_category: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **category_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewTemplatesInCategory**](ViewTemplatesInCategory.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_voice_delivery_receipt_rule**
> ViewVoiceDeliveryReceiptRule view_voice_delivery_receipt_rule(receipt_rule_id, content_type=content_type)

View Voice Delivery Receipt Rule

_Get specific voice delivery receipt automation_

Get specific voice delivery receipt automation

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| receipt_rule_id | path | integer(int32) | true | Receipt rule id |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_voice_delivery_receipt_rule import ViewVoiceDeliveryReceiptRule
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    receipt_rule_id = 'receipt_rule_id_example' # str | 
    content_type = 'application/json' # str |  (optional)

    try:
        # View Voice Delivery Receipt Rule
        api_response = api_instance.view_voice_delivery_receipt_rule(receipt_rule_id, content_type=content_type)
        print("The response of DefaultApi->view_voice_delivery_receipt_rule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_voice_delivery_receipt_rule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **receipt_rule_id** | **str**|  | 
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewVoiceDeliveryReceiptRule**](ViewVoiceDeliveryReceiptRule.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_voice_delivery_receipt_rules**
> ViewVoiceDeliveryReceiptRules view_voice_delivery_receipt_rules(content_type=content_type)

View Voice Delivery Receipt Rules

_Get all voice delivery receipt automations_

Get all voice delivery receipt automations

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | Page number |
| limit | query | integer(int32) | false | Number of records per page |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_voice_delivery_receipt_rules import ViewVoiceDeliveryReceiptRules
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Voice Delivery Receipt Rules
        api_response = api_instance.view_voice_delivery_receipt_rules(content_type=content_type)
        print("The response of DefaultApi->view_voice_delivery_receipt_rules:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_voice_delivery_receipt_rules: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewVoiceDeliveryReceiptRules**](ViewVoiceDeliveryReceiptRules.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_voice_languages**
> ViewVoiceLanguages view_voice_languages(content_type=content_type)

View Voice Languages

_Get all voice languages_


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_voice_languages import ViewVoiceLanguages
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Voice Languages
        api_response = api_instance.view_voice_languages(content_type=content_type)
        print("The response of DefaultApi->view_voice_languages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_voice_languages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewVoiceLanguages**](ViewVoiceLanguages.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_voice_receipts**
> ViewVoiceReceipts view_voice_receipts(content_type=content_type)

View Voice Receipts

_Get all voice receipts_

**Push Delivery Receipts**

If you prefer, we can push message replies to your server as they arrive with us.

1. Log into your account.
2. Click on your profile on the top right.
3. Then click on the Messaging Settings option.
4. Click on Voice then Delivery Report Rules.
5. Click the 'Add New Rule' button.
6. Select the 'URL' action.
7. Enter the URL and click 'Save'.
    

The following variables will be posted to the URL specified:

| Variable | Description |
| --- | --- |
| `timestamp_send` | Timestamp of the original send request in UNIX format. e.g 1439173980 |
| `timestamp` | Timestamp of delivery report in UNIX format. e.g 1439173981 |
| `message_id` | Message ID, returned when originally sending the message. |
| `status` | Delivered or Undelivered |
| `status_code` | Status code. Refer to 'Voice Delivery Status Codes' in docs. |
| `status_text` | Status text. |
| `error_code` | Error code. |
| `error_text` | Error text. |
| `custom_string` | A custom string used when sending the original message. |
| `user_id` | The user ID of the user who sent the message. |
| `subaccount_id` | The subaccount ID of the user who sent the message. |
| `message_type` | 'voice' (constant). |
| `digits` | Numbers the recipient pressed on their keypad during the call. A blank string will be used if they didn't provide any input. |

**Pull Delivery Receipts**

Receive delivery reports by polling. You can poll our server and retrieve delivery reports at a time that suits you.

1. Log into your account.
2. Click on your profile on the top right.
3. Then click on the Messaging Settings option.
4. Click on Voice then Delivery Report Rules.
5. Click the 'Add New Rule' button.
6. Select the 'Poll' action.
7. Then click 'Save'.
    

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_voice_receipts import ViewVoiceReceipts
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Voice Receipts
        api_response = api_instance.view_voice_receipts(content_type=content_type)
        print("The response of DefaultApi->view_voice_receipts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_voice_receipts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewVoiceReceipts**](ViewVoiceReceipts.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_voice_statistics**
> ViewVoiceStatistics view_voice_statistics(content_type=content_type)

View Voice Statistics

_Get voice statistics_

Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.

<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_voice_statistics import ViewVoiceStatistics
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Voice Statistics
        api_response = api_instance.view_voice_statistics(content_type=content_type)
        print("The response of DefaultApi->view_voice_statistics:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_voice_statistics: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewVoiceStatistics**](ViewVoiceStatistics.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_your_numbers**
> ViewYourNumbers view_your_numbers(content_type=content_type, page=page, limit=limit, q=q, q2=q2, excluding_number_type=excluding_number_type, exclude_10dlc_campaign=exclude_10dlc_campaign)

View Your Numbers

_Get all available dedicated numbers_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |
| q | query | string | false | Filter numbers based on multiple criteria. The query string should be formatted as key-value pairs separated by commas. Available filter keys: `type`, `number_type`, `country` |
| q2 | query | string | false | Filter numbers based on multiple criteria. The query string should be formatted as key-value pairs separated by commas. Available filter keys: `type` |
| excluding_number_type | query | string | false | Exclude specific number types from the results. Available number types: `shortcode`, `tollfree`, `10DLC` |
| exclude_10dlc_campaign | query | boolean | false | When set to true, excludes all numbers that are associated with 10DLC campaigns |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_your_numbers import ViewYourNumbers
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)
    page = 1 # int | Page number (optional) (default to 1)
    limit = 15 # int | Number of records per page (optional) (default to 15)
    q = 'type:sms,number_type:longcode,country:AU' # str | Filter numbers based on multiple criteria. The query string should be formatted as key-value pairs separated by commas. Available filter keys: - `type`: Message type (e.g., `SMS`, `MMS`) - `number_type`: Number classification (e.g., `longcode`, `shortcode`, `tollfree`, `10DLC`) - `country`: Two-letter country code (e.g., `AU`, `US`)  (optional)
    q2 = 'type:mms' # str |  (optional)
    excluding_number_type = '10DLC' # str | Exclude specific number types from the results. Available number types: - `shortcode` - `tollfree` - `10DLC`  (optional)
    exclude_10dlc_campaign = False # bool | When set to true, excludes all numbers that are associated with 10DLC campaigns (optional) (default to False)

    try:
        # View Your Numbers
        api_response = api_instance.view_your_numbers(content_type=content_type, page=page, limit=limit, q=q, q2=q2, excluding_number_type=excluding_number_type, exclude_10dlc_campaign=exclude_10dlc_campaign)
        print("The response of DefaultApi->view_your_numbers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_your_numbers: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 
 **page** | **int**| Page number | [optional] [default to 1]
 **limit** | **int**| Number of records per page | [optional] [default to 15]
 **q** | **str**| Filter numbers based on multiple criteria. The query string should be formatted as key-value pairs separated by commas. Available filter keys: - &#x60;type&#x60;: Message type (e.g., &#x60;SMS&#x60;, &#x60;MMS&#x60;) - &#x60;number_type&#x60;: Number classification (e.g., &#x60;longcode&#x60;, &#x60;shortcode&#x60;, &#x60;tollfree&#x60;, &#x60;10DLC&#x60;) - &#x60;country&#x60;: Two-letter country code (e.g., &#x60;AU&#x60;, &#x60;US&#x60;)  | [optional] 
 **q2** | **str**|  | [optional] 
 **excluding_number_type** | **str**| Exclude specific number types from the results. Available number types: - &#x60;shortcode&#x60; - &#x60;tollfree&#x60; - &#x60;10DLC&#x60;  | [optional] 
 **exclude_10dlc_campaign** | **bool**| When set to true, excludes all numbers that are associated with 10DLC campaigns | [optional] [default to False]

### Return type

[**ViewYourNumbers**](ViewYourNumbers.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **view_your_return_addresses**
> ViewYourReturnAddresses view_your_return_addresses(content_type=content_type)

View Your Return Addresses

_Get list of post return addresses_

### Parameters

| Parameter | In | Type | Required | Description |
| --- | --- | --- | --- | --- |
| page | query | integer(int32) | false | [Page number](/#pagination) |
| limit | query | integer(int32) | false | [Number of records per page](/#pagination) |


Refer to [Status Codes](/#status-codes) for definitions of HTTP status code responses.


<div style="background-color: #FF6A4B; padding: 10px; border-radius: 8px;">
  <span style="color: white;">This endpoint requires authentication,</span> 
  <a href="/docs/#authentication" style="color: white; text-decoration: underline;">more info...</a>
</div>

### Example

* Basic Authentication (basicAuth):

```python
import clicksend
from clicksend.models.view_your_return_addresses import ViewYourReturnAddresses
from clicksend.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://rest.clicksend.com
# See configuration.py for a list of all supported configuration parameters.
configuration = clicksend.Configuration(
    host = "https://rest.clicksend.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: basicAuth
configuration = clicksend.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with clicksend.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = clicksend.DefaultApi(api_client)
    content_type = 'application/json' # str |  (optional)

    try:
        # View Your Return Addresses
        api_response = api_instance.view_your_return_addresses(content_type=content_type)
        print("The response of DefaultApi->view_your_return_addresses:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DefaultApi->view_your_return_addresses: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_type** | **str**|  | [optional] 

### Return type

[**ViewYourReturnAddresses**](ViewYourReturnAddresses.md)

### Authorization

[basicAuth](../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

