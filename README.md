# Test
Q1.
Consider the following code snippet: 
for(int i=INT1; i<INT2; i++)
	{
		System.out.println(i);
	}

Where, INT1 and INT2 can be any two integers. 
Which of the following will produce the same result? 
Select 1 correct option. 
a  for(int i=INT1; i<INT2; System.out.println(++i));   
b  for(int i=INT1; i++<INT2; System.out.println(i));   
c  int i=INT1; while(i++<INT2) { System.out.println(i); }   
d  int i=INT1; do { System.out.println(i); }while(i++<INT2);   
e  None of these. 

Q2.
What numbers will be printed by this program? 
public class ForSwitch
{
	public static void main(String args[])
	{
		char i;
	LOOP:   for (i=0;i<5;i++)
		{
			switch(i++)
			{
				case '0': System.out.println("A");
				case 1: System.out.println("B"); break LOOP;
				case 2: System.out.println("C"); break;
				case 3: System.out.println("D"); break;
				case 4: System.out.println("E");
				case 'E' : System.out.println("F");
			}
		}
	}
}
Select 2 correct options 
a  A   
b  B   
c  C   
d  E  
e  F 

Q3.
What will be printed by the following code if it is run with command line: java TestClass --0.50 ? 
(There are two minuses before 0.) 
public class TestClass
{
	public static int getSwitch(String str)
	{
	return (int) Math.round( Double.parseDouble(str.substring(1, str.length()-1)) );
	}
	public static void main(String args [])
	{
		switch(getSwitch(args[0]))
		{
			case 0 : System.out.println("Hello");
			case 1 : System.out.println("World"); break;
			default : System.out.println("Good Bye");
		}
	}
}
Select 1 correct option. 
a  Hello   
b  World   
c  Hello World   
d  Hello World Good Bye   
e  Good Bye 

Q4.
 public class BreakTest
{
  public static void main(String[] args)
  {
    int i = 0, j = 5;
    lab1 : for( ; ; i++)
    {
      for( ; ; --j)  if( i >j ) break lab1;
    }
    System.out.println(" i ="+i+" , j = "+j);
  }
}
What will it print? 
Select 1 correct option. 
a  i = 1, j = -1   
b  i = 1, j = 4   
c  i = 0, j = 4   
d  i = 0, j = -1   
e  It will not compile. 

Q5.
What will the following code print? 
void crazyLoop()
{
	int c = 0;
	JACK: while (c < 8)
	{
		JILL: System.out.println(c);
		if (c > 3) break JILL; else c++;
	}
}
Select 1 correct option. 
a  It'll not compile.   
    Because break JILL; would be valid only if JILL is labeling a loop or a block. In this case, there is no loop/block for break JILL; to break.   
        
b  It'll throw an exception at runtime.   
c  It'll print numbers from 0 to 8   
d  It'll print numbers from 0 to 3   
e  It'll print numbers from 0 to 4 
Q6.
What will the following program print? 
int i=0, j=11;
	do{
		if(i > j) { break; }
		j--;
	}while( ++i < 5);
	System.out.println(i+"  "+j);
Select 1 correct option. 
a  5 5   
b  5 6   
c  6 6   
d  6 5   
 e  4 5 
                                                                                                                                                                                              Q7. What will be printed by the following code if it is run with command line: java TestClass -0.50 ? 
public class TestClass
{
public static double getSwitch(String str)
	{
		return Double.parseDouble(str.substring(1, str.length()-1) );
	}
	public static void main(String args [])
	{
		switch(getSwitch(args[0]))
		{
			case 0.0 : System.out.println("Hello");
			case 1.0 : System.out.println("World"); break;
			default : System.out.println("Good Bye");
		}
	}
}
Select 1 correct option. 
a  Hello   
b  World   
c  Hello World   
d  Hello World Good Bye   
e  None of the above.   

