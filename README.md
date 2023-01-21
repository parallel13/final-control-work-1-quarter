# final-control-work-1-quarter


приветствие  
вывод задания пользователю ввести длинну массива  
вывод задания пользователю ввести строку  
инициализация вводимого массива  
запись в массив введенных строк  
функция проверки на длину строки  
если длина строки меньше 3х, проверяем следующий эллемент. если меньше записываем в новый массив и проверяем следующий.
когда элементы закончились выходим из цикла  
выводим на экран получившийся массив./







string[] SetArray(int Length)
{
    string[] array = new string[Length];
    for (int i = 0; i < array.Length; i++)
    {
        Console.Write($"Введите строку массива :\t");
        array[i] = Console.ReadLine();
    }
    return array;
}
//функция печати массива
void PrintArray(string[] array)
{
    System.Console.Write("[ ");
        for (int i = 0; i < array.Length; i++)
    {
        if (i < array.Length - 1) System.Console.Write($"{array[i]}, "); 
        else System.Console.Write($"{array[i]}");    
    }
    System.Console.WriteLine("]");
}

void PrintArrayNew(string[] array)
{

    System.Console.Write("[ ");
        for (int i = 0; i < array.Length; i++)
    { 
        if (array[i].Length <= 3) System.Console.Write($"{array[i]}, "); 
        else if (array[i].Length <= 3) System.Console.Write($"{array[i]}");    
    }
    System.Console.WriteLine("]");
}


string[]arr1 = SetArray (5);
PrintArray(arr1);
PrintArrayNew(arr1);


