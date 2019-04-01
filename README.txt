## System requirements:
- Build-time: Java 8 JDK, Apache Maven
- Runtime: Java 8 JRE or higher

##Download and Installation Instructions. 

	-Using a web browser navigate to:

	https://github.com/optimusmoose/XNet 

	-Download the repository by clicking the "Clone or Download" Button, and selecting "Download Zip" 
	-Ensure that "Save File" radio button is checked, then click "OK"
	-Move the downloaded ZIP "XNet-master.zip" to wherever you would like the project to be located, then right click and extract. 
	-Xnet should now be ready to run. 


##Testing and using Xnet

	-Open a unix terminal in the target directory. This is located in the root directory of the project, XNet-master. 
	-Type in the following to run XNet:

	java -jar xnet.1.0.jar good_example.csv

	-Xnet will load in the file "good_example.csv", perform trace clustering, and then write to a file called "output.csv" in the same directory. 
	-If you would like to run clustering on your own file, replace the provided example file with your own following the formatting instructions described Below.

##Data Formatting

	-To use the provided .jar file, Xnet requires a .csv input with columns "m/z, RT, intensity, traceID, envelopeID"
	-An example of this can be seen in good_example.csv.
	-Each row must correspond to a point with m/z, RT, intensity, and traceID already resolved. Envelope ID is a required field, but should be filled with 0's for the input file.
	-The output is the same format as the input, but will have EnvelopeID filled out with the results of the clustering.

## Build procedure
- You do not have to rebuild the package unless you modify the source code.
- If you want to make code changes, you can do so by changing the code and rebuilding.
- To rebuild, run `mvn package` from within the project root directory