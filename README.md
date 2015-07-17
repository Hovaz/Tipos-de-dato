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
                        Console.WriteLine("Su tamaño en bits es igual a 8");
                        Console.WriteLine("Sus valores pueden variar entre 0 y 255");
                    
                    }
                    if (d == 2)
                    {
                        Console.WriteLine("\n \t El SByte \n");
                        Console.WriteLine("Su tamaño en bits es igual a 8");
                        Console.WriteLine("Sus valores pueden variar entre -128 y 127");

                    }
                    if (d == 3)
                    {
                        Console.WriteLine("\n \t El Int \n");
                        Console.WriteLine("Su tamaño en bits es igual a 32");
                        Console.WriteLine("Sus valores pueden variar entre -2,147,483,648 y 2,147,483,647");

                    }
                    if (d == 4)
                    {
                        Console.WriteLine("\n \t El UInt \n");
                        Console.WriteLine("Su tamaño en bits es igual a 32");
                        Console.WriteLine("Sus valores pueden variar entre 0 y 4294967295");

                    }
                    if (d == 5)
                    {
                        Console.WriteLine("\n \t El Short \n");
                        Console.WriteLine("Su tamaño en bits es igual a 16");
                        Console.WriteLine("Sus valores pueden variar entre -32,768 y 32,767");

                    }
                    if (d == 6)
                    {
                        Console.WriteLine("\n \t El UShort \n");
                        Console.WriteLine("Su tamaño en bits es igual a 16");
                        Console.WriteLine("Sus valores pueden variar entre 0 y 65535");

                    }
                    if (d == 7)
                    {
                        Console.WriteLine("\n \t El Long \n");
                        Console.WriteLine("Su tamaño en bits es igual a 64");
                        Console.WriteLine("Sus valores pueden variar entre -9223372036854775808 y 9223372036854775807");

                    }
                    if (d == 8)
                    {
                        Console.WriteLine("\n \t El ULong \n");
                        Console.WriteLine("Su tamaño en bits es igual a 64");
                        Console.WriteLine("Sus valores pueden variar entre 0 y 18446744073709551615");

                    }
                    if (d == 9)
                    {
                        Console.WriteLine("\n \t El Float \n");
                        Console.WriteLine("Su tamaño en bits es igual a 32");
                        Console.WriteLine("Sus valores pueden variar entre -3.402823e38 y 3.402823e38");

                    }
                    if (d == 10)
                    {
                        Console.WriteLine("\n \t El Double \n");
                        Console.WriteLine("Su tamaño en bits es igual a 64");
                        Console.WriteLine("Sus valores pueden variar entre -1.79769313486232e308 y 1.79769313486232e308");

                    }
                    if (d == 11)
                    {
                        Console.WriteLine("\n \t El Char \n");
                        Console.WriteLine("Su tamaño en bits es igual a 16");
                        Console.WriteLine("Solo puede almacenar un caracter");

                    }
                    if (d == 12)
                    {
                        Console.WriteLine("\n \t El Bool \n");
                        Console.WriteLine("Su tamaño en bits es igual a 8");
                        Console.WriteLine("Solo puede ser true o false");

                    }
                    if (d == 13)
                    {
                        Console.WriteLine("\n \t El Object \n");
                        Console.WriteLine("es el tipo base de los otros tipos");

                    }
                    if (d == 14)
                    {
                        Console.WriteLine("\n \t El String \n");
                        Console.WriteLine("es una secuencia de caracteres");

                    }
                    if (d == 15)
                    {
                        Console.WriteLine("\n \t El Decimal \n");
                        Console.WriteLine("Su tamaño en bits es igual a 128");
                        Console.WriteLine("Sus valores pueden variar entre ±1.0 × 10e−28 y ±7.9 × 10e28");

                    }
                    Console.ReadKey();
                
                }
            }
        }
    }
}

