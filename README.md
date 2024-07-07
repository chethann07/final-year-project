# Morse Code Authentication System

## Overview

The Morse Code Authentication System is a multi-factor authentication framework that combines facial recognition and Morse code input to secure user login processes. This system integrates traditional password authentication with advanced biometric verification and innovative Morse code input via blinking.

## How It Works

**Registration Process:**

Create User: Users start by creating an account with a username and password.
Face Enrollment: The system captures the user's facial data for future recognition.
Success/Failure: If the face enrollment is successful, the user is registered. If not, the registration fails, and the user is notified.

**Login Process:**

User Authentication: The user enters their username and password.
Face Detection: The system attempts to recognize the user's face.
If face detection fails, an alert message is sent via a Telegram bot.
If face detection is successful, the user proceeds to the next step.
Morse Code Authentication: The user enters Morse code by blinking, using a virtual keyboard.
The system interprets the blinks into Morse code and verifies it.
If Morse code authentication is successful, the user is logged in.
If Morse code authentication fails, the login is unsuccessful, and the user may be prompted to answer a security question to reset their Morse code password.

**Alerts:**

Telegram Notifications: Alerts are sent via a Telegram bot for events such as failed face detection attempts.
Key Components
Facial Recognition: Uses OpenCV for capturing and recognizing the user's face.
Morse Code Input: Interprets user blinks into Morse code using a virtual keyboard.
Telegram Bot: Sends alert messages to the user in case of failed authentication attempts.
