# Kattis Command Line Tools
This **unofficial** command line interface makes writing **Python** solutions 
for [open.kattis.com](https://open.kattis.com/) easier by automating common tasks.

Reduce problem setup and testing times by more than 50%!

## Usage

**Note:** `<problem_id>` refers to a valid Kattis Problem ID. Problem IDs can be 
found in the top-right corner of a problem's description page on Kattis.

`$ kattis new <problem_id>`  
Provisions a problem directory by downloading sample data, standardizing their 
filenames, and opening an empty solution file in your text editor.

`$ kattis test <problem_id>`  
Tests a solution (i.e. naively compares a solution's outputs to the expected 
outputs given by the problem's sample data).

## Limitations

The diverse array of problems on Kattis introduces some limitations:

- Testing is naive (i.e. tests only pass if a solution's output exactly matches 
the expected output). Some Kattis problems have multiple correct answers, or 
accept values within a certain epsilon. These problems will need to be tested 
manually.

- Some problems, such as those related to machine learning, handle sample data 
differently and lack tests. These problems will need to be downloaded and tested 
manually.

- Some problems' sample data might use unique file extensions or naming
conventions, which means that they will need to be manually renamed in order for 
automated testing to work properly. 

The vast majority of problems should work fine, but if you notice any 
problematic problems, please open an issue!
