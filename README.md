# Oct-20-2021-L8ExercisesProblems
only in .txt

//--------------------------DAYS OF THE MONTH (SWITCH)--------------------------------

#include &lt;iostream>
  
using namespace std;

int main()

{

cout << "Kindly select the option number for the month you want to see the days of:\n";

cout << " 1. January\n 2. February\n 3. March\n 4. April\n 5. May \n 6. June \n 7. July \n 8. August\n 9. September\n 10. October\n 11. November\n 12. December\n";

int a;
cout <<"\n Please enter the number here: ";
cin >> a;

switch (a)

{

case 1:

{

cout << "The month of January have days 31";

break;

}

case 2:

{

cout << "The month of February have days 28 if there is a leap year than 29";

break;

}

case 3:

{

cout << "The month of March have days 31";

break;

}

case 4:

{

cout << "The month of April have days 30";

break;

}

case 5:

{

cout << "The month of May have days 31";

break;

}

case 6:

{

cout << "The month of June have days 30";

break;

}

case 7: {

cout << "The month of July have days 31";

break;

}

case 8:

{

cout << "The month of August have days 31";

break;

}

case 9:

{

cout << "The month of September have days 30 ";

break;

}

case 10:

{

cout << "The month of October have days 31";

break;

}

case 11:

{

cout << "The month of November have days 30";

break;

}

case 12:

{

cout << "The month of December have days 31";

break;

}

default:

{

cout << "Invalid Input." << endl;

break;

}

}

}

//--------------------------FUEL ME UP (SWITCH)--------------------------------
  
// Oct10-L8Exercise-FUEL ME UP (SWITCH).cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include &lt;iostream>

#include &lt;stdexcept> //just in case the stdlimits is not working

#include &lt;limits> //just in case the stdlimits is not working

using namespace std;

int main() {

double liter, total;

cout << "Hello! Kindly select which Fuel Type you want to use. 'P' for Petrol or 'D' for Diesel: ";

char fuel;

cin >> fuel;

if (fuel == 'p' || fuel == 'P'){

cout << "You have selected " << fuel << " For Perol." << endl;

}

else if (fuel == 'd' || fuel == 'D'){

cout << "You have selected " << fuel << " For Diesel." << endl;

}

else  {

cout << "Invalid Input. Exiting Program..." << endl;

exit(1);

}

cout << "Enter how many liters you want to fill your car: ";

cin >> liter;

if (std::cin.fail())

{

std::cin.clear();

std::cin.ignore(std::numeric_limits<std::streamsize>::max(), '\n');

std::cout << "Invalid input.. exiting program... ";

}

else {

cout << "You have selected " << liter << " litres\n";

switch (fuel)

{

case 'P':

case 'p':

{

total = liter * 0.8;

cout << "\n The total price would be " << total << " AED" << endl;

break;

}

case 'd':

case 'D':

{

total = liter * 0.5;

cout << "\n The total price would be " << total << " AED" << endl;

break;

}

default:

{

cout << "Invalid input.. exiting program... ";

break;

}

}

}

}


//--------------------------SWITCHING TEMPERATURE--------------------------------
// Oct10-L8Exercise-Switching Temp(SWITCH).cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include &lt;iostream>

using namespace std;

int main()

{

int a;

cout << "Press 1 for Celsius To Fahrenheit. \n";

cout << "Press 2 for Fahrenheit To Celsius. \n";

cout << "Press 3 to Exit.\n\n";

cout << "Please Enter Your Choice of Number:  ";

cin >> a;

switch (a)

{

double ans,celcius,fahrenheit;

case 1:

cout << "Enter The Temperature in Celsius: ";

cin >> ans;

fahrenheit = (ans * 9 / 5) + 32;

cout << "\nTemperature in Fahrenheit is = " << fahrenheit << "F";

break;

case 2: 

cout << "Enter The Temperature in Fahrenheit: ";

cin >> ans;

celcius = (ans - 32) * 5 / 9;

cout << "\nTemperature in Celsius is = " << celcius << "C";

break;

case 3:

cout << "Exiting Program.... ";

exit(0);

default:

cout << "\nError, unknown number. Exiting program.... \n";

break;

}

}

//--------------------------BONUS EXERCISE: SWITCHING GRADE CALCULATOR--------------------------------
// Example program
  
#include &lt;iostream>
  
#include &lt;string>

using namespace std;

int main()

{

int score;

string name;

char grade;

cout << "Enter a Student Name: ";

getline(cin, name);

cout << "Enter the Student's Mark(between 0-100): ";

cin >> score;

if (score < 0 || score>100)

{

cout << "Invalid Score" << endl;

return 0;

}

switch (score / 10)

{

case 10:

case 9:

case 8:

grade = 'A';

cout << "\nStudent Name: "<< name << "\n" << "Grade = " << grade << endl;

break;

case 7:

grade = 'B';

cout << "\nStudent Name: " << name << "\n" << "Grade = " << grade << endl;

break;

case 6:

grade = 'C';

cout << "\nStudent Name: " << name << "\n" << "Grade = " << grade << endl;

break;

case 5:

grade = 'D';

cout << "\nStudent Name: " << name << "\n" << "Grade = " << grade << endl;

break;

case 4:

grade = 'E';

cout << "\nStudent Name: " << name << "\n" << "Grade = " << grade << endl;

break;

case 3:

case 2:

case 1:

case 0:

grade = 'F';

cout << "\nStudent Name: " << name << "\n" << "Grade = " << grade << endl;

break;

default:

cout << " \nInvalid Grade..." << endl;

}

return 0;

}


//--------------------------CAPITAL OF FRANCE (SWITCH)---------------------------------
// Example program

#include &lt;iostream>

using namespace std;

int main()

{

char input;

cout << "What is the Capital of France? \n \n a) Paris \n b) France \n c) Nice \n \n Enter your answer: ";

cin >> input;

switch (input)

{

case 'a':

cout << "\n Correct!";

break;

case 'b':

cout << "\n Wrong.";

break;

case 'c':

cout << "\n Nope.";

break;

default:

cout << "\n Invalid Input.";

}

}

//--------------------------NAME THAT SHAPE (SWITCH)--------------------------------
// Example program

#include &lt;iostream>

using namespace std;

int main()

{

int shape;

cout << "Enter number of sides to name the shape: ";

cin >> shape;

switch (shape)

{

case 1:

case 2:

cout << "\nCannot identify the shape.\n ";

break;

case 3:

cout << "\n Triangle  has " << shape << " sides. \n";

break;

case 4:

cout << "\nSquare | Rectangle has " << shape << " sides.\n";

break;

case 5:

cout << "\nPentagon has " << shape << " sides.\n";

break;

case 6:

cout << "\nHexagon have " << shape << " sides.\n";

break;

case 7:

cout << "\nHepaton have " << shape << " sides.\n";

break;

case 8:

cout << "\nOctagon have " << shape << " sides.\n";

break;

case 9:

cout << "\nNonagon have " << shape << " sides.\n";

break;

case 10:

cout << "\nDecagon have " << shape << " sides.\n";

break;

default:

cout << "\nInvalid Input.";

break;

}

}
