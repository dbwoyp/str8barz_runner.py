import argparse

# Initialize the parser
parser = argparse.ArgumentParser(description='Process some command line arguments.')

# Adding optional argument
parser.add_argument('--arg1', type=str, help='An optional string argument')
# Adding required argument
parser.add_argument('--arg2', type=int, required=True, help='A required integer argument')

# Parse the arguments
args = parser.parse_args()

# Accessing the arguments
print('arg1:', args.arg1)
print('arg2:', args.arg2)
