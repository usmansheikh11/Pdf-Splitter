Here’s a README template for your GitHub repository, describing the Python script that processes PDF files:

---

# PDF Splitter for Research and Appendix

This Python script processes PDF files in a specified directory and splits them into two separate PDFs: one containing the research content and the other containing the appendix. The script uses the `pypdf` library to read and write PDF files, and it organizes the output into distinct folders for easier management.

## Features

- **Automatic Directory Creation**: If the output directories for research and appendix PDFs don't exist, the script automatically creates them.
- **Content-Based Splitting**: The script scans each page of the PDF to find the word "appendix" and splits the document into two parts:
  - The research content up to the page where "appendix" is found.
  - The appendix content starting from the page where "appendix" is found.
- **Batch Processing**: The script can process multiple PDF files at once, organizing the output into separate folders.

## Installation

1. Ensure you have Python installed on your system.
2. Install the required library using pip:
   ```bash
   pip install pypdf
   ```
3. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/yourusername/pdf-splitter.git
   cd pdf-splitter
   ```

## Usage

1. Place the PDF files you want to process in the `files` directory.
2. Run the script:
   ```bash
   python pdf_splitter.py
   ```
3. The output will be saved in two separate directories:
   - `./research`: Contains the research content PDFs.
   - `./appendix`: Contains the appendix content PDFs.

## Directory Structure

- `./files`: Directory where the input PDF files should be placed.
- `./research`: Directory where the research PDFs will be saved.
- `./appendix`: Directory where the appendix PDFs will be saved.

## Example

If a PDF file named `example.pdf` contains the word "appendix" on page 10, the script will:
- Save pages 1-9 in `./research/example.pdf`.
- Save pages 10 onward in `./appendix/example.pdf`.

## Contributing

Contributions are welcome! If you have any improvements or fixes, feel free to submit a pull request or open an issue.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

.
