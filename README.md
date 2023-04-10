# Large CSV File Ingestion and Schema Validation
This project is designed to demonstrate how to ingest and validate a large CSV file using Python. It includes examples of using multiple libraries for file ingestion and compares their computational efficiency.

# Data Generation

The `data_generation.py` script is designed to produce a large simulated dataset of over 2.5GB, consisting of fundamental details of individuals.

# Data Reading
The `data_ingestion_week6.ipynb` notebook explores different methods of reading a file, including pandas, Dask, Modin, and Vaex. The computational efficiency of each method is compared and the findings are presented in the notebook.

# Data Validation
The ingested data is validated by performing basic cleaning on the column names, such as removing special characters and white spaces. A YAML file is created to define the schema and column names. A utility file is created to verify the ingested data against a schema, in order to ensure that the data contains the expected number of columns with correct column names.

# Data Output
The ingested data is then written to a pipe-separated text file in gz format. 

# Files
* data_generation.py: Python script that generates a sample data file.
* data_ingestion_week6.ipynb: Jupyter notebook that demonstrates different methods of ingesting data and performs basic validation and summary.
* schema.yaml: YAML file that defines the schema and column names.
* utility.py: Utility file for column validation.  
* dataset.gz: Dataset is stored in Pipe seprated format in gz file.  

# Usage
* Clone the repository.
* Install the required libraries.
* Run data_generation.py to generate a sample data file.
* Open data_ingestion.ipynb in Jupyter notebook and Follow the steps in the notebook to ingest, validate, and summarize the data.
