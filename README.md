# 2D-ARRAY-LARGEST-ELEMENT
import java.util.*;
class HelloWorld {
    public static void main(String[] args) {
        int a[][];
        a=new int[100][3];
        int c=0;
        Scanner sc= new Scanner(System.in);
          System.out.println("Enter array length: ");
        int n=sc.nextInt();// Array length
          System.out.println("Enter array elements: ");
        for(int i=0;i<n;i++){
            for(int j=0;j<n;j++){
            int k=sc.nextInt();
            a[i][j]=k;
            }
        }
        c=a[0][0];
        for (int i=0;i<n;i++){
            for(int j=0;j<n;j++){
             if(c<a[i][j])
             c=a[i][j];
            }
        }
         System.out.println(c+" is largest");
    }
}
