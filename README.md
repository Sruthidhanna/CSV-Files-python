# Reading and Writing CSV Files

This Python project program investigated using a list to represent a row of a CSV file. We will use dictionaries to represent a row of a CSV file.  This dictionaries will then be organized using either a list or a dictionary.

-------

# Project description

The project consists of multiple problems. Each problem will utilize functions you wrote for the previous problems. You can also download all of the files used when testing your code as a zip file.

### Problem 1: Reading the field names from a CSV file
First, you will write a function called read_csv_fieldnames that takes the name of a CSV file and returns a list of the field names from that file. This function assumes that the first row of the CSV file contains the field names. As CSV files can use different separator characters and quote characters, this function takes those characters as input and uses them to properly parse the CSV file.

### Problem 2: Reading a CSV file into a list of dictionaries
Next, you will write a function called read_csv_as_list_dict that takes the name of a CSV file and returns the data within the file as a list of dictionaries. Each item in the list corresponds to a row in the CSV file. The dictionaries within the list map the field names to the column values for that row.  As CSV files can use different separator characters and quote characters, this function takes those characters as input and uses them to properly parse the CSV file.

### Problem 3: Reading a CSV file into a dictionary of dictionaries
Next, you will write a function called 
read_csv_as_nested_dict that takes the name of a CSV file and returns the data within the file as a dictionary of dictionaries. Each key-value pair in the outer dictionary corresponds to a row in the CSV file. The keys in that dictionary are the values of a header column in the table. The function takes the name of that header column as the input keyfield.  If a key appears multiple times in column corresponding to keyfield, the last row containing the key is used to create the dictionary used as the corresponding value.The inner dictionaries within the outer dictionary map the field names to the column values for that row.  As CSV files can use different separator characters and quote characters, this function takes those characters as input and uses them to properly parse the CSV file. Note that the key-value pair for keyfield should be in the inner dictionaries, even though its value is used as the key in the outer dictionary.

### Problem 4: Writing a list of dictionaries to a CSV file
Finally, you will write a function called write_csv_from_list_dict. This function takes a table structured as a list of dictionaries (as if read by 
read_csv_as_list_dict) and writes it to the file named by the filename input. The function also takes a list of field names, fieldnames, as input in order to make sure the fields appear in the appropriate order (as specified by the order of the list fieldnames) in the CSV file. The function also takes a separator character and a quote character that should be used when writing the file. All non-numeric fields should be quoted using the specified quote character.


# Features
1. Read CSV field names with custom separators and quotes.
2. Load CSV data as a list of dictionaries (read_csv_as_list_dict).
3. Load CSV data as a nested dictionary keyed by any column (read_csv_as_nested_dict).
4. Write list-of-dicts data back to CSV with custom formatting (write_csv_from_list_dict).
5. Handles duplicate keys (last one wins).
6. Automatically quotes non-numeric fields.
7.Built using Python’s standard csv module.

-----



