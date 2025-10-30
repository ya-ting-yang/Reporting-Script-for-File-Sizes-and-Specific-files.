README — Wine Data Filtering Script

### Author: Ya-Ting Yang
### Purpose: Create a Python script in a single file that will traverse the filesystem finding the largest files in a path..

# Description
This Python script automatically searches through a given directory (including all its subdirectories) to locate all files with the .ipynb extension (Jupyter Notebook files).
For each notebook found, the script prints the file path and its size in bytes (or other units if modified).
It is useful for managing large projects containing multiple Jupyter notebooks, helping users quickly identify, locate, or audit files.

Use different options in the script for reporting, like:
No more than 20 files
Files larger  than a specific size in megabytes
Find files that end in .ipynb 

# Workflow
1. Start Search – The script begins scanning from the specified root directory ('.' by default, meaning the current directory).
2. Directory Traversal – Uses os.walk() to recursively go through all subdirectories and files.
3. File Detection – Checks if each file ends with .ipynb.
4. Size Retrieval – Gets each file’s size using os.path.getsize().
5. Output – Prints the file path and its corresponding size in bytes.

# Output Files
1. No new files are created.
2. The script outputs information directly to the terminal (stdout).
