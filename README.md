# abbrivation-form


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System;   

namespace ConsoleApp6
{
    class Program
    {
        static void Main(string[] args)
        {
            string str = "raj kumar sharma";
            string[] strarr = str.Split();

            StringBuilder sb = new StringBuilder();

            for (int i = 0; i < strarr.Length-1; i++)
            {
                sb.Append(strarr[i].Substring(0, 1).ToUpper());
            }
             sb.Append(".");

            sb.Append(strarr[strarr.Length - 1]);

            Console.WriteLine(sb);
            Console.ReadLine();
        }
    }
}
