import java.lan.System;
public class TilingProblem{
    public static int getways(int n){
        
        //base case
        if(n<=3){
            return n;
        }
        
        //recursive call
        return getways(n-1)+getways(n-2);
        
    
            
    }
}
public class Main
{
	public static void main(String[] args) {
		System.out.println("for n=1,total ways="+getways(1));
	}
}
//LOGIC EXPLANATION
//suppose you have to find at n=4;
//return getways(4)=getways(3)+getways(2)
//Both are less than 3
//getways=3+2=5

