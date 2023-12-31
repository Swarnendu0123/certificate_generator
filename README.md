# Certificate Generator

This Python script generates certificates for a list of names provided in the `Data.xlsx` Excel file. Each certificate includes the participant's name, a unique certificate ID, and the title "Certificate of Participation". The generated certificates are saved as PDF files in the `certificates` directory.

## Prerequisites

Before running the script, ensure you have the following installed:

- Python 3.x
- Pillow library (PIL) for image processing: Install using `pip install Pillow`
- Pandas library for reading data from Excel: Install using `pip install pandas`

## Usage

1. **Prepare your data:**
   - Create an Excel file named `Data.xlsx` with a column named `name` containing the names of the participants.

2. **Prepare your certificate template:**
   - Ensure your certificate template is in a supported image format (e.g., PNG, JPEG).
   - Name the template image file `cert.png` and place it in the same directory as the script.

3. **Prepare your font files:**
   - Choose TrueType font (TTF) files for text and titles on the certificates.
   - Name the text font file `BRUSHSCI.TTF` and the title font file `kepler_std_bold_semicondensed_subhead.otf`.
   - Place the font files in a `fonts` directory in the same location as the script.

4. **Run the script:**
   - Open a terminal or command prompt and navigate to the directory containing the script.
   - Run the script by executing `python script_name.py` (replace `script_name.py` with the actual name of your Python script).

5. **Generated Certificates:**
   - The generated certificates will be saved as PDF files in the `certificates` directory.

## Notes

- Ensure the font size and location settings in the script (`font_size`, `location`) are appropriate for your certificate template.
- Verify the color settings (`text_color`) for proper visibility against the certificate background.
- Each certificate includes a unique certificate ID.
- Test the script with a small set of names first to ensure the certificates are generated as expected.
