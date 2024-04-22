import 'dart:io';

void main() {
  // Prompt the user for input
  stdout.write('Enter a number: ');
  var input = stdin.readLineSync();
  
  // Convert the input to a double
  var number = double.tryParse(input);
  
  if (number == null) {
    print('Invalid input. Please enter a valid number.');
    return;
  }
  
  // Check the criteria and print the appropriate message
  if (number > 10) {
    print('Your number is greater than 10');
  } else if (number < 10) {
    print('Your number is less than 10');
  } else {
    print('Your number is equal to 10');
  }
}
