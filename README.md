# BubbleSort
program for bubble sort

public class BubbleSort {

	public static void main(String[] args) {
		int[] a= {36, 19, 29, 12, 5};
		int temp;
		
		//loop to increment rounds
		for(int i=0;i<a.length;i++)
		{
			int flag=0;
			//loop for comparing the adjacent elements
			for(int j=0;j<a.length-1-i;j++)
			{
				if(a[j]>a[j+1])
				{
					//swap operation
					temp=a[j];
					a[j]=a[j+1];
					a[j+1]=temp;
					flag=1;
				}
			}
			//if the list is already swapped it need not to swap again
			if(flag==0)
			{
				break;
			}
		}
		for(int i=0;i<a.length;i++)
		{
			System.out.print(a[i]+" ");
		}
	}

}

