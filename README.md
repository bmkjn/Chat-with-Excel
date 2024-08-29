# Chat-with-Excel
---

## Overview

This project is designed to create a data analysis agent that helps non-technical users interpret and understand advertising data from multiple mediums, such as TV, Radio, Print, Digital, and Outdoor. The agent is powered by Google Generative AI and uses the PandasAI library to provide clear and concise answers to user queries. The data is organized into separate dataframes for each medium, and the agent is trained to respond accurately based on these dataframes.


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

3. Install the required packages


4. Set up environment variables:

   - Create a `.env` file in the root directory and add the following:

     ```bash
     GOOGLE_API_KEY=<your-google-api-key>
     LANGCHAIN_API_KEY=<your-langchain-api-key>
     PANDASAI_API_KEY=<your-pandasai-api-key>
     ```

## Usage

1. Place your data files (Excel format) in the `Data/` directory.
2. Run the `ChatWithExcel.ipynb` script:

4. The agent will be initialized with data from the specified files. You can interact with the agent by sending queries like:

   - "What is the GrossAmount of Jalsa Movies for TV medium?"
   - "What is the Market for the top spent Channel for TV medium?"
   - "Who created the campaign for Radio Mirchi Jaipur Channel?"

5. The agent will respond with clear and concise answers based on the data.

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


