# Open Document Labeling

With Open Document Labeling, we provide a tool for the annotation of rectangular document regions for various document region detection and classification tasks.
The process of labeling regions is supported with a graphical user interface.

## How-to

* Input documents used for labeling in ```data/custom/pdfs/```
* Run ```main/main.py```
* Label documents, as described in the next section
* The output label csv will be stored one directory in ```data/custom/```

## Labeling Environment

<img src="./documentation/labeling_env.png" width="500" />
<img src="./documentation/keyboard_usage.jpg" />

## Project Structure

* ```data```: PDF data files and generated region ground-truth
* ```main```:
  * ```input```: converted PDF input files
  * ```output```: coordinate-based output of labeling
  * ```main.py```: labeling UI
  * ```remove_output.sh```: clean labels of input data
  * ```class_list.txt```: list of region classes which can then be used for labeling
* ```util```:
  * ```constants```: paths to input, output and ground-truth data, supported file types
  * ```StorageUtil```: store/load functionalities
  

## Acknowledgements

* The tool is based on the work of https://github.com/Cartucho/OpenLabeling and adapted for a labeling of PDF documents.
* Example PDFs are obtained from the ICDAR Table Recognition Challenge 2013 https://roundtrippdf.com/en/data-extraction/pdf-table-recognition-dataset/.
