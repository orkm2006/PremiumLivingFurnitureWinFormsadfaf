# ProfileForm Full View Fix

This update fixes the Update Profile window layout.

Changes:
- Increased ProfileForm height so the complete form is visible when opened.
- Added AutoScroll protection to prevent controls from being clipped on smaller displays.
- Kept Update Profile as password-only:
  - Username read-only
  - Old Password
  - New Password
  - Confirm Password
  - Show passwords
- Role / Email / Full Name are still not editable here.

Apply:
1. Replace ProfileForm.cs.
2. Clean Solution.
3. Rebuild Solution.
