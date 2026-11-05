# Java-lab-pro_1
import java.util.Scanner;
class Lab1
{
public static void main(String[]args)
{
int row = Integer.parseInt(args[0]);
int col = Integer.parseInt(args[1]);
int i,j;
int m1[][]=new int[row][col];
int m2[][]=new int[row][col];
int res[][]=new int[row][col];
Scanner scn = new Scanner(System.in);
System.out.println("Enter first matrix element:");
for(i=0; i<row; i++)
{
for(j=0; j<col; j++)
{
System.out.print("Enter Elements:");
int ele = scn.nextInt();
m1[i][j]=ele;
}
}
System.out.println("Enter second matrix element:");
for(i=0; i<row; i++)
{
for(j=0; j<col; j++)
{
System.out.print("Enter Element:");
int ele = scn.nextInt();
m2[i][j]=ele;
}
}
System.out.println("Resultant Matrix:");
for(i=0; i<row; i++)
{
for(j=0; j<col; j++)
{
res[i][j]=m1[i][j]+m2[i][j];
System.out.print(res[i][j]+"\t");
}
System.out.println();
} 
}
} 
