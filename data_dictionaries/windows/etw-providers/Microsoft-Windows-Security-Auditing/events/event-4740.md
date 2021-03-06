# Event ID 4740: A user account was locked out

## Description
This event generates every time a user account is locked out. For user accounts, this event generates on domain controllers, member servers, and workstations.

## Data Dictionary
|Standard Name|Field Name|Type|Description|Sample Value|
|---|---|---|---|---|
|user_name|TargetUserName|UnicodeString|the name of the account that was locked out.|`Auditor`|
|user_domain|TargetDomainName|UnicodeString|the name of computer account from which logon attempt was received and after which target account was locked out.|`WIN81`|
|user_sid|TargetSid|SID|SID of account that was locked out.|`S-1-5-21-3457937927-2839227994-823803824-2104`|
|user_reporter_sid|SubjectUserSid|SID|SID of account that performed the lockout operation.|`S-1-5-18`|
|user_reporter_name|SubjectUserName|UnicodeString|the name of the account that performed the lockout operation.|`DC01$`|
|user_reporter_domain|SubjectDomainName|UnicodeString|domain or computer name.|`CONTOSO`|
|user_reporter_id|SubjectLogonId|HexInt64|hexadecimal value that can help you correlate this event with recent events that might contain the same Logon ID, for example, "4624: An account was successfully logged|`0x3e7`|

## References
* [MS Source](https://github.com/MicrosoftDocs/windows-itpro-docs/blob/master/windows/security/threat-protection/auditing/event-4740.md)
* [MS Security Auditing Category - Account Management](https://docs.microsoft.com/en-us/windows/security/threat-protection/auditing/advanced-security-audit-policy-settings#account-management)
* [MS Security Auditing Sub-category - Audit User Account Management](https://github.com/MicrosoftDocs/windows-itpro-docs/tree/master/windows/security/threat-protection/auditing/audit-user-account-management.md)

## Tags
* etw_level_Informational
* etw_task_task_0
* Account Management
* Audit User Account Management