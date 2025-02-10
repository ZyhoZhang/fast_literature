# Academic Paper Summarization and Documentation Tool

**Developed by Zyho Zhang**

When you take notes on literature review, this Python script automates the summarization of academic papers by allowing you to add and update paper entries. It stores the entries persistently in a JSON file and generates a Microsoft Word document (`academic_papers.docx`) that groups papers by research topic and sorts them by publication year.

## Features

- **Topic Selection:**  
  Choose from a predefined list of research topics when adding a new paper entry.

- **Paper Details Input:**  
  Add details such as title, authors (separated by semicolons), publication year, and journal name (selected from a list or entered manually).

- **Multi-line Abstracts:**  
  Enter abstracts as multi-line input. Separate paragraphs by leaving a blank line, and finish the input by typing `END` on a new line.

- **Persistent Data Storage:**  
  All entries are saved in a JSON file (`papers_data.json`) so that your data persists between runs.

- **Word Document Output:**  
  The script creates or updates a Microsoft Word document (`academic_papers.docx`) in real time. Each topic is represented with a heading, and the papers under each topic are numbered sequentially with abstracts indented as separate paragraphs.

- **Modify Abstract Functionality:**  
  Search for and modify the abstract of an existing paper by entering one or more author names (separated by semicolons) and the publication year. If multiple matches are found, the script will list the paper titles along with topic information and prompt you to select the correct entry.

## Installation

1. **Python Version:**  
   Make sure you have Python 3.x installed on your system.

2. **Install Dependencies:**  
   This project requires the `python-docx` library. Install it using pip:
   ```bash
   pip install python-docx

## Usage

Run the script from your terminal:

    ```bash
    python notes_literature.py

## When the script starts, you’ll be presented with a menu:

1. **Add New Paper Entry:**
   - **Topic Selection:** Choose a research topic by entering its corresponding number.
   - **Paper Details Input:** Provide the title, author names (separated by semicolons), publication year, and choose or input the journal name.
   - **Multi-line Abstract Input:**  
     Enter the abstract line by line. To create separate paragraphs, leave a blank line between them. When finished, type `END` on a new line.
   - **Output:**  
     The new entry is saved in `papers_data.json` and the Word document (`academic_papers.docx`) is updated immediately.

2. **Modify Paper Abstract:**
   - **Search for a Paper:**  
     Enter one or more author names (separated by semicolons) and the publication year to locate the desired paper.
   - **Selection:**  
     If multiple matches are found, the script lists the matching titles (with topic details) and prompts you to select one.
   - **Update Abstract:**  
     After reviewing the current abstract, input a new multi-line abstract using the same method as for adding a new entry.
   - **Output:**  
     The updated abstract is saved in `papers_data.json` and the Word document is regenerated.

3. **Exit:**  
   Exit the application. All your data remains saved and the Word document will reflect your latest changes.