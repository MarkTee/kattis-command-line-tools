# Kattis Command Line Tools
This command line interface makes writing Python solutions for 
[open.kattis.com](open.kattis.com) easier.

This **unofficial** command line interface automates common actions to reduce 
problem setup and testing times by more than 50%!

## Usage

**Note:** `<problem_id>` refers to a valid Kattis Problem ID. Problem IDs can be 
found in the top-right corner of a problem's description page on 
[Kattis](open.kattis.com).

`$ kattis new <problem_id>`  
Provisions a problem directory by downloading sample data, standardizing their 
filenames, and creating an empty solution file.

`$ kattis test <problem_id>`  
Tests a solution (i.e. compares its outputs to the expected outputs given by a 
problem's sample data).

## Limitations

Kattis problems' sample data aren't standardized, which makes them difficult to 
generalize. Therefore, the following limitations apply:

- Some problems, such as those related to machine learning, handle sample data 
differently. These problems' data will need to be downloaded manually.
- Some problems' sample data might use unique file extensions or naming 
conventions, which means that this CLI will be unable to perform automated 
testing.

If you notice any problematic problems, please open an issue!
