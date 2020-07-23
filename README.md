# Open Document Labeling
A tool for labeling document regions as a basis for various region detection task.
The tool is based on the work of https://github.com/Cartucho/OpenLabeling.

IN PROGRESS

## How-to

* Input documents in data/custom/pdfs (or change PDF_LABEL_INPUT_PATH in utils/constants accordingly)
* Run main/main.py
* Label documents
* The output label csv will be stored one directory up PDF_LABEL_INPUT_PATH

## Labeling Environment

![keyboard](https://github.com/MBAigner/Open-Document-Labeling/blob/master/keyboard_usage.jpg)


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
  
  
