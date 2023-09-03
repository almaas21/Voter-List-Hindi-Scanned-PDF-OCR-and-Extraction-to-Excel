# Voter-List-Hindi-Scanned-PDF-OCR-and-Extraction-to-Excel
I have used voter list.pdf which contains voter data available on https://eci.gov.in/electoral-roll/link-to-pdf-e-roll/. You can choose any state and view any pdf from any vidhansabha and download the bhag/part which you want to prcoess.
I used https://www.i2pdf.com/enhance-scanned-pdf to enhance the pdf as The PDFs are scanned images. Use 300 dpi in settings and reduce saturation appropriately. Pages with Deleted as watermark won't render correct OCR.
This python code uses Tesseract OCR so that must be installed before using this. The output is an excel file with columns: {Name, Father/Husband Name, House Number, Age, and Gender} along with images extracted from the pdf
Some minor manual data cleaning/ manipulation will be needed in most cases. OCR is very bad with EPIC Number or Voter ID card number so that is not included.
If anyone is capable of tuning Tesseract Settings to use with hin+eng and create a fork out of this he is most welcome.
