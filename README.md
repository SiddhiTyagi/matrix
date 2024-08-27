# matrix
import java.util.*;
class matrix {
public void main(int n) {
    Scanner b=new Scanner(System.in);
    int store[][]=new int[n][n];
    for(int i=0;i<n;i++)
    for(int j=0;j<n;j++){
        System.out.println("Enter elements: ");
        store[i][j]=b.nextInt();
    }
    int sum=0;
    for(int i=0;i<n;i++)
    for(int j=0;j<n;j++)
    if (i==j || i+j==n-1)
    sum=sum+store[i][j];
    System.out.println("Total sum of the numbers present in both the diagonals: "+sum);
}
} 
