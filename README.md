using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Massivi
{
    class Program
    {
        static void Main(string[] args)
        {
            //            Задачи по массивам.
            //1.Считать с клавиатуры число, объявить массив с количеством элементов 
            //равным этому числу, заполнить массив случайными числами от 10 до 99,  
            //вывести на экран все значения массива
            //2.Создать массив состоящих из двух элементов, заполнить вывести элементы на экран, поменять элементы местами, вывести на экран
            //3.Создать массив состоящий из 10 элементов, заполнить случайными значениями, вывести на экран все элементы массива, найти минимальное и максимальное значение, поменять их местами, вывести все элементы массива еще раз
            //4.Создать массив из 5 элементов, заполнить случайными значениями, вывести на экран, посчитать сумму и произведение всех элементов массива и вывести на экран
            //5.Создать двухмерный массив 5х5, заполнить случайными числами, вывести на экран
            //6 *.Выполнить задание номер 2 из задачника

            //Задание №1
            
            Console.Write("Добро пожаловать. Введи число: ");
            Random rnd = new Random();
            string r = Console.ReadLine();
            int s = System.Convert.ToInt32(r);
            int[] arr = new int[s];

            for (int i = 0; i < s; i++)
            {
                
                arr[i] = rnd.Next(10, 99);
                Console.WriteLine(arr[i] + " ");

                if (arr[i] % 2 == 0)
                {
                  Console.WriteLine("Четное число "  +arr[i]);               
                }
            }

            //Минимальное и максимальное значение.
            //int min = arr.Min();
            //int max = arr.Max();
            //Console.WriteLine("Минимальное - " + min + "\nМаксимальное - " + max);
            //int diff = max - min; //Разница min и max
            //Console.WriteLine("Вот вам разница между наибольшим и наимешьим числами: " + diff );
            //Console.Write("Сейчас возведём в степень максимальное число: " + Math.Pow(max,2)); //в степень
