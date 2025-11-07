string[] wordsToSearch = { "apple", "banana", "cherry", "date", "elderberry", "fig" };

        Console.Write("Enter the word you would like to find: ");
        string targetWord = Console.ReadLine();

        if (targetWord != null)
        {
            targetWord = targetWord.ToLower();
            
            bool wordFound = PerformLinearSearch(wordsToSearch, targetWord);

            if (wordfound=true)
            {
                Console.WriteLine("True");
            }
            else
            {
                Console.WriteLine("False");
            }
        }
    }

    static bool PerformLinearSearch(string[] wordList, string target)
    {
        foreach (string currentWord in wordList)
        {
            if (string.Equals(currentWord, target, StringComparison.OrdinalIgnoreCase))
            {
                return true;
            }
        }


    }
}
