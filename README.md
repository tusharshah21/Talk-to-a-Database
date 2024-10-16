
# AtliQ Tees: Talk to a Database

This project is an end-to-end Large Language Model (LLM) system based on Google PaLM and LangChain, designed for AtliQ Tees, a T-shirt store. The system allows users to interact with a MySQL database by asking questions in natural language. It then translates these questions into SQL queries, executes them, and returns accurate responses. The data includes inventory, sales, and discounts information, enabling a store manager to ask questions such as:

- "How many white Adidas T-shirts do we have left in stock?"
- "What would our store's revenue be if we sold all extra-small T-shirts with discounts applied?"

The system is equipped to generate accurate SQL queries based on natural language input and execute them against the MySQL database.

---

## Project Highlights

- **AtliQ Tees Store**: Sells brands like Adidas, Nike, Van Heusen, and Levi’s.
- **Data Storage**: Inventory, sales, and discount data is maintained in a MySQL database.
- **Question and Answer System**:
  - Uses **Google PaLM** for language processing.
  - Leverages **Hugging Face embeddings** for semantic search.
  - Built with **Streamlit** for a user-friendly UI.
  - Developed using the **LangChain framework** for efficient chaining.
  - **ChromaDB** is used as a vector store for embedding-based search.
  - Incorporates **few-shot learning** for improved query generation.
- **User Interaction**: Store managers can ask inventory and sales-related questions in natural language, and the system provides accurate answers.

---

## Installation

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/tusharshah21/Talk-to-a-Database.git
   ```
2. Navigate to the project directory:
   ```bash
   cd 4_sqldb_tshirts
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Set up the Google API key:
   - Acquire an API key from [Makersuite](https://makersuite.google.com) and add it to the `.env` file:
     ```bash
     GOOGLE_API_KEY="your_api_key_here"
     ```
5. For database setup, run `database/db_creation_atliq_t_shirts.sql` in your MySQL Workbench to initialize the schema and data.

---

## Usage

1. Run the Streamlit app:
   ```bash
   streamlit run main.py
   ```
2. Open the web app in your browser and ask questions about the store’s inventory and sales.
