# 🔐 Password Strength Meter (Streamlit App)

This is a **Streamlit-based web application** designed to check the strength of your passwords, generate secure ones, and keep track of your last 10 passwords to avoid reusing old ones.

---

## 🚀 Features

- 🔐 **Check Password Strength:** Validates length, letter case, digits, special characters, and uniqueness.
- 🔑 **Generate Strong Passwords:** Creates random strong passwords with a combination of letters, digits, and special characters.
- 📜 **Password History:** Keeps a record of the last 10 passwords used/generated.
- 🛡️ **Email Check:** Ensures that your password does not contain your email address.
- 🌟 **User-Friendly Interface:** A clean and interactive UI using **Streamlit** for seamless experience.

---

## 🧰 Tech Stack

- [Python](https://www.python.org/)
- [Streamlit](https://streamlit.io/)
- [JSON](https://www.json.org/json-en.html) (for local password storage)

---

## 📦 Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/password-strength-meter.git
    cd password-strength-meter
    ```

2. **Create a virtual environment** (optional but recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. **Install the dependencies**:
    ```bash
    pip install streamlit
    ```

4. **Run the app**:
    ```bash
    streamlit run app.py
    ```

---

## 📝 How It Works

1. **Password Strength Check:**
   - Enter a password and it will be evaluated based on the following criteria:
     - Minimum length of 8 characters
     - Contains both uppercase and lowercase letters
     - Includes at least one digit and one special character
     - Not matching your email or any previous password
   - The app will display feedback and suggestions to improve the password strength if necessary.

2. **Password Generation:**
   - Choose the desired password length (6, 8, 12, or custom).
   - A strong random password will be generated with a mix of letters, digits, and special characters.

3. **Password History:**
   - The app stores the last 10 passwords used/generated, helping you avoid reusing old passwords.
   - You can clear the history at any time using the button in the sidebar.

---

## 🛡️ Security Notes

- **Password History:** Passwords are saved locally in a `passwords.json` file. Make sure this file is protected and not shared publicly.
- **Email Protection:** The app checks to ensure that your password does not contain your email address, offering an additional layer of security.
- **Clipboard:** The generated password can be copied manually, but the clipboard feature may vary depending on the environment.

---