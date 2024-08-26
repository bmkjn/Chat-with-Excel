# Chat-with-Excel
---

# Advertising Data Analysis Agent

## Overview

This project is designed to create a data analysis agent that helps non-technical users interpret and understand advertising data from multiple mediums, such as TV, Radio, Print, Digital, and Outdoor. The agent is powered by Google Generative AI and uses the PandasAI library to provide clear and concise answers to user queries. The data is organized into separate dataframes for each medium, and the agent is trained to respond accurately based on these dataframes.

## Project Structure

- **`main.py`**: The main script that sets up the environment, loads the data, initializes the data connectors, and creates the agent.
- **`Data/`**: Directory containing Excel files with ad campaign data for different mediums (TV, Radio, Print, Digital, Outdoor).
- **`field_descriptions.py`**: Contains dictionaries that describe each column in the dataframes for different mediums.
- **`descriptions.py`**: Contains detailed descriptions of the agent's role for each medium, helping it interpret user queries accurately.

## Installation

### Prerequisites

- Python 3.7+
- pip (Python package installer)
- Virtual environment (optional but recommended)

### Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/advertising-data-agent.git
   cd advertising-data-agent
   ```

2. Set up a virtual environment (optional but recommended):

   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

4. Set up environment variables:

   - Create a `.env` file in the root directory and add the following:

     ```bash
     GOOGLE_API_KEY=<your-google-api-key>
     LANGCHAIN_API_KEY=<your-langchain-api-key>
     PANDASAI_API_KEY=<your-pandasai-api-key>
     ```

## Usage

1. Place your data files (Excel format) in the `Data/` directory.
2. Run the `main.py` script:

   ```bash
   python main.py
   ```

3. The agent will be initialized with data from the specified files. You can interact with the agent by sending queries like:

   - "What is the GrossAmount of Jalsa Movies for TV medium?"
   - "What is the Market for the top spent Channel for TV medium?"
   - "Who created the campaign for Radio Mirchi Jaipur Channel?"

4. The agent will respond with clear and concise answers based on the data.

## Features

- **Data Interpretation**: The agent can interpret user queries with potential spelling or capitalization errors and provide the closest matching correct values.
- **Multi-Medium Support**: The agent can handle data from different mediums, including TV, Radio, Print, Digital, and Outdoor.
- **Language Support**: The agent can provide insights into various aspects of ad campaigns, including language, market, amount spent, and more.

## Customization

- **Field Descriptions**: You can customize the descriptions of the fields in the dataframes by modifying the dictionaries in `field_descriptions.py`.
- **Agent Description**: The agent's role and behavior can be tailored for each medium by updating the descriptions in `descriptions.py`.

## Example Queries

- "What are the top 5 ad languages for TV?"
- "Who created the campaign for Radio Mirchi Jaipur Channel?"
- "What is the GrossAmount of Jalsa Movies for TV medium?"

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any features or fixes.

