# OCR and Translation Web App

This project uses Tesseract.js for OCR (Optical Character Recognition) to recognize Japanese text from uploaded images. It then translates the recognized text using Microsoft's Translator Text API via RapidAPI.

## Live Demo

You can test the live version of the app [here](http://shark.tewi.club/ocr/translate.html).

## How To Install

Clone the repository:
    ```bash
    git clone https://github.com/0xOptimizer/simple-ocr-translate.git
    ```

Open `translate.html` in your web browser.

## Features

- Drag and Drop functionality for image upload.
- OCR using Tesseract.js (optimized for Japanese text).
- Translation using Microsoft's Translator Text API via RapidAPI.
- Bootstrap 5 for UI components.

## How To Change Language for OCR

Locate the following line in your JavaScript code:

    ```javascript
    Tesseract.recognize(
      file,
      'jpn',
    ```

Replace `'jpn'` with the language code of your choice (e.g., `'eng'` for English, `'deu'` for German).

## How To Change Language for Translation

Update the `data` field in the AJAX settings:

    ```javascript
    data: JSON.stringify([{"Text": text, "To": "en"}])
    ```
    Change `"To": "en"` to your desired language code.

## License

This project is open-source, feel free to use and modify.

## Issues

For any issues, please create a new issue [here](https://github.com/0xOptimizer/simple-ocr-translate/issues).
