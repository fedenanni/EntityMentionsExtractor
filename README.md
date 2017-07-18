Instruction For "EntityLinkingExtraction.jar"


This program is developed with JDK 8u102 by Eclipse Java EE IDE. The whole program is implemented 100% by Java and does not need any third-party library. Thus, it can be executed in any platform with Java Runtime Environment (JRE) 8.102 or higher version. 

JVM Parameters:
-Xms: The initial and minimum Java heap size.
-Xmx: The maximum Java heap size.

Program Parameters:
args[0]: file path of index file; set "-1" for wikia or no index file. 
args[1]: type of analyzing index file: 1 - not split and Serial; 2 - split and parallel; -1 for no index. 
args[2]: file path of Wiki content XML file. 
args[3]: type of analyzing index file: 1 - not split and Serial; 2 - split and parallel; 3 - load whole content file into RAM and parallel, this option uses vast of RAM space to "exchange" time, not recommend for computers with limited RAM space. 
args[4]: folder path of splitted Wiki files. All files in this folder will be deleted before splitting. 
args[5]: folder path for output file. All files in this folder will be deleted before splitting.
args[6]: default char buffer size for reading and writing file, Unit: MB. 
args[7]: whether speed up program in reverting index and saving result? true or false. Using vast of RAM space to "exchange" time, not recommend for computers with limited RAM space.


Example:
java -Xms512G -Xmx650G -jar EntityLinkingExtraction.jar "./Input/en20161001/index.txt" "1" "./Input/en20161001/content.xml" "3" "./SplittedFiles" "./Output/en20161001" "200" "true"


If you have further problem, don't hesitate to contact me by E-Mail: zhaoyang868686@gmail.com. Have fun!


Yang Zhao

2016-10-13
Mannheim
Germany