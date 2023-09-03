# Voter-List-Hindi-Scanned-PDF-OCR-and-Extraction-to-Excel

I have been working on a project where I needed to extract data from scanned PDFs of voter lists in Hindi. To get the PDFs, I visited the official government voter electoral roll website at https://eci.gov.in/electoral-roll/link-to-pdf-e-roll/. This website allows you to choose any state, view PDFs from different Vidhan Sabhas, and download the specific section (bhag/part) you want to process.

To prepare the scanned PDFs for extraction, I found a useful tool called https://www.i2pdf.com/enhance-scanned-pdf. The PDFs I downloaded weren't of very high resolution, so I used this tool with 300 dpi settings and adjusted saturation appropriately. It's important to note that pages with a watermark saying "Deleted" may not produce accurate OCR results.

For the OCR part of my project, I used Tesseract OCR. Before using this code, make sure you have Tesseract installed on your system.

The output of my code is an Excel file with specific columns: Name, Father/Husband Name, House Number, Age, and Gender. I also made sure to extract images from the PDFs.

However, I should mention that some manual data cleaning and manipulation may be needed for most cases. Unfortunately, OCR is unable to correctly extract EPIC Numbers or Voter ID card numbers, so I decided not to include them in the output.

If you're interested in improving the code and tuning Tesseract settings to work with the "hin+eng" language, please feel free to create a fork of this project. Your contributions would be greatly appreciated!
