The file `Disk Usage Script.ipynb` is a Jupyter Notebook that contains a Python script for analyzing the disk usage of a specified directory. The script calculates the total size of all files within the directory and its subdirectories, and then prints the total size in megabytes (MB).

### Key Components:
1. **Importing the `os` Module**:
   - The script starts by importing the `os` module, which provides functions for interacting with the operating system, particularly for file and directory operations.

2. **Function Definition**:
   - The `get_size` function is defined to recursively calculate the total size of all files in a given directory.
   - **Parameters**:
     - `path`: The path of the directory to be analyzed.
   - **Functionality**:
     - Initializes a variable `total_size` to zero.
     - Uses `os.walk` to iterate through the directory and its subdirectories.
     - For each file, it calculates the file size using `os.path.getsize` and adds it to `total_size`.
     - Returns the total size of all files in bytes.

3. **Calculating and Printing Disk Usage**:
   - The script sets the `directory` variable to the path of the directory to be analyzed.
   - Calls the `get_size` function to get the total size in bytes.
   - Converts the size from bytes to megabytes (MB) by dividing by \(1024 \times 1024\).
   - Prints the total size in MB with a formatted message.

### Example Output:
- The script prints the total size of the specified directory in MB, providing a quick overview of the disk usage for that directory.