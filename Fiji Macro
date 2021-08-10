// open and load the mast cell image
selectWindow("Aufnahme-161029-0017.jpg");

// convert the image into 8-bit format
run("8-bit");

// run("Threshold...");
// setThreshold(199, 255);
setAutoThreshold("Default dark no-reset");

// convert the image into mask
run("Convert to Mask");
run("Close");

// fill all the holes either using fill holes method or can be manually adjusted using erosion and dilation function
run("Fill Holes");

// run the watershed function to seperate the cells from each other by marking boundaries
run("Watershed");

// run analyze particles function to get the results and it can be exported into excel spreadsheet
run("Analyze Particles...", "size=60 circularity=0.5-1.00 display exclude add");
run("Close");

//save the results 
saveAs("Results", "/Users/nagarjunakki/Desktop/master thesis/proffessor images/Results_new.csv");
