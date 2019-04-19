Collecting and analyzing data
Tools used: PITClipse
Calculating Mutation Score: The mutation score is defined as the percentage of killed mutants with the total number of mutants.
·	Mutation Score = (Killed Mutants / Total number of Mutants) * 100

Steps executed to generate a mutation score in PITClipse for all test suites:
1) Install PITClipse plugin in Eclipse
2) Run maven build project for PIT testing
3) Mutant generation and execution 
4) Get Mutation Score from PIT Report generated in PITClipse console.

Steps executed to generate a mutation score in Command Line Interface for all test suites:
1) Add Pitest plugin in pom.xml file of project.<br>
Configuration<br>

< plugin><br>
    < groupId>org.pitest</groupId><br>
    < artifactId>pitest-maven</artifactId><br>
    < version>LATEST</version><br>
 </ plugin><br>
2) Run “maven clean install”<br>
3) Run “mvn org.pitest:pitest-maven:mutationCoverage”<br>
4) Mutant generation and execution<br>
5) Get Mutation Score from PIT Report generated in target folder of project.<br>
