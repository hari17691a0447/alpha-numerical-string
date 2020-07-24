# alpha-numerical-string

import java.io.*;
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    Scanner in=new Scanner(System.in);
		String s=in.nextLine();
		String a[]=s.split(" ");
		ArrayList<Integer>a1=new ArrayList<>();
		ArrayList<String>a2=new ArrayList<>();
		int n=a.length;
		for(int i=0;i<n;i++){
		    if(i%2==0){
		        a2.add(a[i]);
		    }else{
		        int d=Integer.parseInt(a[i]);
		        a1.add(d);
		        
		    }
		}
		Collections.sort(a1);
		Collections.sort(a2);
		int p=0;int e=0;
		for(int i=0;i<n;i++){
		    if(i%2==0){
		        System.out.print(a2.get(p)+" ");
		        p++;
		    }else{
		       System.out.print(a1.get(e)+" ");
		       e++;
		        
		    }
		}
	}
}
