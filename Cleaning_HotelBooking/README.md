# 🧹 Hotel Booking Data Cleaning Project

This project demonstrates essential **data cleaning techniques** on a hotel booking dataset, as part of practicing core skills for Data Analysts and Data Scientists.

## 📁 Dataset

The dataset is sourced from Kaggle:
**[Hotel Booking Dataset by saadharoon27](https://www.kaggle.com/datasets/saadharoon27/hotel-booking-dataset)**

It contains information about bookings in a city hotel and a resort hotel.

## 🔧 Tools Used

- Python 🐍
- Pandas
- NumPy
- SciPy
- Matplotlib / Seaborn (optional)
- Google Colab / Jupyter Notebook

## 📊 Cleaning Steps Performed

1. **Loading the data**
   - Used `kagglehub` to download the dataset
   - Loaded CSV into a pandas DataFrame

2. **Handling Missing Values**
   - Identified missing values using `.isnull().sum()`
   - Dropped rows with missing `country` values

3. **Removing Outliers**
   - Applied **Z-Score** method to remove statistical outliers from numeric columns

4. **Changing Data Types**
   - Converted `is_canceled` to boolean (`bool`)
   - Converted `reservation_status_date` to datetime

5. **Standardizing Column Names**
   - Lowercased all column names
   - Replaced spaces with underscores
   - Removed any leading/trailing whitespace

6. **String Cleaning**
   - Cleaned up `email` column: trimmed spaces and converted to lowercase

7. **Exporting Cleaned Data**
   - Saved the cleaned dataset as `cleaned_hotel_bookings.csv`

## 🧪 How to Run

1. Clone this repository or open the notebook in Google Colab.
2. Make sure `kagglehub` is installed and configured properly.
3. Run all cells in the notebook to download the dataset and perform cleaning.
4. The cleaned file will be saved as `cleaned_hotel_bookings.csv`.

## 📌 Notes

- Outliers were removed based on Z-Score > 3
- This is a practice project and can be extended further with EDA, feature engineering, and modeling

---

## 🔗 Author

Made with ❤️ by [Your Name]

