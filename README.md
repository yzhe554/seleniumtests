### Run with dataProvider
`http://www.mkyong.com/unittest/testng-tutorial-6-parameterized-test/`
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
Report files are under the project folder with the name `CombineTest*.html`

## Maven commands
<ol>
<li>mvn test</li>
<pre>
Run All the tests
</pre>
<li>mvn mvn -Dtest=TestCircle test</li>
<pre>
Specify a test class(Change TestCircle to the class name, for example, CombineTest.java, just use CombineTest) to run
</pre>
<li>mvn mvn -Dtest=TestCircle#xyz test</li>
<pre>
Run a specified test method in a class. Change xyz to the method name
</pre>
</ol>

## Method query
| Description  | command para | ClassName/MethodName |
| :------------ |:---------------:| :-----|
| ToolBar Test      | CombineTest | ClassName |
| SignIn/Off Test     | SignInTest        |   ClassName |
| Pen thickness Test | CombineTest#penThickness       | MethodName   |
| Pen color Test | CombineTest#penColor       | MethodName   |
| Page Navigation Test | CombineTest#pageNavigation       | MethodName   |
| Zoom and Scale Test | CombineTest#zoomAndScale       | MethodName   |
| Signin with valid info Test | SignInTest#signInWithValidInfo       | MethodName   |
| Signin witn invalid info Test | SignInTest#signInWithInvalidInfo       | MethodName   |
