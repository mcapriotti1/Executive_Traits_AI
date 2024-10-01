# Executives_Traits_AI

**Executives_Traits_AI** is a  repository designed to extract and analyze data using ChatGPT. While the specific method is primarily focused on determining executive traits, the methodologies implemented in this repository can be adapted to any data type by updating the formatting. The process involves several key steps: extracting data from a spreadsheet, converting images to text, applying general text formatting, implementing specific formatting for GPT input, and finally running the files through ChatGPT before copying the output. The framework leverages **Pyppeteer** for web automation.

To utilize the features of this repository, please ensure that you have Chrome installed at the following path:  
`C:\Program Files\Google\Chrome\Application`.  
You will also need to run Chrome with remote debugging enabled using the command:  
`chrome --remote-debugging-port=9222`.

Also ensure that you leave the Chrome browser open otherwise Pyppeteer does not function properly. Also the data is quite compacted, but if somehow there is too much data ChatGPT will stop responding (about 30 messages in 1 hour), in which case you will have to split the data up, or simply add your own delays.

## Required Libraries

To run this project, make sure to install the following libraries:

- `openpyxl`
- `requests`
- `PIL` (Pillow)
- `tiktoken`
- `asyncio`
- `nest_asyncio`
- `pyppeteer`
- `pyperclip`
- `pandas`
- `re`

## Summary of Sections

### Extracting Data

This section provides a framework for extracting data from Excel files. The specifics may vary based on the dataset you are using, but the outlined methods serve as a solid foundation for your data extraction needs.

### Image to Text

Convert images to text using `pytesseract` Optical Character Recognition (OCR), enabling the transformation of visual data into a format that can be analyzed and processed.

### File Formatting

Focuses on combining and structuring files, particularly tailored for the dataset being used. This section ensures your files are in the correct format for further processing.

### GPT Formatting

Outlines the necessary formatting for interfacing with ChatGPT. Adhere to the token limits established by ChatGPT, and customize messages using the `tiktoken` library to suit your specific data requirements.

### Running Through GPT

Employs **Pyppeteer** and **Asyncio** to process files through ChatGPT sequentially. This section also includes mechanisms for copying the outputs using XPath, ensuring that data is captured accurately.

### Delete All Files

A convenient function to reset the repository and prepare it for a new data file. This feature allows you to cleanly manage your workspace.

## Future Enhancements

Looking ahead, there are plans to enhance the functionality of this repository to process multiple files concurrently. For now, the system allows for customization, enabling users to run one file at a time while maintaining flexibility in their data analysis workflow.
