# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

 Boolean Algebra is a branch of algebra that deals with boolean values—true
 and false. It is fundamental to digital logic design and computer science, providing a
 mathematical framework for describing logical operations and expressions

  Boolean Expression
  
  (i)F1
  
  ![image](https://github.com/user-attachments/assets/cbd33d99-d9a9-401b-8a5c-221563810959)

  (ii)F2
  
  ![image](https://github.com/user-attachments/assets/4d2bc3e3-e2bf-40dd-8d9a-c9a79c01facd)

  Truth Table
  
 (i)F1
 
 ![image](https://github.com/user-attachments/assets/e24590fb-a699-4ef6-b4de-a09545649383)

 (ii)F2

![image](https://github.com/user-attachments/assets/bf5ebc27-0398-4b59-a0ef-68af65b0b532)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:LEELA KRISHNA A.V.S  RegisterNumber:212224240013

~~~
 i)F1
 module funct1(a,b,c,d,f1);
 input a,b,c,d;
 output f1;
 assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
 endmodule
 ii)F2
 module funct2(w,x,y,z,f2);
 input w,x,y,z;
 output f2;
 assign f2=((~y & z)|( w & y )|(x & y));
 endmodule
~~~


**RTL realization**

 (i)F1

 ![image](https://github.com/user-attachments/assets/85880932-677b-436a-b67d-4ec2e9b5859d)

 (ii)F2
![image](https://github.com/user-attachments/assets/c9392d35-684c-4a13-b08a-2f6a6769bbae)


**Timing Diagram**

(i)F1

![image](https://github.com/user-attachments/assets/dd66fc83-2695-4949-8cc2-9c19daa0ccb1)

(ii)F2


![image](https://github.com/user-attachments/assets/b61eb70b-6884-4611-a4d7-a2d92d53717c)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

