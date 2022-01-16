# -dsa5-
#string_infytq
#remove duplicates and white spaces 
#using linkedHashSet
import java.util.*;
class Main{
    public static String removeDuplicatesandSpaces(String str){
         LinkedHashSet s = new LinkedHashSet();
         for(char c:str.toCharArray())
         {
             s.add(c);
         }
        String a="";
       Iterator<Character> itr = s.iterator(); 
       while(itr.hasNext())
       {
           a+=itr.next();
       }
        return a.replace(" ","");
	}
	
	public static void main(String args[]){
	    String str = "object oriented programming";
	    System.out.println(removeDuplicatesandSpaces(str));
	}
}
