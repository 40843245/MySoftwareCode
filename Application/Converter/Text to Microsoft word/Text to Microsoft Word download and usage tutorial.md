
# Module

# Install

step 1: 
In the terminal, simply type
pip install aspose-words

# Import
Type such following line in your IDE.
import aspose.words as aw

# Use
step 1:
Create an object for the blank document.
Type such following line in your IDE.
doc = aw.Document()

step 2:
To create a document builder to add content to the document.
builder = aw.DocumentBuilder(doc)

step 3:
Then you can write or modify the document.
More instruction about modify the document, 
please see the following section or see the below link.
https://pypi.org/project/aspose-words/

step 4:
Before closing, don't forget saving the document.
To save the document, use the save method.

Type such following line in your IDE.
doc.save("output.docx")

To Write a new paragraph in the document with the text "Hello World!".
builder.writeln("Hello, World!")

# Example
## Example Code
import aspose.words as aw

doc = aw.Document()

builder = aw.DocumentBuilder(doc)

builder.writeln("Hello, World!")

doc.save("output.docx")

## Example intro
The file output.docx will be created. 
Nothing will be outputted in the example code.

## Example Output
