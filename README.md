# Exploring Structured Data with LangChain and Llama 3

This repository showcases the application of LangChain with Llama 3, a factual language model, to interact with structured data stored in a SQLite database. The provided Jupyter notebook (`structured_llama.ipynb` file) demonstrates how to:

- **Query the Database:** Formulate questions that retrieve specific information from the database schema.
- **Ask Follow-up Questions:** Ask Llama 3 additional questions related to the retrieved data, leveraging its knowledge and capabilities.
- **Replicate Model:** The code utilizes the Replicate platform ([https://replicate.com](https://replicate.com)) to run the "meta-llama-3-8b-instruct" model. This powerful factual language model excels at understanding and responding to factual queries.

## Data Preparation:

The repository includes scripts that facilitate the conversion of data scraped from the web into a usable format for interaction with Llama 3:

- `nba.txt`: Contains initially scraped NBA roster information, likely gathered from a website.
- `txt2csv.py`: Python script that transforms the scraped data in `nba.txt` into a structured comma-separated values (CSV) file named `nba_roster.csv`.
- `csv2db.py`: Python script that reads the `nba_roster.csv` file and populates a SQLite database named `nba_roster.db` with the extracted information.

## Getting Started:

1. **Clone or download the repository.**
2. **Install dependencies:** Execute `pip install -r requirements.txt` to install the required Python libraries for running the scripts and the notebook.
3. **(Optional) Update `nba.txt`:** If you wish to use a different data source, you can modify the `nba.txt` file with your own scraped data.
4. **Run data conversion scripts:** Execute `python txt2csv.py` followed by `python csv2db.py` to generate the `nba_roster.csv` and `nba_roster.db` files, respectively.
5. **Open the Jupyter notebook:** Launch your preferred Jupyter Notebook environment and open the provided `.ipynb` file.
6. **Explore queries:** Follow the notebook's instructions to interact with the database using LangChain and Llama 3.

### Disclaimer:

- This is a demonstration of using LangChain and Llama 3 for querying structured data. It serves as a starting point for further exploration.
- Ensure you have the necessary permissions and adhere to the terms of service for scraping data from websites.

## Further Enhancements:

- Integrate data validation and error handling into the data conversion scripts.
- Expand the range of query types the notebook supports, allowing for more complex information retrieval.
- Visualize the retrieved data using libraries like Matplotlib or Seaborn to gain deeper insights.

This repository helps you explore the fascinating capabilities of LangChain and Llama 3 for leveraging factual language models to interact with structured databases. Feel free to modify and extend the code to fit your specific data and query needs.