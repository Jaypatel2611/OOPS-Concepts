import java.util.*;
class 	Digit
{
	static int count=0;
	
	void counter()
	{
	    Scanner sc=new Scanner(System.in);
		System.out.print("Enter the number : ");
	    int num=sc.nextInt();
	    num = Math.abs(num);
		while(num!=0)
		{
			num=num/10;
			count++;
		}
		if(count==0)
		{
		    count=1;
		}
		System.out.println("The Number of digits is : "+count);
	}
}

class Main
{
	public static void main(String[]args)
	{
		Digit d=new Digit();
		d.counter();
		
		
	}
}
