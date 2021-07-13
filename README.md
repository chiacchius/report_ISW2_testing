# report_ISW2_testing

Repository di consegna per il modulo software testing di ISPW2.

Travis Bookkeeper: https://travis-ci.com/github/chiacchius/bookkeeper
Sonar Bookkeeper: https://sonarcloud.io/dashboard?id=chiacchius%3Aorg.apache.bookkeeper%3Abookkeeper

Travis Zookeeper: https://travis-ci.com/github/chiacchius/zookeeper
Sonar Zookeeper: https://sonarcloud.io/dashboard?id=chiacchius%3Aorg.apache.zookeeper%3Aparent

Link cartella classi di test JCS 
- https://github.com/chiacchius/jcs/tree/main/src/test/java/it/uniroma2/dicii/isw2/jcs/paramTests  


Link cartelle classi di test BOOKKEEPER  
- BookkeeperAdmin: https://github.com/chiacchius/bookkeeper/tree/master/bookkeeper-server/src/test/java/org/apache/bookkeeper/client/bookkeeperAdminTest
- LedgerHandle : https://github.com/chiacchius/bookkeeper/tree/master/bookkeeper-server/src/test/java/org/apache/bookkeeper/client/ledgerHandleTest

Link cartelle classi di test ZOOKEEPER  
- Zookeeper : https://github.com/chiacchius/zookeeper/tree/master/zookeeper-server/src/test/java/org/apache/zookeeper/zookeeperTest
- ObserverMaster : https://github.com/chiacchius/zookeeper/tree/master/zookeeper-server/src/test/java/org/apache/zookeeper/observerMasterTest

### Per eseguire la build e generare i report di Jacoco eseguire:
>mvn clean org.jacoco:jacoco-maven-plugin:prepare-agent verify

### Per generare i report di pit utilizzare il comando:
>mvn -DwithHistory org.pitest:pitest-maven:mutationCoverage surefire:test -Ppit

