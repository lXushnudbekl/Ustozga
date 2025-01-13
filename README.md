# Django Telegram Bot Project

## Overview

This project is a simple Django-based application integrated with a Telegram bot. Its primary purpose is to allow users to register and log in, after which a notification is sent to the connected Telegram bot.

---

## Features

1. **User Authentication**:
   - Users can register via the web interface.
   - Users can log in using their credentials.

2. **Telegram Bot Integration**:
   - Notifications are sent to the Telegram bot upon user registration and login.

---

## Requirements

### Prerequisites
Ensure you have the following installed on your system:
- Python (3.8 or higher)
- Django (4.0 or higher)
- Aiogram (for Telegram bot integration)

### Telegram Bot
You need a Telegram bot token. Create a bot via [BotFather](https://t.me/BotFather) and obtain the token.

---

## Installation

1. Set up a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Configure the project:
   - Rename `.env.example` to `.env`.
   - Add your environment variables (e.g., database credentials, Telegram bot token) to the `.env` file:
     ```env
     TELEGRAM_BOT_TOKEN=your-telegram-bot-token
     ```

4. Apply database migrations:
   ```bash
   python manage.py migrate
   ```

5. Run the development server:
   ```bash
   python manage.py runserver
   ```

6. Start the Telegram bot script (if separate):
   ```bash
   python bot.py
   ```

---

## Usage

1. **Register/Login:**
   - Open the web application.
   - Register a new account or log in with an existing account.

2. **Telegram Notification:**
   - After registration or login, check the Telegram bot chat for notifications.

---

## Project Structure

```plaintext
project/
├── app/                # Main Django application
├── bot.py              # Telegram bot script
├── templates/          # HTML templates
├── static/             # Static files (CSS, JS, images)
├── manage.py           # Django management script
├── requirements.txt    # Python dependencies
└── .env                # Environment variables (ignored by Git)
```

---

## Future Improvements

- Add more user features such as profile management.
- Extend the Telegram bot functionalities (e.g., user-specific commands).
- Implement error handling and logging for the bot.

---

## Contributing

Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes and push to the branch.
4. Open a pull request.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Contact

For any inquiries or issues, feel free to reach out:
- **Email:** x200828@gmail.com
- **Telegram:** [l_xushnudbek_l](https://t.me/l_xushnudbek_l)
