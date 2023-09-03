# Voter-List-Hindi-Scanned-PDF-OCR-and-Extraction-to-Excel
I have used pdf downloaded from the official government voter electoral roll https://eci.gov.in/electoral-roll/link-to-pdf-e-roll/. From the website, you can choose any state and view any pdf from any VidhanSabha, and download the bhag/part that you want to process.
Replace pdf_file_path = 'Voter List.pdf' # change file name to what you want to replace with.

I used https://www.i2pdf.com/enhance-scanned-pdf to enhance the PDFs as they aren't of very high resolution. Use 300 dpi in settings and reduce saturation appropriately. Pages with Deleted as a watermark won't render correct OCR.

This Python code uses Tesseract OCR so that must be installed before using this. The output is an Excel file with columns: {Name, Father/Husband Name, House Number, Age, and Gender} along with images extracted from the pdf.

Some minor manual data cleaning/ manipulation will be needed in most cases. OCR is unable to extract correctly EPIC Numbers or Voter ID card numbers so that is not included.
If anyone is capable of tuning Tesseract Settings to use with language "hin+eng" and create a fork out of this he is most welcome.
