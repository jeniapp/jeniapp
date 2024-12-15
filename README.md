# Diet Recommendation System 
This is a Streamlit-based diet recommendation system that uses machine learning to suggest recipes based on user-defined nutritional preferences and optional ingredient filters. 

## Features 
- TDEE calculator for total caloric needed in a day.
- Nutritional input preferences like calories, fat, protein, and sodium. 
- Filter recipes based on users choosing specific dietary preferences. 
- View detailed recommendations with recipe names, calories, ingredients, and instructions.

## Project Structure
```
/web_server_diet
|--  dataset
       |-- dataset_recipes.csv          # Cleaned dataset
|--  diet_recommendation.py             # Main Streamlit app
|--  food_image.jpeg	
|--  requirements.txt                   # Python dependencies
|--  README.md
```

## How to Run 
1. Navigate to the web_server_diet directory:
```bash 
cd ~/web_server_diet
```
2. Install the required dependencies (with appropriate version included):
```bash
pip install -r requirements.txt
```
3. Run the Streamlit app:
```bash
streamlit run diet_recommendation.py
```
4. Open the app in your browser at http://localhost:8501.

## Run on Cloud
Or you can access to this URL without installing anything: https://dietrecom.azurewebsites.net

