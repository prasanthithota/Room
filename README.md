# Room

https://testing.in.capgemini.com/skillsfactory/login/index.php

Selenium WebDriver Training with Java and Many Live Projects | Udemy


package sample;

import java.util.List;

import org.openqa.selenium.Alert;
import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.chrome.ChromeDriver;
import org.openqa.selenium.support.ui.ExpectedConditions;
import org.openqa.selenium.support.ui.WebDriverWait;

public class Program {

	public static void main(String[] args) throws InterruptedException {
		// TODO Auto-generated method stub
		
		System.setProperty("webdriver.chrome.driver", "C:\\Users\\Prasatho\\chromedriver.exe");
		WebDriver driver=new ChromeDriver();
		/*driver.get("https://opensource-demo.orangehrmlive.com/");
		
		driver.findElement(By.xpath("//input[@id='txtUsername']"));
		driver.findElement(By.name("txtUsername")).sendKeys("Admin");		
		driver.findElement(By.id("txtPassword")).sendKeys("admin123");
		driver.findElement(By.cssSelector("input[id='btnLogin']")).click();*/
		
		driver.get("https://www.goindigo.in/");
		/*List<WebElement> ab=driver.findElements(By.xpath("//input[@type='radio']"));
		System.out.println(ab.size());
		WebDriverWait wait = new WebDriverWait(driver, 10);
		wait.until(ExpectedConditions.visibilityOfAllElements(ab));
		ab.get(2).click();*/
		
		//wait.until(ExpectedConditions.elementToBeClickable(ab));
		
		driver.findElement(By.xpath("//input[@id='oneWayTrip']")).click();
		
		Alert a=driver.switchTo().alert();
		System.out.println(a.getText());
		Thread.sleep(500);
		
		
		

		
	}
}


                List<WebElement> radio = driver.findElements(By.xpath("//h1[text()='Book a Flight']/parent::div/following-sibling::div[1]/div/label")); 
                System.out.println(radio.size()); 
                radio.get(2).click();

