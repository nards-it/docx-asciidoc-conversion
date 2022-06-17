# docx-asciidoc-conversion

Repository for internal working with Epsilon Italia on develop the algorithm to support translations from INSPIRE specifications .docx documents format to asciidoc format specification.  

## Supported file formats

Script supports actually three different file format specifications:

* **metadata** converting the unique metadata document
* **services** converting a services document
* **data** converting a data document

## Working process

In order to release a new adoc conversion you have to:

1. Create a new folder with the name of the document to convert (according to the order provided in [this table](./docx/README.md))

        mkdir my_example_data_specifications_EX

2. Copy the Microsoft Word document into the new folder from the [docx](./docx) folder 

3. Convert the Microsoft Word document into the last .docx format

        From Microsoft Word document: File -> Informations -> Convert

4. Launch the preliminary folder script from main folder

        .\pandoc-folder.bat .\my_example_data_specifications_EX

5. Launch the conversion script from main folder, using the correct data format between **metadata**, **services** and **data**

        .\pandoc-postpy.bat .\my_example_data_specifications_EX data

6. Check the result document, named as folder (ex. my_example_data_specifications_EX data.adoc) to verify if script need fixes

7. Fix script and re-launch the conversion script until conversion is ok
