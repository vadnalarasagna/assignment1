def print_lines_in_reverse(file_path):
    try:
        # Open the file in read mode
        with open(file_path, 'r') as file:
            # Read all lines from the file
            lines = file.readlines()

            # Print each line in reverse order
            for line in reversed(lines):
                # Strip newline characters and print the reversed line
                print(line.rstrip()[::-1])

    except FileNotFoundError:
        print(f"File not found: {file_path}")

# Example usage: Replace 'your_file.txt' with the path to your file
print_lines_in_reverse('your_file.txt')
