# Combined Fix - Employee Accounts + Password-only Update Profile

## Fixed in this update

1. Restored `Employee Accounts` module and `Add New` account function.
2. `Employee Accounts` is Admin-only through `Security.cs`.
3. `Update Profile` no longer allows users to edit Role, Email, or Full Name.
4. `Update Profile` now only allows password change:
   - Old Password
   - New Password
   - Confirm Password
5. New password is stored using PBKDF2 hash.
6. Existing sample plain-text passwords still work until changed.
7. New employee accounts receive a temporary password by email through `smtp_config.json`.

## Files included

- MainForm.cs
- Security.cs
- ProfileForm.cs
- EmployeeAccountForm.cs
- EmailService.cs
- PasswordService.cs
- AuthService.cs
- smtp_config.json

## Apply

Replace the matching files, add the new forms/classes if not already included, set `smtp_config.json` as Content + Copy if newer, then Clean and Rebuild.
