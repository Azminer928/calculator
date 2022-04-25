# calculator
Simple Addition/Subtraction Calculator

// Header file which has the information to include the inout/output realted functions.
// The users first Entered Number!
        
    #include <stdio.h>
// The users first Entered Number!

    int EnterFirstinteger(char* msg)
    {
    int a;
    printf(msg);
    scanf_s(" %d", &a);
    return a;
    }

 
// The users Second Entered Number!

    int EnterSecondinteger(char* msg)
    {
    int b;
    printf(msg);
    scanf_s(" %d", &b);
    return b;
    }
    
 // The program calling on user to pick an option to add or to subtract!
    
    int Add1Subtract2(char* msg)
    {
    int c;
    printf(msg);
    scanf_s(" %d", &c);
    return c;
    }
    
 // The application asking if the user wants to enter another math question!
    
    int Again(char* msg)
    {
    int again;
    printf(msg);
    scanf_s(" %d", &again);
    return again;
    }
    int main()
    {
// The main program that puts together the math question and calls upon the users entered integers!
   
    char yes;
    int a, b, c, choice, again;

    yes = 'y';
    while (yes == 'y' || yes == 'Y')
    {

// Programming putting together the main numbers and calling on the integers!

        int main();
        char* First = "First Integer: ";
        printf("Please Enter First Number\n");
// Calling the users First Entered Number!

        a = EnterFirstinteger(First);
        printf("\nCalculating...\n");
        
// Calling the users Second Entered Number.

        char* Second = "Second Integer: ";
        printf("\nPlease Enter Second Number\n");
        b = EnterSecondinteger(Second);
// Putting together the users Numbers!

        printf("\nCalculating...\n");
        
// Calling the action to add or to subtract!

        char* Third = "Add(1), Subtract(2):\n";
        printf("\nPlease Enter (1) for Addition OR Please Enter (2) for Subtraction!\n");
        c = Add1Subtract2(Third);
        printf("\nFinal choice Press 1 for Addition or 2 for Subtraction and Press Enter!\n");
        
// Calling on the users choice to add and or to subtract and showing the question!

        scanf_s(" %d", & choice);
        
// This segment is where the program will show the answer to the math question.
// calling on the users choice and running in the background to find the answer! 

        switch (choice)
        {
        case(1):
            c = a + b;
            printf("\n%d + %d = %d\n", a, b, c);
            break;
        case(2):
            c = a - b;
            printf("\n%d - %d = %d\n", a, b, c);
            break;

        }
// Showing the Answer to the question at hand!

        char* Fourth = "Y or N?";
        printf("\nWould you want to Enter another Calculation?\n");
        again = Again(Fourth);
        printf("\n");

        scanf_s(" %c", &yes);
        
        printf("\n");
    }
// Ending the program unless the user picks the option to ask another question at hand!

        return 0;
}
