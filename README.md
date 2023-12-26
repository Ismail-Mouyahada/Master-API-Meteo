# Weather Station API

This Flask-based API is designed to manage data related to a weather station, including weather measurements, sensors, and user information. The API interacts with a MySQL database to store and retrieve data.

## Features

1. **Add Weather Data:**
   - **Endpoint:** `/api/v1/ajouter/`
   - **Method:** POST
   - **Description:** Adds new weather data to the database, including temperature, humidity, and sensor information.

2. **Fetch Weather Data:**
   - **Endpoint:** `/api/v1/donnees/`
   - **Method:** GET
   - **Description:** Retrieves all weather data from the database.

3. **Filter Humidity Data:**
   - **Endpoint:** `/api/v1/donnees/humidite/<int:id>`
   - **Method:** GET
   - **Description:** Retrieves humidity data for a specific record identified by the provided `id`.

4. **Filter Temperature Data:**
   - **Endpoint:** `/api/v1/donnees/temperature/<int:id>`
   - **Method:** GET
   - **Description:** Retrieves temperature data for a specific record identified by the provided `id`.

5. **Modify Weather Data:**
   - **Endpoint:** `/api/v1/modifier/`
   - **Method:** PUT
   - **Description:** Modifies existing weather data based on the provided JSON payload, including updates to temperature, humidity, date, and sensor data.

6. **Delete Weather Data:**
   - **Endpoint:** `/api/v1/supprimer/<int:id>`
   - **Method:** DELETE
   - **Description:** Deletes weather data for a specific record identified by the provided `id`.

7. **Add Sensor Data:**
   - **Endpoint:** `/api/v1/capteur/ajouter/`
   - **Method:** POST
   - **Description:** Adds new sensor data to the database, including sensor name, description, version, and status.

8. **Fetch Sensor Data:**
   - **Endpoint:** `/api/v1/capteurs/`
   - **Method:** GET
   - **Description:** Retrieves all sensor data from the database.

9. **Filter Sensor Data:**
   - **Endpoint:** `/api/v1/capteur/<int:id>`
   - **Method:** GET
   - **Description:** Retrieves sensor data for a specific record identified by the provided `id`.

10. **Modify Sensor Data:**
    - **Endpoint:** `/api/v1/capteur/modifier/`
    - **Method:** PUT
    - **Description:** Modifies existing sensor data based on the provided JSON payload, including updates to sensor name, description, version, and status.

11. **Delete Sensor Data:**
    - **Endpoint:** `/api/v1/capteur/supprimer/<int:id>`
    - **Method:** DELETE
    - **Description:** Deletes sensor data for a specific record identified by the provided `id`.

12. **Add User Data:**
    - **Endpoint:** `/api/v1/user/ajouter/`
    - **Method:** POST
    - **Description:** Adds new user data to the database, including username, name, surname, email, and password.

13. **Fetch User Data:**
    - **Endpoint:** `/api/v1/utilisateurs/`
    - **Method:** GET
    - **Description:** Retrieves all user data from the database.

14. **Filter User Data:**
    - **Endpoint:** `/api/v1/utilisateur/<int:id>`
    - **Method:** GET
    - **Description:** Retrieves user data for a specific record identified by the provided `id`.

15. **Modify User Data:**
    - **Endpoint:** `/api/v1/user/modifier/`
    - **Method:** PUT
    - **Description:** Modifies existing user data based on the provided JSON payload, including updates to username, name, surname, email, and password.

16. **Delete User Data:**
    - **Endpoint:** `/api/v1/user/supprimer/<int:id>`
    - **Method:** DELETE
    - **Description:** Deletes user data for a specific record identified by the provided `id`.

## How to Use

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/weather-api.git
   cd weather-api

    Install Dependencies:

  bash

    pip install -r requirements.txt

Configure Database:

    Set up a MySQL database and update the configuration in config.py.

Run the Application:

bash

    python app.py

Access Endpoints:
        Use a tool like Postman to interact with the API endpoints.


    
