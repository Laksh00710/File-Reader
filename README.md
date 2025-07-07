# File-Reader
def read_file(filepath):
    try:
        with open(filepath, 'r') as file:
            content = file.read()
        print(content)
    except FileNotFoundError:
        print(f"File not found: {filepath}")

if __name__ == "__main__":
    path = input("Enter file path: ")
    read_file(path)
