# pingu2
package com.example; 
import com.google.gson.Gson; 
public class Main 
{ 
    public static void main(String args[]) 
    { 
        Gson gson= new Gson(); 
        String json= gson.toJson(new Person("john",30) ); 
        System.out.println(json); 
    } 
} 
class Person 
{ 
    private String name; 
    private int age; 
    public Person(String name, int age) 
    { 
        this.name=name; 
        this.age=age; 
    }








    import org.openqa.selenium.WebDriver; 
import org.openqa.selenium.chrome.ChromeDriver; 
import org.testng.Assert; 
import org.testng.annotations.AfterTest; 
import org.testng.annotations.BeforeTest; 
import org.testng.annotations.Test; 
import static org.testng.Assert.assertTrue; 
public class WebPageTest 
{ 
    private static WebDriver driver; 
    @BeforeTest 
    public void openBrowser() throws InterruptedException 
    { 
        driver = new ChromeDriver(); 
        driver.manage().window().maximize(); 
        Thread.sleep(2000); 
        driver.get("https://sarvarbegum-coder.github.io/LAB_1/"); 
    } 
    @Test 
    public void titleValidationTest() 
    { 
        String actualTitle = driver.getTitle(); 
        String expectedTitle = "My simple website"; 
        Assert.assertEquals(actualTitle, expectedTitle); 
        assertTrue(true, "Title should contain 'simple'"); 
    } 
    @AfterTest 
    public void closeBrowser() throws InterruptedException 
    { 
        Thread.sleep(1000); 
        driver.quit(); 
    } 
} 





package com.example; 
import com.google.gson.Gson; 
public class Main 
{ 
    public static void main(String args[]) 
    { 
        Gson gson= new Gson(); 
        String json= gson.toJson(new Person("john",30) ); 
        System.out.println(json); 
    } 
} 
class Person 
{ 
    private String name; 
    private int age; 
    public Person(String name, int age) 
    { 
        this.name=name; 
        this.age=age; 
    } 
} 
 





4b.  https://fadihaafra.github.io/<your-repository-name>/ remove the angular later

5b        maven deploy plugin
deploy ftp
copy from dist
edit urlk   <url>file:///D:/my-local-maven-repo</url> 
5b        mkdir d:/mylocalrepo_1
5b        mvn deploy
       
8       java -jar jenkins.war --httpPort=8181 
8              http://localhost:8181 
7       java -jar target/copy filename
7       gradle init --type pom
        gradle clean build
        java.build.gradle example with main 

7.....
        
         plugins {
    id 'java'
    id 'application'
}

group 'com.example'
version '1.0-SNAPSHOT'

sourceCompatibility = '1.8'
targetCompatibility = '1.8'

repositories {
    mavenCentral()
}

dependencies {
    testImplementation 'org.junit.jupiter:junit-jupiter-api:5.8.1'
    testRuntimeOnly 'org.junit.jupiter:junit-jupiter-engine:5.8.1'
}

test {
    useJUnitPlatform()
}

application {
    mainClassName = 'com.example.Main'
}

jar {
    manifest {
        attributes 'Main-Class': 'com.example.Main'
    }
    from {
        configurations.runtimeClasspath.collect { it.isDirectory() ? it : zipTree(it) }
    }
}
                 http://localhost:8181 




2a   mvn --version
     gradle -v

     3  maven repository 
       gson
     open <dependencies>
     4 maven jar plugion 
     change main classs
     terminal mvn clean package
     target demo copy dekstop 
     cd prompt cd desktop
     java -jar paste

     4 html index
     maven plugin to copy resources
     project.basedir/docs
     src/main/resoucws
     terminal mvn install
     git bash create repo
     git init
     git add .
     gt commit -m "ic"
     copu url
     go to git bash pages master docs save
     chrome follwoing url 



     
