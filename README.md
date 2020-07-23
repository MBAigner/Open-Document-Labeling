# Open Document Labeling
A tool for labeling document regions as a basis for various region detection task.

The tool is based on the work of https://github.com/Cartucho/OpenLabeling and adapted for a labeling of PDF documents.
Example PDFs are obtained from the ICDAR Table Recognition Challenge 2013 https://roundtrippdf.com/en/data-extraction/pdf-table-recognition-dataset/.

IN PROGRESS

## How-to

* Input documents in data/custom/pdfs (or change PDF_LABEL_INPUT_PATH in utils/constants accordingly)
* Run main/main.py
* Label documents
* The output label csv will be stored one directory up PDF_LABEL_INPUT_PATH

## Labeling Environment

<img src="./documentation/labeling_env.png" width="500" />
<img src="./documentation/keyboard_usage.jpg" />

## Structure

* data: PDF data files and generated region ground-truth
* main:
  * input: converted PDF input files
  * output: coordinate-based output of labeling
  * main.py: labeling UI
  * remove_output.sh: clean labels of input data
* util:
  * constants: paths
  * StorageUtil: store/load functionalities
  
  