Q8.
What is the result of executing the following code when the value of i is 5: 
switch (i)
{
    default:
    case 1:
        System.out.println(1);
    case 0:
        System.out.println(0);
    case 2:
        System.out.println(2);
        break;
    case 3:
        System.out.println(3);
}

Select 1 correct option. 
a  It will print 1 0 2   
b  It will print 1 0 2 3   
c  It will print 1 0    
d  It will print 1   
e  Nothing will be printed. 

Q9.
Which of these for statements are valid? 
1. for (int i=5; i=0; i--) { }
2.  int j=5;
      for(int i=0, j+=5;  i<j ; i++) {  j--;  }
3. int i, j;
    for (j=10; i<j; j--) { i += 2; }
4. int i=10;
    for ( ; i>0 ; i--) { }
5. for (int i=0, j=10; i<j; i++, --j) {;}
Select 1 correct option. 
a  1, 2   
b  3, 4   
c  1, 5   
d  4, 5   
e  5

Q10.
What will the following code print?
class Test
{
	public int luckyNumber(int seed)
	{
		if(seed > 10) return seed%10;
		int x = 0;
		try
		{
			if(seed%2 == 0) throw new Exception("No Even no.");
			else return x;
		}
		catch(Exception e)
		{
			return 3;
		}
		finally
		{
			return 7;
		}
	}
	public static void main(String args[])
	{
		int amount = 100, seed = 6;
		switch( new Test().luckyNumber(6) )
		{
			case 3: amount = amount * 2;
			case 7: amount = amount * 2;
			case 6: amount = amount + amount;
 			default :
		}
		System.out.println(amount);
	}
}
Select 1 correct option. 
a  It'll not compile.   
b  It'll throw an exception at runtime.   
c  It'll print 800   
d  It'll print 200   
e  It'll print 400   

Q11.
  Which of the following code snippets will compile fine? 
Select 3 correct options 
a  while (false) { x=3; }   
b  if (false) { x=3; }   
c  do{  x = 3;  } while(false);   
    In a do- while, the block is ALWAYS executed atleast once.   
d  for( int i = 0; i< 0; i++) x = 3; 

Q12.
What will the following program print? 
class LoopTest
{
	public static void main(String args[])
	{
		int counter = 0;
		outer: for(int i = 0; i < 3; i++)
                   	middle: for(int j = 0; j < 3; j++)
                        	inner: for(int k = 0; k < 3; k++)
				       {
	                             		if(k-j>0) break middle;
                             			counter++;
                             	       }
		System.out.println(counter);
	}
}
Select 1 correct option. 
a  2   
b  3   
c  6   
d  7   
e  9   

Q13.
  What will the following program print? 
class Test
{
	public static void main(String args[])
	{
		int c = 0;
		boolean flag = true;
		for(int i = 0; i < 3; i++)
		{
			while(flag)
			{
				c++;
				if(i>c || c>5) flag = false;
			}
		}
		System.out.println(c);
	}
}
Select 1 correct option. 
a  3   
b  4   
c  5   
d  6   
e  7 

Q14.
  What will the following program print? 
class Test
{
	public static void main(String args[])
	{
		int i=0, j=0;
		X1: for(i = 0; i < 3; i++)
		{
			X2: for(j = 3; j > 0; j--)
			{
				if(i < j) continue X1;
				else break X2;
			}
		}
		System.out.println(i+" "+j);
	}
}
Select 1 correct option. 
a  0 3   
b  0 2   
c  3 0   
d  3 3   
e  2 2 

Q15.
Which of the following constructs are valid.... 
1.                                 
   switch(5)                             
   {
      default :
   }
2.                                 
   switch(5)                          
   {                                  
      default : break;
   }                                  
3.switch(8);
4.  int =0;
Switch(x)
{
}
Select 1 correct option. 
a  1, 3   
b  1, 2, 3   
c  All are valid.   
d  3, 4   
e  1, 2, 4.   

   
