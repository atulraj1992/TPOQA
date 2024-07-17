# TPOQA
Assessment SDETs/QA Leads
package com.tpo.qa.ass.URL;

import ...
/**
 * This Class is to navigate to the URL to search for product name iPhone.
 * /
public class navigateUrl {
public static String iphone

//
WebDriver driver;
//Validates if URL is loaded
public void navigateUrl {
try {
driver = TC.driver.get.navigate().to("https://www.amazon.com/);
driver.navigate().refresh();
String url = geturl ();
if (url!=null) {
closeBrowser ();
}
else {
TC.Report(driver,Status.Fail, "UTL fetched is null");
}
Catch (InterruptedException | BadPaddingException | NoSuchAlgorithmException | NoSuchPaddingException | InvalidKeyException e) {
TC.Report (driver, Status.Fail, " Navigation to url unsuccessful | failed in class navigateurl | Method navigateurl");
closeBrowser();
WebElement search_bar = TC.findelement(driver, By.ID,"searchtextbox");
//or alternatively use By.xpath("//*[@id=\"Amazon-url\"]/div/nav/a));
search_bar.send_keys("iPhone");
search_bar.send_krys(Keys.RETURN);

// Wait until the search results are loaded
First_result = WebDriverWait(driver, 10).until(EC.presence_of_element_located((By.xpath("//*[@id=\"Search-bar\"]/div/nav/a));
)
Assert "Apple iPhone found in the first result.");
driver.quit();

