# Shalini_QA
import org.openqa.selenium.By;
import org.openqa.selenium.firefox.FirefoxDriver;

public class checkBox {

public static void main(String[] args) throws InterruptedException {
		
		// TODO Auto-generated method stub
		FirefoxDriver driver = new FirefoxDriver();
		//get url		
		driver.get("https://login.yahoo.com/config/login?.src=fpctx&.intl=us&.lang=en-US&.done=https%3A%2F%2Fwww.yahoo.com");
		driver.findElement(By.id("persistent")).isEnabled();
		boolean enabled = false;
		if(!enabled)
        {
     System.out.println("Already checked");
	    }
	    else
	    {
	        driver.findElement(By.id("persistent")).click();
	        System.out.println("checked now");
        }
		driver.close();
		}

		}

