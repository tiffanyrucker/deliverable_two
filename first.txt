import java.util.Scanner;

public class DataDifference {
	public static void main(String [] args)

	{
		Scanner scanner = new Scanner(System.in); // create scanner object
	
	int year1, year2, month1, month2, day1, day2;

//prompt for input
System.out.println ("Enter the first date: (format -> \"Y M D\")");

//read the first input
year1 = scanner.nextInt(); //assuming the input is correct
month1 = scanner.nextInt();
day1 = scanner.nextInt();

//prompt for input
System.out.println ("Enter the second date: (format -> \"Y M D\")");

//read the second input
year2 = scanner.nextInt(); // assuming the input is correct
month2 = scanner.nextInt();
day2 = scanner.nextInt();

//convert the input to days
int date1 = (year1 * 365 + month1 * 30) + day1; 
int date2 = (year2 * 365 + month2 * 30) + day2;

int durationdifference = date2 - date1; 

//convert back
int year = durationdifferenc /365;
int month = (durationdifference % 365) / 30;
int day = (durationdifference % 365) % 30; 

// output the difference
System.out.println ("Difference is: " + year + " " + month + " " + day);
	}

    }
























































