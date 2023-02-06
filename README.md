// Nirav
package com.Nirav;

public class feb_6_assesment {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
           //String a="COVID crisis has taught us several lessons and together we will overcome this great challenge. Now there is a sense of introspection in people. India will emerge stronger from this.";
        String a="COVID crisis has taught us several lessons and together we will overcome this great challenge. Now there is a sense of introspection in people. India will emerge stronger from this." ;  
		int sum=0;
           int count=0;
           int j=0;
           for(int i=0;i<a.length();i++) {
        	   char ch=a.charAt(i);
        	   
        	   int temp= (int)ch;
        	   if(Character.isUpperCase(ch)) {
        		   temp=temp-38;
        		   System.out.print(temp+" ");{count++;}
        	   }
        	   else if(Character.isLowerCase(ch)){
        		   temp=temp-96;
        		   System.out.print(temp+" ");{count++;}
        	   }
        	   else if(ch=='.') {
        		   temp=99;
        	   }
        	   else if(ch==' ') {
        		   temp=0;
        	   }
        	   sum=sum+temp;
        	   if(temp==0) {
        		   j=j+sum+(count*(count*100));
        		   count=0;
        	   }
        	   
           }
           System.out.println();
           System.out.println("Before increment sum is: "+sum);
           System.out.println("After increment sum is: "+j);
           
	}

}
