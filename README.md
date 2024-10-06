
# Antarikṣa Jñānavṛkṣa
Antarikṣa Jñānavṛkṣa (अन्तरिक्ष ज्ञानवृक्ष) is an innovative web application dedicated to exploring and visualizing the fascinating realm of extrasolar planets, commonly known as exoplanets. The name, which translates to "The Tree of Space Knowledge," captures the essence of our mission to cultivate and disseminate knowledge about celestial bodies that orbit stars beyond our solar system.
A web application that visualizes data on extrasolar planets. The data is based on PHL's [Habitable Exoplanets Catalog](http://phl.upr.edu/projects/habitable-exoplanets-catalog/data/database), which provides a comprehensive collection of exoplanet data, combined with additional modeled planet-related information.



### Features
- **Visualizes data for extrasolar planets (exoplanets)**
- **Data sourced from the PHL's Habitable Exoplanets Catalog**
- **Backend-powered JSON file generation for planets, stars, and statistical data**

---

### Frontend Setup

1. Set up a simple web server using [XAMPP](http://www.apachefriends.org) or any similar software.
2. Create a new folder within `htdocs/` and name it "exoplanets".
3. Navigate to the newly created folder.
4. Clone the repository into this folder by running:
    ```bash
    git clone https://github.com/vinayak1729-web/travel_to_exoplanets
    ```
5. Once cloned, open `localhost/exoplanets` in your browser to access the app frontend. Please note that the search functionality will not work until you set up the backend.

---

### Backend Setup

1. **Set up the database**:
   - If you plan to import a new dataset of exoplanets, first set up a SQL database on your server.
   - Open the SQL storage software installed on your system (such as phpMyAdmin, Adminer, etc.).
   - Create a new database named `exoplanets`.

2. **Import the Exoplanets Dataset**:
   - Inside the folder `backend/`, you’ll find an exported `phlplanets.sql` file. Import this file into your `exoplanets` database.
   - You can also visit the [PHL website](http://phl.upr.edu/projects/habitable-exoplanets-catalog/data/database) to download the latest CSV file to update the database with the most recent exoplanet data.

3. **Generating JSON Files**:
   - Once the import is complete, you can use backend resources in your browser to generate various JSON files.
   - **Important:** Keep the directory structure as-is, otherwise, file generation may fail.

   - **Export Planets**: Generates JSON files for each planetary system and stores them in `app/js/data/planetsystems/`.
   - **Export Stars**: Generates a JSON file with star data and stores it in `app/js/data/`.
   - **Export Planet Stats**: Generates statistical information about planets and saves it as a JSON file in `app/js/data/`.
   - **Export General Statistics**: Generates a list of basic statistics for planets and stars, stored as a JSON file in `app/js/data/`.

---

### Running the Project Locally

1. **Frontend**:
   - Ensure you have set up a local web server (such as XAMPP) and cloned the repository into the `htdocs/` folder.
   - Open your browser and navigate to `localhost/exoplanets` to interact with the app.

2. **Backend**:
   - Open your SQL software (phpMyAdmin, Adminer, etc.) and create a new database named `exoplanets`.
   - Import the `phlplanets.sql` file located in the `backend/` folder into this database.
   - Once the database is set up, you can generate the required JSON files for planets, stars, and statistics.

---

Feel free to customize the app further by using the most recent exoplanet data, or by adding new features!

