1  Problem Q



import java.util.Scanner;
class axios {
   
    
    
    void determine(double x,double y){
        if(x==0 && y==0){
         System.out.println("Origem");
        }
         else if(x==0){
             System.out.println("Eixo Y");
         }
          else if(y==0){
             System.out.println("Eixo X");
         }
        else if(x>0&&y>0){
            System.out.println("Q1");
        }
        else if(x>0&&y<0){
            System.out.println("Q4");
        }
        else if(x<0&& y>0){
            System.out.println("Q2");
        }
        else{
            System.out.println("Q3");
        }
        
    }
    
    
  }
  public class Main{
      
      public static void main(String []args){
          Scanner input =new Scanner(System.in);
          double x=input.nextDouble();
          double y=input.nextDouble();
    
          axios object =new axios();
          object.determine(x,y);
      }
      
      
      
  }
  //////////////////////////////////////////
2 Problem R





import java.util.Scanner;

 class age {
   
    int years=0;
    int months=0;
        
      void howOld(int days){
        while(days>=356){ 
            years++;
        days=days - 356;
        
        }
        while(days>=30){ 
            months++;
        days=days - 30;
        
        }
        int day =days;
        System.out.println("years=>" +years+'\n'+ "months=>"+months);
        System.out.println("days=>"+day);
        
    }
}
     public class Main{
     
    public static void main(String[]args){


    
        System.out.println("enter the number of days to determine your age");
         Scanner input =new Scanner(System.in);
         int days=input.nextInt();
        age object=new age();
        object.howOld(days);
        
    }
}
    
    



  
