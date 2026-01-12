### Author: Confy-Code
# 📘 Weather Application – Technical Documentation

## 1. Overview

This document explains the structure and functionality of the **Weather Information Web App**.  
The application is built using **Flask** and integrates an external weather API to provide real-time weather data.

---

## 2. Application Flow

1. User opens the home page (`index.html`)
2. User enters a city name
3. Request is sent to the Flask backend
4. Backend fetches weather data using the weather service
5. Weather details are displayed on `weather.html`
6. If the city is not found, `city_not_found.html` is rendered

---

## 3. Backend Files

### `server.py`
This is the **main Flask server file**.

**Responsibilities:**
- Initialize the Flask application
- Define routes
- Handle form submissions
- Render HTML templates

---

### `weather.py`
This file handles **weather API communication**.

**Responsibilities:**
- Send requests to the external weather API
- Parse API responses
- Return processed weather data to the server

---

## 4. Frontend Files

### `templates/index.html`
- Home page
- Contains the city search form

### `templates/weather.html`
- Displays weather details for the searched city

### `templates/city_not_found.html`
- Displayed when an invalid or unknown city is entered

---

### `static/style.css`
- Controls layout and styling
- Improves visual appearance and user experience

---

## 5. External API Integration

The application uses an external weather API to fetch real-time data.

**Key Notes:**
- API key is required
- API calls are isolated in `weather.py`
- Responses are validated before rendering

---

## 6. Environment Variables

Required environment variable in this case are private

## 7. Error Handling

- Invalid city names return a friendly error page
- API errors are handled gracefully
- Server-side errors are logged

---

## 8. Limitations

- Displays only current weather data
- No forecasts or historical data
- No user authentication

---

## 9. Future Enhancements

- Add weather forecasts
- Improve UI/UX
- Add unit tests
- Add location-based weather detection using AI
- A user-interactive AI chatbot

---

## 10. Conclusion

This project demonstrates a simple Flask-based web application with API integration and template rendering,
suitable for learning and small-scale deployment.

