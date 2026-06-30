# Login Auto Role + Password Eye Update

Changes:
- Removed default username and password values.
- Removed the Role dropdown.
- Role is detected automatically after entering username.
- Added an eye button beside the password box to show/hide password anytime.
- Uses System.Windows.Forms.Timer explicitly to avoid Timer ambiguity errors.

Use:
1. Replace LoginForm.cs and AuthService.cs.
2. Add PasswordService.cs if missing.
3. Clean Solution.
4. Rebuild Solution.
