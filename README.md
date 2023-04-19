# Lab-8_202001089



Code for Boa.java
package Lab8package;

public class Boa {
	private String name;
	private int length; // the length of the boa, in feet
	private String favoriteFood;
	public Boa (String name, int length, String favoriteFood){
	this.name = name;
	this.length = length;
	this.favoriteFood = favoriteFood;
	}
	// returns true if this boa constrictor is healthy
	public boolean isHealthy(){
	return this.favoriteFood.equals("granola bars");
	}
	// returns true if the length of this boa constrictor is
	// less than the given cage length
	public boolean fitsInCage(int cageLength){
	return this.length < cageLength;
	}
	}
  
  
  Code for Boatest
  package Lab8package;

import static org.junit.Assert.*;

import org.junit.Test;


public class BoaTest {

	@Test
	public void testIsHealthy() {
		Boa healthyBoa = new Boa("Healthy Boa", 5, "granola bars");
		Boa unhealthyBoa = new Boa("Unhealthy Boa", 5, "junk food");
		
		assertTrue(healthyBoa.isHealthy());
		assertFalse(unhealthyBoa.isHealthy());
	}

	@Test
	public void testFitsInCage() {
		Boa smallBoa = new Boa("Small Boa", 5, "granola bars");
		Boa largeBoa = new Boa("Large Boa", 10, "granola bars");
		
		assertTrue(smallBoa.fitsInCage(10));
		assertFalse(largeBoa.fitsInCage(5));
	}

}

![image](https://user-images.githubusercontent.com/75687413/233025994-6f7f4cd8-7019-44d6-b872-7cf008266f1d.png)


![image](https://user-images.githubusercontent.com/75687413/233031390-182bcff5-7f0f-48eb-a4e0-802b46584804.png)


![image](https://user-images.githubusercontent.com/75687413/233031957-bb8e69d0-be18-4fd2-8902-0c320d5d95ee.png)


![image](https://user-images.githubusercontent.com/75687413/233032369-f59542f3-72af-4b5f-b3d5-a83b91a38f92.png)
