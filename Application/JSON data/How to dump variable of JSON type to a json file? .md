# Module
json

# Import
import json

# Use
Simply use json.dump method to dump a variable with json type in the specified file.

# Example
## Example Code
import json

dictionary = {
	"name": "sathiyajith",
	"rollno": 56,
	"cgpa": 8.6,
	"phonenumber": "9976770500"
}

with open("sample.text", "w") as outfile:
	json.dump(dictionary, outfile)

## Exampple intro
It will output nothing.
But it will create a new text file named "sample.text".
In the text file, the data is

{"name": "sathiyajith", "rollno": 56, "cgpa": 8.6, "phonenumber": "9976770500"}

## Example Output
