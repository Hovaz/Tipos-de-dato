# Tipos-de-dato
programa q lee el tipo de dato ingresado por el usuario y le dice su tamaño en bytes y el rango

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace tipos_de_dato
{
    class Program
    {
        static void Main(string[] args)
        {

            int origWidth, width;
            int origHeight, height;
            origWidth = Console.WindowWidth;
            origHeight = Console.WindowHeight;
            width = origWidth * 3 / 2;
            height = origHeight * 3 / 2;
            Console.SetWindowSize(width, height);
            Console.ForegroundColor = ConsoleColor.Cyan;

            int d, m = 1;
            string dato;

            while (m == 1) 
            {
                Console.WriteLine("\t Bienvenido este programa le ayudara a conocer acerca de los tipos de datos \n \n");
                Console.WriteLine("\t Porfavor digita el numero correspondiente al tipo de dato que desea conocer \n");
                Console.WriteLine("1. Byte");
                Console.WriteLine("2. SByte");
                Console.WriteLine("3. Int");
                Console.WriteLine("4. Uint");
                Console.WriteLine("5. Short");
                Console.WriteLine("6. UShort");
                Console.WriteLine("7. Long");
                Console.WriteLine("8. Ulong");
                Console.WriteLine("9. Float");
                Console.WriteLine("10. Double");
                Console.WriteLine("11. Char");
                Console.WriteLine("12. Bool");
                Console.WriteLine("13. Object");
                Console.WriteLine("14. String");
                Console.WriteLine("15. Decimal");
                Console.WriteLine("16. Ingrese para salir");

                dato = Console.ReadLine();

                if (int.TryParse(dato, out d)) 
                {
                 if (d == 1) 
                    {
                        Console.WriteLine("\n \t El Byte \n");
                        Console.WriteLine("Su tamaño en bits es igual 8");
                        Console.WriteLine("Sus valores pueden variar entre 0 y 255");
                    
                    }
                }
            }
        }
    }
}
