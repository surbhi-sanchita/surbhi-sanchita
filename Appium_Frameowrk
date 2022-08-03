package tests;

import io.appium.java_client.android.AndroidDriver;
import org.openqa.selenium.remote.DesiredCapabilities;
import org.testng.annotations.AfterTest;
import org.testng.annotations.BeforeTest;

import java.net.MalformedURLException;
import java.net.URL;

public class BaseClass {

    public AndroidDriver driver;

    @BeforeTest
    public void setup()  throws MalformedURLException {

        String appiumServerURL = "http://127.0.0.1:4723/wd/hub";

        DesiredCapabilities dc = new DesiredCapabilities();
        dc.setCapability("deviceName","Huwaei Nova 3i");
        dc.setCapability("udid","JUC7N18710010424");
        dc.setCapability("platformName","Android");
        dc.setCapability("platformVersion","9");
        dc.setCapability("appPackage","com.android.calculator2");
        dc.setCapability("appActivity","com.android.calculator2.Calculator");

        driver= new AndroidDriver(new URL(appiumServerURL), dc);
        System.out.println("Application Started");

    }

    @AfterTest
    public void teardown(){
        driver.quit();
        driver.close();

    }
}


