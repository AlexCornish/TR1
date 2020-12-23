# Statcan Computer Assisted Matching Program
## Exact Word
### What does it do?
- In this page, you can search for all instances of an exact word in one of the two datasets available. 
    - You can search in either the BLS (U.S Bureau of Labour Services) or the NAPCS (North American Product Classificiation System)
- NAPCS Filtering
    - These textboxes will only have any effect if you are searching in the NAPCS dataset. 
        - The length of NAPCS codes that you can search are (3,5,6,7).
        - The first digits of NAPCS codes that you can search are (1,2,3,4,5,6,7,8)
### What should the input be?
- Select one of the two dataset names.
- Enter an exact word to search for in the chosen dataset.
    - Capitalisation of the exact word being searched doesn't matter.
- If you chose NAPCS:
    - Length Code: Enter a number as specified above.
    - First Digit: Enter a number as specified above.
## Code Search
### What does it do?
- In this page, you can search for a code and the result will be the N most similar codes in the opposite dataset. 
    - You can search in either the BLS (U.S Bureau of Labour Services) or the NAPCS (North American Product Classificiation System)
### What should the input be?
- Select one of the two dataset names.
- Enter either a BLS or NAPCS code.
- Enter an integer value greater than 0 for the number of nearest matches you would like to see.
## String Parser
### What does it do?
- In this page, you can enter a string containing multiple words and symbols that emphasize or deemphasize those words. 
### What should the input be?
- The String Parser
    - Strings without symbols such as "cattle farming" .
    - In order to emphasize a word, add + or ++ in directly in front of the word. 
        - Example: "+musical ++instruments" will emphasize instruments of the musical kind.
    - To deemphasize a word, add - or -- in directly in front of the word.
        - Example: "++cattle cows -meat --manufacturing" will deemphasize meat and manufacturing, but still look for cattle and cows. 
## Correlator
### What does it do?
- The correlator uses RMPI (Raw Material Price Index) and IPPI (Industrial Product Price Index) data, takes a code the user passes in, and performs a correlation of that code and returns the 20 most closely correlated rows from the two datasets. 
### What should the input be?
- The input should be a RMPI or IPPI code that exists from January 2010 onwards. 
## Documentation of Technical Aspects