using System;
using System.Text.RegularExpressions;

public class LettersSymbolsNumbers
{
    static void Main()
    {
        int n = int.Parse(Console.ReadLine());
        long lettersSum = 0;
        long symbolsSum = 0;
        long numbersSum = 0;

        for (int i = 0; i < n; i++)
        {
            string inputLine = Console.ReadLine();

            // Convert the input to upper-case
            inputLine = inputLine.ToUpper();

            // Remove the whitespace from the input
            inputLine = Regex.Replace(inputLine, "\\s+", "");

            for (int k = 0; k < inputLine.Length; k++)
            {
                char currentChar = inputLine[k];
                if (currentChar >= 'A' && currentChar <= 'Z')
                {
                    // Letters [a-zA-z]
                    lettersSum += (currentChar - 'A' + 1) * 10;
                }
                else if (currentChar >= '0' && currentChar <= '9')
                {
                    // Numbers [0-9]
                    numbersSum += (currentChar - '0') * 20;
                }
                else
                {
                    // Symbols
                    symbolsSum += 200;
                }
            }
        }

        Console.WriteLine(lettersSum);
        Console.WriteLine(numbersSum);
        Console.WriteLine(symbolsSum);
    }
}
