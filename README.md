# Pattern-1
import java.io.*; 
import java.util.*;  
public class Main { 	
  public static void main(String[] args) { 	
  Scanner sc = new Scanner(System.in); 		 		
  int n = sc.nextInt(); 		 		
  
  //front upper triangle  		
  for(int i=0; i<n/2; i++){ 		    
    for(int k=0; k<n/2-i; k++){ 		        
      System.out.print(" "); 		    
    } 		    
    for(int j=0; j<=i; j++){ 		        
      System.out.print("@"); 		    
    } 		    
    if(i<n/2){ 		        
      for(int l=0; l<(2*n)-1; l++){ 		            
        System.out.print(" "); 		        
      } 		    
    }
    System.out.print("*"); 		    
    System.out.println(); 		
  }           
  
  //front lower triangle 		
  for(int i=0; i<=n/2; i++){ 		    
  for(int k=0; k<i; k++){ 		        
    System.out.print(" "); 		    
  } 		    
  for(int j=i; j<=n/2; j++){ 		        
    System.out.print("@"); 		        
  } 		    
  //for middle line 		    
  if(i==0){ 		        
    for(int l=0; l<2*n; l++){ 		            
      System.out.print("*"); 		        
    } 		    
  } 		    
  else{ 		        
    for(int l=0; l<(2*n)-1; l++){ 		            
      System.out.print(" "); 		        
    } 		        
    System.out.print("*"); 		    
  } 		    
  System.out.println(); 		
}  	
} 
}
