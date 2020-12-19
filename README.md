# CF_731A_Night_at_the_Museum
using System;
 
namespace Night_at_the_Museum
{
    class Program
    {
        static void Main(string[] args)
        {
            string str=Console.ReadLine();
            int flag = 97,diff,sum=0;
            for(int i=0;i<str.Length;i++)
            {
                diff = Math.Abs(flag - str[i]);
                if(diff>13)
                {
                    diff = 26 - diff;
                }
                sum += diff;
                flag = str[i];
            }
 
            Console.WriteLine(sum);
        }
    }
}
