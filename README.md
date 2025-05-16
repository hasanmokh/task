# task

                    Console.WriteLine("The list is empty - nothing to search!");
                    continue;
                }
                Console.Write("Enter number to search for: ");
                if (int.TryParse(Console.ReadLine(), out int searchNumber))
                {
                    bool found = false;
                    for (int i = 0; i < numbers.Count; i++)
                    {
                        if (numbers[i] == searchNumber)
                        {
                            Console.WriteLine($"Number {searchNumber} found at index {i}");
                            found = true;
                        }
                    }

                    if (!found)
                    {
                        Console.WriteLine($"Number {searchNumber} not found in the list!");
                    }
                }
                else
                {
                    Console.WriteLine("Invalid input. Please enter a valid integer!");
                }
            }
            else if (input == "2")
            {
                if (numbers.Count == 0)
                {
                    Console.WriteLine("The list is already empty!");
                }
                else
                {
                    numbers.Clear();
                    Console.WriteLine("All numbers have been removed from the list!");
                }
            }
            else if (input == "3")
            {
             
