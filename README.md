using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Exam_One
{
    class Program
    {
        static void Main(string[] args)
        {
            double priceWhiskey = double.Parse(Console.ReadLine());
            double beer = double.Parse(Console.ReadLine());
            double wine = double.Parse(Console.ReadLine());
            double rakia = double.Parse(Console.ReadLine());
            double whiskey = double.Parse(Console.ReadLine());

            double priceRakia = priceWhiskey / 2;
            double priceBeer = priceRakia - (priceRakia * 0.8);
            double priceWine = priceRakia - (priceRakia * 0.4);

            double beerTotal = beer * priceBeer;
            double wineTotal = wine * priceWine;
            double rakiaTotal = rakia * priceRakia;
            double whiskeyTotal = whiskey * priceWhiskey;

            Console.WriteLine("{0:f2}", beerTotal + wineTotal + rakiaTotal + whiskeyTotal);
        }
    }
}
