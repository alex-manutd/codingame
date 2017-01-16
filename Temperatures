import java.util.*;
import java.io.*;
import java.math.*;

class Solution {

    public static void main(String args[]) {
        
        Scanner in = new Scanner(System.in);
        int n = in.nextInt(); // the number of temperatures to analyse
        in.nextLine();
        String temps = in.nextLine(); // the n temperatures expressed as integers ranging from -273 to 5526
        
        if (n == 0) {
            System.out.println(n);
        }
        else {
            int m;
            int closestPos = 5526;
            int closestNeg = -273;
            int thisTemp;
            String [] tokens = temps.split(" ");
            
            //Integer.parseInt(tokens[0]); 
                        
            for (int i = 0; i < n; i++) {
                thisTemp = Integer.parseInt(tokens[i]);
                if (thisTemp == 0) {
                    System.out.println(0);
                    }
                else if (thisTemp < 0) {
                    if (thisTemp > closestNeg) {
                            closestNeg = thisTemp;
                        }
                    }
                else if (thisTemp > 0) {
                    if (thisTemp < closestPos) {
                            closestPos = thisTemp;
                        }
                    }
                if (i == (n - 1)) {
                    if (closestPos <= Math.abs(closestNeg)) {
                            System.out.println(closestPos);
                        }
                    else {
                        System.out.println(closestNeg);
                        }
                    }
            }
        }
    }
}
