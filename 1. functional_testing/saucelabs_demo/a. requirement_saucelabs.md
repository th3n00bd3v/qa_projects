## Requirement Analysis

### 1. Login screen

- **Objective**: Verify the login functionality of the application.
- **Inputs**: 
  - **Username**: `standard_user`, `locked_out_user`, `problem_user`, `performance_glitch_user`
  - **Password**: `secret_sauce`
  - **Login Button**: Submits the login form.
- **Expected Behavior**:
  - For valid credentials (`standard_user` and `secret_sauce`), login should be successful and the user should be redirected to the product page.
  - For invalid credentials, the system should display an error message such as "Username and password do not match any user in this service."
  - Specific usernames should have different behaviors:
    - `locked_out_user`: Should not be able to log in, and an appropriate error message should be shown.
    - `problem_user`: Should log in, but may have an issue on the product page (e.g., missing image or text).
    - `performance_glitch_user`: Should be able to log in but with a performance delay.
