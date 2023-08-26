# game_RockPaperScissor
import java.util.Random;
import java.util.Scanner;

public class rockPaperC 
{
    public static void main(String[] args) {
    //for genrate random no.
   
    Scanner sc=new Scanner(System.in);
    int game;
    System.out.println("1.Paper");
    System.out.println("2.Rock");
    System.out.println("3.Scissors");
    System.out.println("Enter your no.");
    game=sc.nextInt();
     Random rand= new Random();
    int n=rand.nextInt(3);
    n+=1;
    System.out.println("Computer's no.");
    System.out.println(n);
    switch(game)
    {
        
            case 1:
                if(n==1){
                    System.out.println("Tie!");

                }
                else if(n==2){
                    System.out.println("You win!");
                }
                else{
                    System.out.println("You lost");
                }
                break;
            case 2:
            if(n==1){
                System.out.println("You lost!");
            }
            else if(n==2){
                System.out.println("Tie!");
            }
            else{
                System.out.println("You won");
            }
            break;
            case 3:
            if(n==1){
                System.out.println("You won");

            }
            else if(n==2){
                System.out.println("You lost !");
            }
            else{
                System.out.println("Tie!");
            }
            break;
            default:
            System.out.println("Enter the valid no.");
    }
}
}
