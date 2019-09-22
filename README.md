# Project-Eular-2
Hackerrank Solution

Each new term in the Fibonacci sequence is generated by adding the previous two terms. By starting with 1 and 2, the first 10 terms will be:

1, 2, 3, 5, 8, 13, 21, 34, 55, 89, ...

By considering the terms in the Fibonacci sequence whose values do not exceed four million, find the sum of the even-valued terms.

Solution:-

import java.io.*;
import java.util.*;
import java.text.*;
import java.math.*;
import java.util.regex.*;

public class Solution {

    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int t = in.nextInt();
        for(int a0 = 0; a0 < t; a0++){
            long n = in.nextLong();
            long a=0;
            long b=1,c=2,sum=2;
            while(true)
            {

                a= b+c;
                if(a>n)
                break;
                b=c;
                c=a;
                if(a%2==0)
                {
                sum = sum + a;
                }
            }
            System.out.println(sum);
        }
    }
}


