import java.util.Scanner;

class Add{
	static int arr[] = new int[5];
	static Scanner input = new Scanner(System.in);
	public static void addarr()
	{
		System.out.println("Enter size of array:");
		int n = input.nextInt();
		int arr2[]=new int[arr.length];
		System.out.println("Enter "+ n +" elements of array one");
		for(int i=0;i<n;i++)
		{
			arr[i] = input.nextInt();
		}
		System.out.println("Enter "+ arr.length +" elements of array two");
		for(int i=0;i<arr.length;i++)
		{
			arr2[i] = input.nextInt();
		}
		System.out.println("common elementts are:");
		 for(int i = 0; i < n; i++) 
		 {  
		        for(int j =1; j < n; j++) 
		        {  
		            if(arr[i] == arr2[j])  
		                System.out.println(arr[j]); 
		        }  
		  }  
		
	}
}

public class Jala {

	public static void main(String[] args) {
		Add a = new Add();
		a.addarr();
	}
}
