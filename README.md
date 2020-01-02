# Kattis Command Line Tools
Helpful utilities to make working with [open.kattis.com](open.kattis.com) easier. 

This command line interface automates common actions to reduce problem setup, 
testing, and submission times by more than 50%!

## Usage

**Note:** `<problem_id>` refers to a valid Kattis Problem ID. Problem IDs can be 
found in the top-right corner of a problem's description page.

`$ kattis new <problem_id>`  
Provisions a problem directory by downloading sample data, standardizing their 
filenames, and creating a default solution file.

`$ kattis test <problem_id>`  
Tests a Kattis problem (i.e. compares a solution file's outputs to the expected 
outputs given in a problem's sample data).

## Limitations

Kattis problems' sample data aren't standardized, which makes them difficult to 
generalize. Therefore, the following limitations apply:

- Some problems, such as those related to machine learning, handle sample data 
differently. These problems' data must be downloaded manually.
- Some problems' sample data might use unique file extensions or naming 
conventions, which means that this CLI will be unable to perform automated testing.
