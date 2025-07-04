# Task 1
try:
    with open("sample.txt", "r") as file:
        print("Reading file content:")
        for index, line in enumerate(file, start=1):
            print(f"Line {index}: {line.strip()}")
except FileNotFoundError:
    print("Error: The file 'sample.txt' was not found.")

  # Task 2
    
