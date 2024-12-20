# Art-Sense Project

Art-Sense is a data-driven project designed to recommend artworks based on users' preferences for curated visits. It takes the dataset from the Metropolitan Museum of Art as an example. The project combines machine learning and data analytics to create a tailored art exploration experience. Future work includes creating the actual visits with preferred routes.

---

## Project Structure

### 1. **Data**
   - **`data/clean/`**: Processed and cleaned datasets ready for analysis.
      - `artists.csv`: Contains data on various artists.
      - `artworks.csv`: Details about artworks, including metadata.
      - `floors.csv`: Information about museum floor plans.
      - `full_dataset.csv`: Combined dataset for machine learning.
      - `galleries.csv`: Details of individual galleries.
      - `geo.csv`: Geographical data for museum layout.
      - `images_and_tags.csv`: Artworks linked with image data and tags.
      - `linking_table.csv`: Reference table for connecting different datasets.
      - `museum.csv`: General information about the museum.
      - `wings.csv`: Data on the wings of the museum.
   - **`data/intermediate_or_backups/`**: Backup or intermediary files from preprocessing.
   - **`data/raw/`**: Unprocessed raw data.
      - `.gitattributes`: Configuration file for Git attributes.
      - `met_objects.txt`: Raw text dataset from the MET.

### 2. **Notebooks**
   - Jupyter notebooks used for various stages of the project:
      - `load-clean-met-dataset.ipynb`: Loading and cleaning MET data.
      - `split-df-into-smaller.ipynb`: Splitting the dataset into smaller dataframes for better, more focused cleaning.
      - `filter-merge-preprocess.ipynb`: Preprocessing for Machine Learning and merging the smaller dataframes into a clean(er) full dataset.
      - `machine-learning.ipynb`: Implementing and evaluating the recommendation system.
      - `museum_floorplan.ipynb`: Visualizing museum floor plans for future implementation for the curated visits.
      - `web-scraping-images.ipynb`: Scripts for web scraping images and clean the tags.

### 3. **Slides**
   - **`presentation/`**: Presentation slides summarizing the project with a mock-up.

### 4. **Code Files**
   - `app.py`: Main script for running the streamlit application (unfinnished).
   - `requirements.txt`: Lists all dependencies for the project.
   - `pyproject.toml`: Configuration file for Python project metadata.

### 5. **Environment**
   - **`.venv/`**: Python virtual environment for dependency management.

---

## Getting Started

### Prerequisites
1. Python 3.8+
2. Virtual Environment (recommended)
3. Libraries specified in `requirements.txt`

### Installation
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd art-sense
   ```
2. Activate the virtual environment:
   ```bash
   source .venv/bin/activate  # Linux/Mac
   .venv\Scripts\activate   # Windows
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

---

## Features
- **Personalized Recommendations**: Tailors artworks based on user preferences.
- **Data Analytics**: Processes and visualizes large datasets from the MET.
- **Museum Floor Plan Integration**: Suggests efficient routes for viewing artworks.
- **Machine Learning**: Leverages Random Forest Classifier model to predict user interest in artworks.
- **Web Scraping**: Enhances datasets with additional images and titles, directly from the MET's website

---

## Future Improvements
- Add the real visit's route for a proper curated visit based on the liked 
- Add real-time user feedback to enhance recommendations.
- Expand to other museums and galleries.
- Incorporate augmented reality for interactive museum visits.

---

## Contributors
- Clara Cachapa Baeta (Project Lead) for Ironhack Data Analytics Bootcamp

---

## Acknowledgments
- The MET for providing the open-access dataset.
- Ironhack for giving me the opportunity to learn and supporting me throughout the whole bootcamp.