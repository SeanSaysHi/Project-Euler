# Project-Euler
Collection of PE problems.
# Problem 1
/* Find the sum of all the multiples of 3 or 5 below 1000. */

import java.util.ArrayList;
class Problem1 {

	private static ArrayList<Integer> multiples = new ArrayList<Integer>();
	
	static int sum;
	
	 
	 public static void main(String[] args) {
	
		addToArray();
		
		numberAdder();
			
	}
	
	public static void addToArray () {
		
		for(int i = 0; i < 1000; i++) {
			
			if(i%3 == 0 || i%5 == 0) {
				
				multiples.add(i);
	 
			}	
		}
	}
	
	public static void numberAdder() {
		
		for(int j = 0; j < multiples.size(); j++) {
			
			System.out.println(sum += multiples.get(j));
		}	
	}
}


