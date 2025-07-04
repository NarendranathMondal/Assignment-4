# Task 1

def read_file(filename):
    try:
        with open(filename, 'r') as file:
            print("Reading file content:")
            for i, line in enumerate(file, start=1):
                print(f"Line {i}: {line.strip()}")
    except FileNotFoundError:
        print(f"Error: The file '{filename}' was not found.")
read_file("sample.txt")

# Task 2

c=input('Enter text to write to the file: ')
file=open('output.txt','w')
writing_file=file.write(c + '\n')
file.close()
print('Data successfully written to output.txt.')

b=input('\nEnter additional text to append: ')
file=open('output.txt','a')
appending_file=file.write(b)
file.close()
print('Data successfully appended.')

print('\nFinal content of output.txt: ')
file=open('output.txt','r')
reading_file=file.read()
print(reading_file)
file.close()
    
