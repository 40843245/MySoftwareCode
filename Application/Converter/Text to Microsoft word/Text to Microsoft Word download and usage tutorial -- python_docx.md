# Module
python-docx

# Install
step 1: 
In the terminal, simply type
pip install python-docx

# Import
Type such following line in your IDE.

from docx import Document
from docx.shared import Inches

# Use
step 1:
## create a blank file.
To create an object for the blank document.
Just call the docx.Document method
Type such following line in your IDE.
doc = docx.Document()

## modifying the existing file.
To modifying the existing file.
Type such following line in your IDE.
doc = docx.Document('test.text')

step 2:
Then you can write or modify the document.
More instruction about modify the document, 
please see the following section or see the below link.
https://pypi.org/project/aspose-words/

step 3:
Before closing, don't forget saving the document.
To save the document, use the save method.

Type such following line in your IDE.
doc.save("output.docx")

# Example
## Example Code

from docx import Document

from docx.shared import Inches

document = Document()

document.add_heading('Document Title', 0)

p = document.add_paragraph('A plain paragraph having some ')

"""
This is a comment

p.add_run('bold').bold = True
p.add_run(' and some ')
p.add_run('italic.').italic = True

document.add_heading('Heading, level 1', level=1)
document.add_paragraph('Intense quote', style='Intense Quote')

document.add_paragraph(
    'first item in unordered list', style='List Bullet'
)
document.add_paragraph(
    'first item in ordered list', style='List Number'
)

document.add_picture('monty-truth.png', width=Inches(1.25))

records = (
    (3, '101', 'Spam'),
    (7, '422', 'Eggs'),
    (4, '631', 'Spam, spam, eggs, and spam')
)

table = document.add_table(rows=1, cols=3)
hdr_cells = table.rows[0].cells
hdr_cells[0].text = 'Qty'
hdr_cells[1].text = 'Id'
hdr_cells[2].text = 'Desc'
for qty, id, desc in records:
    row_cells = table.add_row().cells
    row_cells[0].text = str(qty)
    row_cells[1].text = id
    row_cells[2].text = desc
    
end of comment
"""

document.add_page_break()

document.save('demo.docx')

## Example intro
The file demo.docx will be created. 
Nothing will be outputted in the example code.

## Example Output
