# Traveling-At-Light-Speed
Just another repository
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace _8.Traveling_at_Light_Speed
{
    class Program
    {
        static void Main(string[] args)
        {
            decimal ly = decimal.Parse(Console.ReadLine());

            decimal distance = Math.Truncate(ly * 9450000000000m);
            decimal seconds = Math.Truncate(distance / 300000);
            decimal sec = seconds % 60;
            decimal minutes = Math.Truncate(seconds / 60);
            decimal min = minutes % 60;
            decimal hours = Math.Truncate(minutes / 60);
            decimal hrs = hours % 24;
            decimal days = Math.Truncate(hours / 24);
            decimal ds = days % 7;
            decimal weeks =Math.Truncate (days / 7);

            Console.WriteLine(weeks + " " + "weeks");
            Console.WriteLine(ds + " " + "days");
            Console.WriteLine(hrs + " " + "hours");
            Console.WriteLine(min + " " + "minutes");
            Console.WriteLine(sec + " " + "seconds");   
        }
    }
}
