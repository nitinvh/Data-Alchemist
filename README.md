# Data-Alchemist

## Project Overview
The Data-Alchemist project by **Group 1** focuses on creating a movie recommendation system using the MovieLens dataset. This project involves data merging, cleaning, and subsequent recommendation system development using R programming. This README provides step-by-step instructions for setting up and contributing to the project.

## Table of Contents
1. [Project Setup](#project-setup)
2. [Dataset Preparation](#dataset-preparation)
3. [Data Merging](#data-merging)
4. [Working on the Recommendation System](#working-on-the-recommendation-system)
5. [Contributing](#contributing)
6. [License](#license)

## Project Setup
### Prerequisites
- Ensure you have R and RStudio installed on your system.
- Required R packages may include `tidyverse` and other relevant libraries for data manipulation and visualization.

### Step-by-Step Setup
1. **Clone the Project Repository:**
   ```bash
   git clone https://github.com/your-repo/data-alchemist.git
   cd data-alchemist
   ```
2. **Create a Datasets Folder:**
   - After cloning the project, you must create a folder named `datasets` inside the `Data-Alchemist` directory if it does not already exist.

     Example:
     ```
     /Data-Alchemist/datasets/
     ```

## Dataset Preparation
1. **Download the MovieLens CSV Files:**
   - Download all six CSV files of the MovieLens dataset from [MovieLens Website](https://grouplens.org/datasets/movielens/) or other provided sources.
   - Move these files into the `datasets` folder you created.

     Example file structure:
     ```
     /Data-Alchemist/datasets/
     ├── tags.csv
     ├── movies.csv
     ├── ratings.csv
     ├── links.csv
     ├── genome-tags.csv
     └── genome-scores.csv
     ```

## Data Merging
1. **Open the Data Merging Script:**
   - Open the file `MovieLensDataMerging.Rmd` in RStudio.

2. **Modify File Paths:**
   - Update the file paths in the code to reflect your system's structure. For example:
     ```r
     read.csv("/path/to/your/Data-Alchemist/datasets/tag.csv")
     ```
   - Make sure to change all necessary paths in the script to ensure files are correctly loaded from your `datasets` folder.

3. **Run the Script:**
   - Execute all cells in the `MovieLensDataMerging.Rmd` file. As the script runs, it will clean and merge the datasets.
   - Save the cleaned datasets within the `datasets` folder using appropriate file paths.

     Example:
     ```r
     write.csv(cleaned_data, "/path/to/your/Data-Alchemist/datasets/cleaned_data.csv")
     ```

4. **Verify the Output:**
   - Upon successful completion of the script, you should find six cleaned datasets and one combined dataset (`group1_combined_data.csv`) in the `datasets` folder.
   - If everything is in place, congrats! You have completed the data merging process.

## Working on the Recommendation System
1. **Open the Recommendation Script:**
   - Open `MovieRecommendationSystem.Rmd` in RStudio.

2. **Import the Combined Dataset:**
   - Import the `group1_combined_data.csv` file into this script to start developing the recommendation system.

     Example:
     ```r
     combined_data <- read.csv("/path/to/your/Data-Alchemist/datasets/group1_combined_data.csv")
     ```
3. **Develop and Contribute:**
   - Use the combined dataset to build and test your recommendation models.
   - Add your contributions and experiments within `MovieRecommendationSystem.Rmd`.

## Contributing
- Fork the repository and create your branch for new features or fixes.
- Commit your changes and push them to your branch.
- Open a pull request for review.

---

Feel free to let me know if you'd like any additional customization or specific details added to your README!