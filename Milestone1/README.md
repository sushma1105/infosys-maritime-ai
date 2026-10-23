
Agentic AI for Maritime Freight Pricing and Route Optimization
Milestone 1 — Authentication Module
This milestone implements the required Streamlit authentication layer with maritime-themed branding. It is the secure entry point for the larger project; it does not claim to implement freight pricing or route-optimization agents yet. Those capabilities are planned for later milestones.

Included
Login and signup in one Streamlit application.
Required-field checks, unique username/email checks, email validation, password confirmation, and fixed security questions.
Bcrypt password hashing and hashed security answers.
Password policy: 8+ characters, uppercase, lowercase, number, and special character.
JWT session tokens with expiry and logout.
Forgot Password via security-question verification or email OTP.
Separate administrator sign-in and a user list that never displays password data.
Maritime UI styling: navy, ocean teal, port/anchor identity, and workspace-focused copy.
Tech stack
Python, Streamlit, SQLite, bcrypt, PyJWT, Gmail SMTP for OTP, Google Colab Secrets, and ngrok.

Run in Google Colab
Open Milestone1_Maritime_Auth.ipynb in Colab.
In Colab Secrets, add JWT_SECRET, NGROK_AUTHTOKEN, EMAIL_ADDRESS, EMAIL_PASSWORD, ADMIN_EMAIL, and ADMIN_PASSWORD. Enable notebook access for each.
Use a Gmail App Password for EMAIL_PASSWORD, not your normal Gmail password.
Run all cells from top to bottom and open the ngrok URL printed by the last cell. Keep that cell running while using the app.
If ngrok reports too many active endpoints, stop old tunnels or restart the runtime before launching one new tunnel.
Local run
Install dependencies with pip install streamlit pyjwt bcrypt, set the environment variables above, then run streamlit run app.py. Email OTP requires valid Gmail SMTP credentials.

Screenshots

login.png — login page
signup.png — signup form
forgot-security-question.png — security-question recovery
forgot-email-otp.png — OTP recovery
user-dashboard.png — user dashboard
admin-dashboard.png — admin dashboard
