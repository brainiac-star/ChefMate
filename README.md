# ChefMate – AI Recipe Generator

ChefMate is a vision-powered cooking assistant that uses Google Gemini to:
- Detect ingredients from an image
- Generate 3 creative recipes
- Classify cuisine (Indian, Italian, Thai, etc.)
- Adapt recipes using preferences (healthiness, spice level, prep time)
- Save recipe outputs inside the notebook (force-save)

## Features
- Vision ingredient recognition
- Multi-recipe generation
- Cuisine classification
- Sliders for customization
- Zero-waste cooking tips
- Leftover meal ideas

## Installation
pip install google-genai ddgs pillow ipywidgets
jupyter nbextension enable --py widgetsnbextension


## API Key (Kaggle)
Add in **Add-ons → Secrets**:


GOOGLE_API_KEY = <your key>


## Usage


chef = ChefMateAgent(enable_search=True)
chef.run("fridge_sample.jpg", healthiness_level=7, spice_level=5, max_prep_time=30)


## Output
Each recipe includes:
- Title + cuisine  
- Quick facts  
- Ingredients  
- Steps  
- Nutrition  
- Shopping list  
- Zero-waste tips  
- Leftover plan  
