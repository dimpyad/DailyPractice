### Step by step apporach for running simple selenium tests on chrome browser inside docker container
1. Verify docker is installed and running in your system run the command docker --version
  
   Output may look like this as per your system installed docker version: 
   ```
   Docker version 20.10.10, build b485636
   ```
2. Run the command - docker pull selenium/standalone-chrome and make sure download is successful.
3. Run the command - docker images
   output: 
   ```
   selenium/standalone-chrome   latest  c89972124090   5 days ago    1.18GB
   ```
4. Run the command - docker run -p 4444:4444 -v /dev/shm:/dev/shm selenium/standalone-chrome
   Output: If everything goes fine selenium grid should start in the docker container with a standalone chrome node (you should be able to see the logs in console)
   Open browser and type http://localhost:4444/ - you should see selenium grid UI with one registered chrome node.
   
5. Run the following code:
```
import java.net.MalformedURLException;
import java.net.URL;

import org.openqa.selenium.chrome.ChromeOptions;
import org.openqa.selenium.remote.RemoteWebDriver;

public class DockerTests {

	public static void main(String[] args) throws MalformedURLException {
		ChromeOptions options = new ChromeOptions();
		options.addArguments("start-maximized"); // open Browser in maximized mode
		options.addArguments("--disable-dev-shm-usage"); // overcome limited resource problems

		RemoteWebDriver driver = new RemoteWebDriver(new URL("http://localhost:4444/wd/hub"), options);
		driver.get("https://google.com");
		System.out.println("Page title = " + driver.getTitle());
		driver.quit();
	}

}
```
You will see the following output of the program running inside the docker container:
```
Mar 23, 2022 10:31:41 PM org.openqa.selenium.remote.ProtocolHandshake createSession
INFO: Detected dialect: W3C
Page title = Google
```
6. Stop the container running either from command line or from Docker Desktop UI.
