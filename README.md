package com.ia.ass;
import java.util.Scanner;
public class CountLettersInArray {

     static Scanner sc=new Scanner(System.in);
     static char[] arr={'D','D','S','W','R','J','K','K','O','S','W','Q','E','T','Y','W','A','W','V','M'};
 
	public int[] RandomCharecter(){
		System.out.println(arr);
		int counts[]=new int[26];
		for(int i=0;i<arr.length;i++){
			counts[arr[i]-'A']++;
		}
	return counts;
	}
		
	
	public void displayCounts(int counts[]){
		System.out.println("===========occurence of letters================");
		for(int i=0;i<arr.length;i++){
			if(counts[arr[i]-'A'] !=0){
				System.out.print(arr[i]+"   ");
				System.out.println(counts[arr[i]-'A']);
				counts[arr[i]-'A']=0;
			}
		}
	}
	public  char[] createArray(char[] arr){
	
		
		return arr;
	}

	public static void main(String[] args) {

		CountLettersInArray m=new CountLettersInArray();
		System.out.println(m.createArray(arr));
		m.displayCounts(m.RandomCharecter());
	}
}
