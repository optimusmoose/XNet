## System requirements:
- Build-time: Java 8 JDK, Apache Maven
- Runtime: Java 8 JRE or higher

## Build procedure
- Run `mvn package` from within the project root directory

## Testing
- Place ground truth CSVs into target folder (same folder as jar) 
- in unix terminal use the command "java -jar xnet-1.0.jar <your-csv> 
- The csv will be read in, xnet will cluster the provided traces, and output to a csv called output.txt
- Test files have bene provided for your benefit and as an example for the required input. 
