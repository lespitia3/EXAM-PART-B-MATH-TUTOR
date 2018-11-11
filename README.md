# EXAM-PART-B-MATH-TUTOR


----Choosing a menu option----
	int choice;
	unsigned numbOne, numbTwo;

	cout << "Hello, Welcome to the Math Tutor." << endl;

	cout << " \nPick Subtraction, Multiplaication, or Addition to get started or end the program. " << endl;

	cout << "1.Subtraction \n" << "2.Multiplication \n" << "3.Addittion \n " << "4.End Program\n" << endl;
	cin >> choice;
  
  ----Allowing the menu to perform user request and the user solve math problems----
	if (choice == 1) { 
		numbOne = rand();
		numbTwo = rand();
	
		int answer = numbOne - numbTwo;
		int userInput;

		cout << "Subtract the following numbers." << endl;
		cout << numbOne << " " << "-" << " " << numbTwo <<  " = " ;
		cin >> userInput;
		if (userInput == answer) {
			cout << "Correct" << endl;
		}
		else {
			cout << "Incorrect" << endl;
		}
		return 0;

	}

	else if (choice == 2) {
		numbOne = rand();
		numbTwo = rand();

		int answer = numbOne * numbTwo;
		int userInput;

		cout << "Multiply the following numbers." << endl;
		cout << numbOne << " " << "*" << " " << numbTwo << " = ";
		cin >> userInput;
		if (userInput == answer) {
			cout << "Correct" << endl;
		}
		else {
			cout << "Incorrect" << endl;
		}
		return 0;


	}

	else if (choice == 3) {
		numbOne = rand();
		numbTwo = rand();

		int answer = numbOne + numbTwo;
		int userInput;

		cout << "Add the following numbers." << endl;
		cout << numbOne << " " << "+" << " " << numbTwo << " = ";
		cin >> userInput;
		if (userInput == answer) {
			cout << "Correct" << endl;
		}
		else {
			cout << "Incorrect" << endl;
		}
		return 0;


	}
	else if (choice == 4){
		return 0;

		
	}
	else {
		cout << "Error, you have not selected a choice on the menu!" << endl;
		return 0;
	}


	cin.get();
	cin.ignore();
	return 0;
}
