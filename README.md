# Acoustic_liquid_handling
## For generating complex screens with an Echo liquid handler. Intended for advanced users with comfort using pandas.

While the Echo comes with softwares that can do simple, high throughput tasks like 1:1 transfer, pooling, etc, two tasks I've come across that aren't addressed is the pairwise combination of wells from a sourceplate as well as generating instructions from a list of genes. Provided are some notebooks (tempting to pack it up into a .exe but I like to have more control/oversight of my plates) I use to handle these two tasks.

Gene list based notebook is based on the siRNA Silencer Select library from Thermofisher. 
  To do gene list based instruction generation, simply change the path for 'gene_list' to direct it to your own list. Ensure your spreadsheet of genes has the genes in column 1 and use the appropriate column header - 'Gene/product'. Errors will arise if column names are different, so go cell by cell and compare with the pseudodependencies I've provided as examples.
  
Pairwise based notebook generates nonredundant pairwise combos of mimics (AA and AB is good but BA would already be covered by AB) and requires a spreadsheet of the mimics of interest.  To make this one work with your list, change the path to direct the call for 'df' to your spreadsheet of picked mimics. Like above, if you run into errors, check my example files here to make sure you have the information required in the spreadsheet for your picklist-library.
