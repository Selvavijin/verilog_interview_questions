# verilog_interview_questions

![image](https://github.com/user-attachments/assets/96968d39-5c99-43f8-a2d4-2c8d837833d3)

'&' in VHDL acts as a contatenation operator.

![image](https://github.com/user-attachments/assets/3014e446-f920-41dd-b5ad-39ebbacf9033)

In unary operator(&), if any one bit is zero, then the output is zero. Output is 1, only if all the bits are 1.

![image](https://github.com/user-attachments/assets/80d01d10-fd3b-4dd2-9755-9366815905ad)

![image](https://github.com/user-attachments/assets/40177f80-d783-4705-a8ba-cf9e4edaa8f9)

'~' in verilog is a unary not operator. Whereas '!' acts as a logical NOT operator and the output will be 1 bit.

![image](https://github.com/user-attachments/assets/10ab8b7b-af9b-4d1c-a692-734aa296754a)

'~A' in verilog = 'not A' in vhdl

![image](https://github.com/user-attachments/assets/b2b4b57f-cd22-4486-bb87-2d4e77b30836)

In vhdl, 'not' is used for both the bitwise not and logical not operation. How?, if we use the 'not' in any assignment statement, it will acts as a bitwise 'not'. If we use 'not' in conditional statements, it will acts like logical 'not'.

![image](https://github.com/user-attachments/assets/efb58b24-3217-4e92-a2e5-03433588d751)

The #(parameter='no of bits') should be given after the module name and before the arguments list. If we do not write this, the default value of '4' will taken for the number of bits.

![image](https://github.com/user-attachments/assets/90b2b17d-cd04-401e-9ee8-2e7a80b870af)

Importance of sensitivity list:

Synthesizer is not going to consider the sensitivity list but, simulator consider the sensitivity list. Here, the simulation result and the synthesizer result are same. Because, whenever there is a change in a or b, it will be ANDed.

![image](https://github.com/user-attachments/assets/ed63fb16-a741-45cf-a453-724d0d0851aa)

This is the simulator output
![image](https://github.com/user-attachments/assets/876ec13d-57b4-4ca9-a1a0-5d975fb9bc4f)

In this case, only when there is a change in A, there will be expected result.

![image](https://github.com/user-attachments/assets/556aeb57-feb1-47e3-9ce1-b0eb512b3a6a)

This is the simulator result
![image](https://github.com/user-attachments/assets/091c919f-cad4-4295-b757-387282643d67)

In this case, the simulator will goes on running. Because there is no statements inside the always block.

![image](https://github.com/user-attachments/assets/095bb4ae-f8b0-4325-bce6-485898d5a246)

![image](https://github.com/user-attachments/assets/76a74708-35d6-4d4e-8037-ae0f1a4602bf)

But in all the three cases, the synthesis result will be same. Because, the synthesizer will not consider the sensitivity list as mentioned above.
