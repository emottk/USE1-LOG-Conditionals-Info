#>> CONDITIONALS

Let's say we want to make a method that greets you when you say hello, and says goodbye when you say goodbye.		
How would we approach something like this?		

Well, we'd want to check for the user input. For this, we will be using something called an if/else statement, also known as a conditional. Conditionals look like this:

	if 	[ some statement ]
		#some code here
	else
		#some code here
	end

This is much easier to see within a working example. Let's try to build our greeter conditional.

	if greeting == "hello"
		print "hello, how are you?"
	else 
		print "I'm not sure what you said"
	end
		
This conditional is checking to see if `greeting == "hello"`. If this statement is true, it runs the code below it -- `print "hello, how are you?`. If the first statement is NOT true, however, it will instead go to the `else` statement, and run the code there. This would print `"I'm not sure what you said"`.		
This helps us control the flow of our program, and allows our app to be much more dynamic and user friendly!		

This if/else statement only gives us two choices, however. What if we wanted more options? Ruby has a solution for this. We can add an `elsif` to account for another piece of code.		

	if greeting == "hello"
		print "hello, how are you?"
	elsif greeting == "goodbye"
		print "have a nice day!"
	else 
		print "I'm not sure what you said"
	end
	
Now our program is even more dynamic! It can respond to multiple inputs. We can add as many `elsif` statements as we see fit.		


