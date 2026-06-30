# Employee Account Email OTP Update - smtp_config.json Version

This update removes the need to configure Windows environment variables for SMTP.

The ERP now reads SMTP settings from `smtp_config.json` placed next to the application `.exe` file.

## Files included

- `MainForm.cs`
- `Security.cs`
- `EmployeeAccountForm.cs`
- `EmailService.cs`
- `PasswordService.cs`
- `AuthService.cs`
- `smtp_config.json`

## How to use

1. Replace the existing `.cs` files in your Visual Studio project.
2. Add the new files if Visual Studio does not include them automatically:
   - `EmployeeAccountForm.cs`
   - `EmailService.cs`
   - `PasswordService.cs`
3. Add `smtp_config.json` to the project.
4. Select `smtp_config.json` in Visual Studio.
5. In Properties, set:
   - Build Action: Content
   - Copy to Output Directory: Copy if newer
6. Edit `smtp_config.json` with your real sender mailbox SMTP settings.
7. Clean Solution.
8. Rebuild Solution.
9. Run the ERP and test Employee Accounts > Add New.

## Security behaviour

- The administrator does not type or see the new employee password.
- The system generates a temporary password automatically.
- The temporary password is sent to the employee email address.
- The database stores only a PBKDF2 password hash.
- If the email cannot be sent, the account is not created.
