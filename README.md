# Homework

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApp3
{
    class Program
    {
        static void Main(string[] args)
        {
            //      Задание: Пользователь вводит число от 1 до 9999 (сумму выдачи в банкомате). 
            //      Необходимо вывести на экран словами введенную сумму и в конце написать название валюты с правильным окончанием.
            //      Например: 7431 — семь тысяч четыреста тридцать один доллар

            Console.WriteLine("Введите сумму от 1 до 9999");

            enter: int enter = Convert.ToInt32(Console.ReadLine());

            bool enter_check = (enter >= 1) && (enter <= 9999);
            switch (enter_check)
            {
                case false:
                    Console.WriteLine("Число превышает указанный диапазон, повторите попытку");
                    goto enter;

                default:
                    break;
            }

            int l_4 = enter % 10;
            int e_1 = enter / 10;

            int l_3 = e_1 % 10;
            int e_2 = e_1 / 10;

            int l_2 = e_2 % 10;
            int e_3 = e_2 / 10;

            int l_1 = e_3 % 10;
            
            switch (l_1)
            {
                case 1:
                    Console.WriteLine("одна тысяча");
                    break;

                case 2:
                    Console.WriteLine("две тысячи");
                    break;

                case 3:
                    Console.WriteLine("три тысячи");
                    break;

                case 4:
                    Console.WriteLine("четыре тысячи");
                    break;

                case 5:
                    Console.WriteLine("пять тысяч");
                    break;

                case 6:
                    Console.WriteLine("шесть тысяч");
                    break;

                case 7:
                    Console.WriteLine("семь тысяч");
                    break;

                case 8:
                    Console.WriteLine("восемь тысяч");
                    break;

                case 9:
                    Console.WriteLine("девять тысяч");
                    break;

                default:
                    break;
            }

            switch (l_2)
            {
                case 1:
                    Console.WriteLine("сто");
                    break;

                case 2:
                    Console.WriteLine("двести");
                    break;

                case 3:
                    Console.WriteLine("триста");
                    break;

                case 4:
                    Console.WriteLine("четыреста");
                    break;

                case 5:
                    Console.WriteLine("пятьсот");
                    break;

                case 6:
                    Console.WriteLine("шестьсот");
                    break;

                case 7:
                    Console.WriteLine("семьсот");
                    break;

                case 8:
                    Console.WriteLine("восемьсот");
                    break;

                case 9:
                    Console.WriteLine("девятьсот");
                    break;
            }

            bool десять_девятьнадцать = (l_3 == 1) && (l_4 != 0);
            if (десять_девятьнадцать)
            {
                switch (l_4)
                {
                    case 1:
                        Console.WriteLine("одиннадцать");
                        break;

                    case 2:
                        Console.WriteLine("двенадцать");
                        break;

                    case 3:
                        Console.WriteLine("тринадцать");
                        break;

                    case 4:
                        Console.WriteLine("четырнадцать");
                        break;

                    case 5:
                        Console.WriteLine("патнадцать");
                        break;

                    case 6:
                        Console.WriteLine("шестнадцать");
                        break;

                    case 7:
                        Console.WriteLine("семнадцать");
                        break;

                    case 8:
                        Console.WriteLine("восемнадцать");
                        break;

                    case 9:
                        Console.WriteLine("девятнадцать");
                        break;
                }
            }
            else
            {
                switch (l_3)
                {
                    case 1:
                        Console.WriteLine("десять");
                        break;

                    case 2:
                        Console.WriteLine("двадцать");
                        break;

                    case 3:
                        Console.WriteLine("тридцать");
                        break;

                    case 4:
                        Console.WriteLine("сорок");
                        break;

                    case 5:
                        Console.WriteLine("пятьдесят");
                        break;

                    case 6:
                        Console.WriteLine("шестьдесят");
                        break;

                    case 7:
                        Console.WriteLine("семьдесят");
                        break;

                    case 8:
                        Console.WriteLine("восемьдесят");
                        break;

                    case 9:
                        Console.WriteLine("девяносто");
                        break;
                }

                switch (l_4)
                {
                    case 1:
                        Console.WriteLine("один");
                        break;

                    case 2:
                        Console.WriteLine("два");
                        break;

                    case 3:
                        Console.WriteLine("три");
                        break;

                    case 4:
                        Console.WriteLine("четыре");
                        break;

                    case 5:
                        Console.WriteLine("пять");
                        break;

                    case 6:
                        Console.WriteLine("шесть");
                        break;

                    case 7:
                        Console.WriteLine("семь");
                        break;

                    case 8:
                        Console.WriteLine("восемь");
                        break;

                    case 9:
                        Console.WriteLine("девять");
                        break;
                }

            }

            Console.ReadKey();
        }
    }
}
