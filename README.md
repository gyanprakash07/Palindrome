# Palindrome
import java.util.Scanner;

class Palindrome
{
    public static void main(String arg[])
    {
        int n,p,s,rem;
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter any number ");
        n=sc.nextInt();
        p=n;
        for(s=0;n>0;n/=10)
        {
            rem=n%10;
            s=(s*10)+rem;
        }
        if(s==p)
            System.out.println(p+" is a palindrome number ");
        else
            System.out.println(p+" is not a palindrome number ");

    }
}

