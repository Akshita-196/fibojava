# fibojava
package fibonacci;
import java.util.*;
public class Fibonacci {
    static void fibo(int n){
        int f1=0 ,f2=1;
        if(n==1){
            return;
        }
        System.out.println(f1+" ");
        for(int i=2;i<=n;i++){
            System.out.println(f2+" ");
            int t=f1+f2;
            f1=f2;
            f2=t;
        }
    }
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        fibo(n);
    }
    
}
