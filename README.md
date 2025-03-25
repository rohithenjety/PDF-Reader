## Project Structure and Key Files

### 1. `PdfReaderController.java`
This is the main controller file that defines the API endpoints. It handles:
- Uploading and processing PDF files.
- Extracting text using Apache PDFBox or Tesseract OCR.
- Sending the extracted text to OpenAI's API for parsing.
- Returning structured data (name, email, opening balance, closing balance) as a JSON response.

### 2. `PDFBox` and `Tesseract OCR`
- **PDFBox**: Extracts text from machine-readable PDFs.
- **Tesseract OCR**: Extracts text from scanned PDFs or images using optical character recognition.

### 3. `pom.xml`
The Maven configuration file that:
- Manages dependencies (e.g., Spring Boot, PDFBox, Tesseract, OkHttp).
- Configures the build process and packages the project as a JAR file.
