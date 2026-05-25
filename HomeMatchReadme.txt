HomeMatch Project Readme

Hi there! Welcome to the HomeMatch application. This project uses AI (specifically OpenAI's language models) and a Chroma vector database to match home buyers with their perfect real estate properties.

How it works:
First, the script generates 10 realistic real estate listings using the language model. 
Second, it saves these listings into a vector database (ChromaDB) so we can search through them semantically.
Third, we take some pre-defined buyer preferences and search the database for the top 3 matching homes.
Finally, the language model rewrites the descriptions of those top 3 homes to highlight exactly why they fit the buyer's needs, without changing any of the actual facts (like the price or number of bedrooms).

Prerequisites:
To run this project, you'll need Python 3 installed. It's also highly recommended to use a virtual environment. You will also need an OpenAI API Key.

How to run the code:
1. Open your terminal and install the required packages by running:
   pip install -r requirements.txt

2. Open the "HomeMatch.ipynb" file in Jupyter Notebook or VS Code.

3. In the first code block, paste your OpenAI API key where it says "YOUR_OPENAI_API_KEY". 

4. Run all the cells in the notebook from top to bottom. 

Once the notebook finishes running, it will automatically save the generated properties into a file called "Listings.txt", and the customized recommendations will be printed right there at the bottom of the notebook for you to read.

