# tamrin3..using System;

class Program
{
    static void Main()
    {
        double product = 1; // متغیر برای ذخیره حاصل ضرب
        int number;

        Console.WriteLine("برای خاتمه دادن عدد ۰ را وارد کنید.");

        while (true)
        {
            Console.Write("لطفاً یک عدد وارد کنید: ");
            string input = Console.ReadLine();

            if (int.TryParse(input, out number))
            {
                if (number == 0)
                {
                    break; // خاتمه دادن به حلقه
                }
                product *= number; // محاسبه حاصل ضرب
            }
            else
            {
                Console.WriteLine("لطفاً یک عدد صحیح وارد کنید.");
            }
        }

        Console.WriteLine("حاصل ضرب اعداد وارد شده: " + product);
    }
}
