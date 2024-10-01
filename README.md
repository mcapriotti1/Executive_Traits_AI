# Executives_Traits_AI

**Executives_Traits_AI** is a powerful repository designed to extract and analyze executive data using ChatGPT. While primarily focused on executive traits, the methodologies implemented in this repository can be adapted to any data type by updating the formatting. The framework leverages **Pyppeteer** for web automation, allowing for a seamless interaction with online platforms.

To utilize the features of this repository, please ensure that you have Chrome installed at the following path:  
`C:\Program Files\Google\Chrome\Application`.  
You will also need to run Chrome with remote debugging enabled using the command:  
`chrome --remote-debugging-port=9222`.

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

## Features

- **Data Extraction**: Efficiently extract data from Excel spreadsheets, making it accessible for further analysis.
- **Executive Traits Analysis**: Analyze and derive insights related to executive traits.
- **Web Automation**: Utilize Pyppeteer for automating web tasks and interactions.
- **Adaptability**: Easily adapt the repository for various data types with appropriate formatting adjustments.

## Summary of Sections

### Extracting Data

This section provides a framework for extracting data from Excel files. The specifics may vary based on the dataset you are using, but the outlined methods serve as a solid foundation for your data extraction needs.

### Image to Text

Convert images to text using `pytesseract`, enabling the transformation of visual data into a format that can be analyzed and processed.

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
