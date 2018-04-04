# Pyre
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Pyre
{
    class Program
    {
        static void Main(string[] args )55
        {
            Tycoon();
            Boxy();
            Average();
            Switch();
            Temp();
            Licence();
            Radius();
            Flour();
            Peraria();
            Moon();
            Numb();

            
            
        }
      
        static void Numb()
        {
            for (int i = 1; i < 101; i++)
            {
                Console.WriteLine("{0} + {1} = {2}\n", i, i, i + i);
            }
        }
        static void Peraria()
        {
            Console.WriteLine("Enter the dimensions of the rectangle");
            Console.WriteLine("Enter the width");
            int width = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Enter the length");
            int length = Convert.ToInt32(Console.ReadLine());

            int perimeter = width + length + width + length;
            int area = width * length;

            Console.WriteLine("The perimeter = {0}", perimeter);
            Console.WriteLine("The area = {0}\n", area);
            
        }

        static void Moon()
        {
            int weight;
            Console.WriteLine("Enter your weight");
            weight = Convert.ToInt32(Console.ReadLine());
            double moonWeight = (weight / 9.81) * 1.622;
            Console.WriteLine("{0}\n", moonWeight);
        }
        static void Radius()
        {
            Console.WriteLine("Enter the radius of the circle");
            int radius = Convert.ToInt32(Console.ReadLine());
            double perimeter = 2 * 3.142 * radius;
            double area = 3.142 * (radius * radius);
            Console.WriteLine("Perimeter = {0} \nArea = {1}\n", perimeter, area);
        }
        static void Flour()
        {
            Console.WriteLine("How much grams of flour do you have?");
            int grams = Convert.ToInt32(Console.ReadLine());
            double cup = grams / 125;
            Console.WriteLine("Cups = {0}\n", cup);
            
        }
        static void Licence()
        {
            Console.WriteLine("How old are you?");
            int age = Convert.ToInt32(Console.ReadLine());
            if (age <= 15)
            {
                Console.WriteLine("You cannot apply");
            }
            else
            {
                Console.WriteLine("You can apply");
            }
        }
        static void Temp()
        {
            Console.WriteLine("Please enter your temperature");
            int temp = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("And now age");
            int age = Convert.ToInt32(Console.ReadLine());

            Console.WriteLine("Temp = {0}\nAge = {1}", temp, age);

            if (age < 2 || temp >= 38)
            {
                Console.WriteLine("You need to call a doctor");
            }

            if (temp > 39.5)
            {
                Console.WriteLine("You have a high temperature");
            }
        }
        static void Switch()
        {
            Console.WriteLine("Enter a number between 0-9");
            int num = Convert.ToInt32(Console.ReadLine());
            if(num > 9 || num < 0)
            {
                Console.WriteLine("You didn't enter the right number coon!! \nEnter again");
                num = Convert.ToInt32(Console.ReadLine());
            }
            else
            {
                switch (num)
                {
                    case 0:
                        Console.WriteLine("zero");
                        break; 
                    case 1:
                        Console.WriteLine("one");
                        break;
                    case 2:
                        Console.WriteLine("two");
                        break;
                    case 3:
                        Console.WriteLine("three");
                        break;
                    case 4:
                        Console.WriteLine("four");
                        break;
                    case 5:
                        Console.WriteLine("five");
                        break;
                    case 6:
                        Console.WriteLine("six");
                        break;
                    case 7:
                        Console.WriteLine("seven");
                        break;
                    case 8:
                        Console.WriteLine("eight");
                        break;
                    case 9:
                        Console.WriteLine("nine\n");
                        break;
                }
            }
        }
        static void Array()
        {
            int[] abray = new int[20];
            for (int a = 0; a < 20; a++)
            {
                abray[a] = a * 5;
                Console.WriteLine(abray[a]);
            };
        }

        static void TwoArray()
        {
            // Two arrays that compare and check each other 

            int[] price = new int[8];
            int[] choco = new int[5];
        }

        static void Machine()
        {
            Console.WriteLine("Please enter your name and the amount of eggs you want \nEnter your name:");
            string name = Console.ReadLine();
            Console.WriteLine("Enter eggs");
            int eggs = Convert.ToInt32(Console.ReadLine());

        }
        static void Average()
        {
            Console.WriteLine("How many numbers do you want averaged?");
            int num = int.Parse(Console.ReadLine());
            int sum = 0;
            for (int y = 1; y <= num; y++)
            {
                
                Console.WriteLine("Enter number {0}", y);
                int sumVarible = int.Parse(Console.ReadLine());
                sum = sum + sumVarible;

            }
            Console.WriteLine("Total is {0}", sum);
            Console.WriteLine("Average is {0}", sum / num);
        }

        static void Boxy()
        {
            Console.ForegroundColor = ConsoleColor.DarkCyan;

            Console.WriteLine("LADIES AND METALMEN!!! TONIGHT WE ARE HOSTING THE INTERNATIONAL METALMAN BOXING COMPETITION!!!\nWOOOOOOOOO!!!");
            Console.WriteLine("TWO FIGHTERS, TWO CHAMPIONS, TWO HOTBOYS, BUT ONLY ONE WILL BE STANDING AT THE END OF THE NIGHT!!!\n");
            Console.WriteLine("(Hey)\n(PSTTT)\n(Hey you, coolguy, you hear me?)\n(Tell me your name)");
            string playerbun = Console.ReadLine();
            Console.WriteLine("{0}?\nThats your name?!?!\nGreat\nHey how about you there, you got a name?", playerbun);
            string playerpoo = Console.ReadLine();
            Console.WriteLine("Your kidding!\n{0} is your name!!!\nTHATS AWESOME!!!", playerpoo);
            Console.WriteLine("LADIES AND GENITALS!!! OUR TWO METALMEN STAND BEFORE US!!! \nIN THE LEFT CORNER GIVE IT UP TO {0}!!!!!", playerbun);
            Console.WriteLine("WOOOOOOO!!!\nAND HERE IN THE RIGHT CORNER WE HAVE {0}\nWOOOOOOOOOOOOOOOOOOO!!!", playerpoo);
            Console.WriteLine("{0}, ENTER A NUMBER BETWEEN 0-10", playerbun);
            int p1 = int.Parse(Console.ReadLine());
            Console.WriteLine("AND YOU {0}, PLEASE ENTER A NUMBER BETWEEN 0-10", playerpoo);
            int p2 = int.Parse(Console.ReadLine());
            Random rnd = new Random();
            if (p1 > p2)
            {
                int p1Score = 10;
                int p2Score = 9;
                Console.WriteLine("{0} GETS 10 points AND {1} GETS 9 POINTS", playerbun, playerpoo);
                int num = 10;
                for (int b = 1; b <= num; b++)
                {
                    Console.WriteLine("ROUND {0}", b);
                    
                    int p1Scorer = rnd.Next(1, 11);
                    int p2Scorer = rnd.Next(1, 11);
                    Console.WriteLine("{0} gets {1}", playerbun, p1Scorer);
                    Console.WriteLine("{0} gets {1}", playerpoo, p2Scorer);
                    if (p1Scorer > p2Scorer)
                    {
                        Console.WriteLine("{0} WINS THE ROUND!!!!", playerbun);
                        p1Score = p1Score + 1;
                    }
                    if (p2Scorer > p1Scorer)
                    {
                        Console.WriteLine("{0} WINS THE ROUND!!!!", playerpoo);
                        p2Score = p2Score + 1;
                    }

                    if (p1Scorer == p2Scorer)
                    {
                        Console.WriteLine("ITS A TIE");
                        p1Score = p1Score + 0;
                        p2Score = p2Score + 0;
                    }

                }

                Console.WriteLine("{0}  {1}", p1Score, p2Score);
            }
            if (p2 > p1)
            {
                int p1Score = 10;
                int p2Score = 9;
                Console.WriteLine("{0} GETS 10 points AND {1} GETS 9 POINTS", playerpoo, playerbun);
                int num = 10;
                for (int b = 1; b <= num; b++)
                {
                    Console.WriteLine("ROUND {0}", b);

                    int p1Scorer = rnd.Next(1, 11);
                    int p2Scorer = rnd.Next(1, 11);
                    Console.WriteLine("{0} gets {1}", playerbun, p1Scorer);
                    Console.WriteLine("{0} gets {1}", playerpoo, p2Scorer);
                    if (p1Scorer > p2Scorer)
                    {
                        Console.WriteLine("{0} WINS THE ROUND!!!!", playerbun);
                        p1Score = p1Score + 1;
                    }
                    if (p2Scorer > p1Scorer)
                    {
                        Console.WriteLine("{0} WINS THE ROUND!!!!", playerpoo);
                        p2Score = p2Score + 1;
                    }

                    if (p1Scorer == p2Scorer)
                    {
                        Console.WriteLine("ITS A TIE");
                        p1Score = p1Score + 0;
                        p2Score = p2Score + 0;
                    }

                }

                Console.WriteLine("{0} GETS {1}\n{2} GETS {3}", p1, p1Score, p2, p2Score);
            }
        }

        static void Tycoon()
        {
            //I would have to use multiple methods for the different functions
            //This one could be the chatacter sheet

            Console.WriteLine("Welcome to Console Tycoon!");
            Console.WriteLine(".x.x.xSTORYx.x.x.");
            Console.Write("Enter your name:");
            string name = Console.ReadLine();
            CharacterSheet();
            Console.WriteLine(".X.X.X.CHARACTER CUSTOMISATIOJN.X.X.X.");
            Console.WriteLine(".x.x.xSTORYx.x.x.");

        }
        static void CharacterSheet()
        {
            string[] menu = { "Name", "Gender", "Build", "Age", "Hair Colour" };
            Console.WriteLine("Menu:");
            for (int p = 1; p < menu.Length; p++)
            {
                Console.WriteLine("{0} {1}", p, menu[p]);

            }

        }



    }

}



