# Nagarro-Assessment-test-2022


#1 - Modify Variabe Names

Variables in any programming language should be named in such a way that the name iteself clarifies the purpose. However, we cannot have a variable name having multiple words separated by space. Therefore, we use different approaches of defining variable names as given below:
In C++: this_is_a_variable
In Java: thisIsAVariable
Your task is to convert a C++ variable name into a Java variable name and vice versa and then return the converted variable name.


C# solution:

public string modify_variableName{

		string input1 = "modify_variable_name";
	    string ans = "";
	    string l = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
	    bool b1 = false;
	    bool b2=false;
	    char p = ' ';
	    if(!string.IsNullOrEmpty(input1)) {
		foreach(char c in input1)
		{
		    if(c.ToString()=="_" && !b1 && !b2)
		    {
		        b1 = true;
		    }
		    else if(l.ToUpper().Contains(c.ToString()) && !b1 && !b2)
		    {
		        b2 = true;
		    }
		    if(b1) {
		        if(p.ToString() == "_")
		            ans = ans + c.ToString().ToUpper();
		        else if(c.ToString() != "_")
		            ans = ans + c.ToString();
		    }
		    else if(b2) {
		        ans = ans + "_" + c.ToString().ToLower();
		        b2 = false;
		    }
		    else {
		        ans = ans + c.ToString();
		    }
		    p = c;
		}
	}
	return ans;

}


#2 - Array of duplicate elements

You are given an integer array of N positive elements. Any integer in array can occur multiple times. Your task is to find all the distinct duplicate elements and store them in an array in increasing order and then finally return this array as output.

Input: 6
Input2: {4,4,7,8,8,9}

Output: {4,8}

Java - 


#3 - Students Report

Given a list of N students, every student is marked for M subjects. Each student is denoted by an index value. Their teacher Ms. Margaret must ignore the marks of any 1 subject for every student. For this she decides to ignore the subject which has the lowest class average.
Your task is to help her find that subject, Calculate the total marks of every student in all the other subjects and then finally return the array of the total marks scored by each student.


#4 - Find the shortest Substring

Find the shortest substring in a given string that contains all the characters of a given a word.
Return the shortest substring containing all the characters of input2.
