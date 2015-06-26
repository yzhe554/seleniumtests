# seleniumtests

# For MacOs

## Install maven on your mac

[Install maven with brew](http://brewformulas.org/Maven)

```
brew update
brew install maven
```

## Install maven plugin on Eclipse

[Maven Eclipse plugin installation step by step](http://stackoverflow.com/questions/8620127/maven-in-eclipse-step-by-step-installation)

## Download chromedriver

[ChromeDriver Download](http://chromedriver.storage.googleapis.com/index.html?path=2.16/)
```
For MacOs users
Download chromedriver_mac32.zip	2015-06-08 13:29:32	3.34MB	
```

## Configure your project
```
Edit codes in **/seleniumtests/src/test/java/au/com/vclass/init/InitAndFunction.java
public final String web = "http://192.168.1.25/wwork7_/WebApp/web/cviewer5.html";
public final String chromeDriverPath = "/Users/zhengyu/Documents/JavaJar/chromedriver"; 
```

## Edit test suite
Edit files under `**/seleniumtests/src/test/java/au/com/vclass/automationtests` to change test scope

Here's an idea: why don't we take `SuperiorProject` and turn it into `**Reasonable**Project`.

## Run tests with command line
Navigate to project folder and run `mvn clean test`

## Check Reports
Reprt files are under the project folder with the name `CombineTest*.html`
