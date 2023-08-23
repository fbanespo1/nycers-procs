# Extract Text from Image and Generate Word Document

## Overview

This is a Streamlit application that allows users to upload an image, extracts text from the image using Azure Computer Vision, and then generates a Word document with the extracted text. The Word document is formatted with a step-by-step guide based on the extracted text, and it also includes the uploaded image as a screenshot. The application is built by Tony Esposito.

## Features

- Upload an image in PNG, JPEG, or JPG format.
- Extract text from the image using Azure Computer Vision.
- Generate a Word document that includes the extracted text and the image.
- Download the generated Word document.

## Prerequisites

- Python 3.x
- Streamlit
- Azure Cognitive Services SDK
- PIL (Pillow)
- python-docx
- OpenAI Python package

## Setup and Installation

1. Clone the repository:

    ```bash
    git clone <repository-url>
    ```

2. Navigate to the project directory:

    ```bash
    cd <project-directory>
    ```

3. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

4. Set up environment variables:

    - `AZURE_SUBSCRIPTION_KEY`: Your Azure subscription key for Computer Vision.
    - `AZURE_ENDPOINT`: Endpoint URL for Azure Computer Vision.
    - `OPENAI_API_KEY`: Your OpenAI API key.

    You can set these variables in a `.env` file or directly in your system's environment variables.

5. Run the Streamlit application:

    ```bash
    streamlit run <your-script-name>.py
    ```

## Usage

1. Open the Streamlit application in your web browser.
2. Upload an image using the file uploader.
3. The application will display the text extracted from the image.
4. A Word document will be generated, and a download button will appear.
5. Click the download button to get the generated Word document.

## Code Structure

- `generate_word_document(text, image_path, doc_path)`: Function to generate the Word document.
- Streamlit UI: Code for rendering the Streamlit interface.
- Azure Computer Vision: Code for extracting text from images.
- Word Document Generation: Code for creating and saving the Word document.

## Contributions

Built by Tony Esposito.
