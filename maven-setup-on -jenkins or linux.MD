Maven is a Java based tool, so the very first requirement is to have JDK java-1.7 or above installed on your machine.
```sh
yum list | grep java-1.8
java -version
```

Set the JAVA_HOME environment variable on <.bash_profile> to point to the base directory location where Java is installed on your machine. For example 
```sh
# go to .bashrc file and set env variable
export JAVA_HOME=/usr/local/current-java
export PATH=$PATH:$JAVA_HOME/bin/
```

Download Maven from https://maven.apache.org/download.cgi
```sh 
apache-maven-3.3.1-bin.tar.gz      lates 
```

Add M2_HOME, M2, MAVEN_OPTS to environment variables. in .bash_profile
```sh
export M2_HOME=/usr/local/apache-maven-3.3.1
export M2=$M2_HOME/bin
PATH=$PATH:$JAVA_HOME:M2_HOME:$M2:$HOME/bin
```
Relaunch the terminal or execute source .profile to apply the changes

