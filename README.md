# report_ISW2_testing

Repository di consegna per il modulo software testing di ISPW2.

### Per eseguire la build e generare i report di Jacoco eseguire:
>mvn clean org.jacoco:jacoco-maven-plugin:prepare-agent package

### Per generare i report di pit utilizzare il comando:
>mvn -DwithHistory org.pitest:pitest-maven:mutationCoverage surefire:test -Ppit

