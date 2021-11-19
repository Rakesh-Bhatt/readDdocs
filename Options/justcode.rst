Codes to the problem
++++++++++++


Ruby code
=========

Here is the code for finding greatest number among three number
Ruby code ::
            x,y,z = 2,5,4
            if x >= y and x >= z
                puts "x = #{x} is greatest."
            elsif y >= z and y >= x 
                puts "y = #{y} is greatest."
            else 
                puts "z = #{z} is greatest."
            end

Python code :

.. code-block:: python

                        num1 = float(input("Enter first number: "))
                        num2 = float(input("Enter second number: "))
                        num3 = float(input("Enter third number: "))
                        
                        if (num1 > num2) and (num1 > num3):
                        largest = num1
                        elif (num2 > num1) and (num2 > num3):
                        largest = num2
                        else:
                        largest = num3
                        
                        print("The largest number is",largest)
