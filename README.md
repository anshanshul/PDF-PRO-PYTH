# PDF-PRO-PYTH

#importing required modules
import PyPDF2
#creating a pdf file object
pdfFileObj = open('proble.pdf', 'rb')
#creating a pdf reader obbject
pdfReader = PyPDF2.PdfFileReader(pdfFileObj)
#printing number of pages in pdf file
print(pdfReader.numPages)
#creating apage object
pageObj =pdfReader.getPage(0)
#extrting text from page
print(pageObj.extractText())
#closing the pdf file object
pdfFileObj.close()
