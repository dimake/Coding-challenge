Import all dependencies

1) Creating a function to get all the files:
    Input of 1 or 2 only, for csv files to be sampled from each folder
    Loop over all files and assign the path to each one
    Select only non-empty folders and within them, filter only csv files
    Getting full path of the non-empty csv file
    Sample based on the input number provided
    Iterating over the samples to get the full path and append the result in a df list

2) Looping over each csv from the previous function to:
    Generate a random number from index 0 to last one minus 29
    Getting the price column and match the index from xl file
    Substracting 2 and adding 28 from random number to get 30 values and return that array

3) From previous obtained array:
    Calculating the mean price and standard deviation and setting the threshold at 2, according to the doc
    Using the z-score method to find and return the outliers

4) Export csv
    Reading previous df and outlier and if outliers found, then build headers and populate with values
    Getting the filename and add a "new" in front of it
    Displaying what csvs had been saved
