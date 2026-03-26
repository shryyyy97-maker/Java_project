# Java_project
 compound interest calculator 💸
package shreya;
import java.util.Scanner;
public class p2 
{
	public static void main(String [] args)
	{
		Scanner s=new Scanner(System.in);
		double principal;
		double rate;
		int timescompound;
		int years;
		double amount;
		
		System.out.println("enter the principal amount");
		principal=s.nextDouble();
		System.out.println("enter the interest rate (in %)");
		rate=s.nextDouble()/100;
		System.out.println("Enter the # of times compounded per year");
		timescompound=s.nextInt();
		System.out.println("enter the # years");
		years=s.nextInt();
		
		amount=principal* Math.pow(1+rate/timescompound,timescompound*years);
		System.out.println("the amount later"+years+"is :$"+amount);
		s.close();
	}
}
