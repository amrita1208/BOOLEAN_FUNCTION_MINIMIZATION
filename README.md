# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

Boolean function minimization is the process of simplifying Boolean algebraicexpressions to reduce the number of logic gates and complexity in a digital circuit,leading to more efficient, faster, and less costly hardware

For minimizing Boolean expressions,we can use a set of rules and laws (like distributive,associative, and complement laws) to simplify Boolean expressions. This methodfocuses on applying algebraic manipulations to reduce the complexity of the expressionby eliminating redundant terms.

Identity Law A ⋅ 1 = A, A + 0 = A

Null Law A ⋅ 0 = 0, A + 1 = 1

Idempotent Law A ⋅ A = A, A + A = A

Complement Law A ⋅ A′ = 0, A + A' = 1

Distributive Law A ⋅ (B + C) = A ⋅ B + A ⋅ C

De Morgan’s Law (A ⋅ B)′ = A′ + B', (A + B)′ = A′ ⋅ B′

Absorption Law A ⋅ (A + B) = A, A + (A ⋅ B) = A

Associative Law A + (B + C) = (A + B) + C, A.(B.C) = (A.B).C

Commutative law A B = B A,A + B = B + A

**Logic Diagram**

identity law

<img width="485" height="258" alt="{AB71490A-6122-4D45-93B2-00EF73AFB7CA}" src="https://github.com/user-attachments/assets/bb39893f-edc8-4d0f-98cf-51be29388ca7" />

idempotent law

<img width="182" height="237" alt="{266ED8D6-4C18-465A-93F3-3711AE18DE65}" src="https://github.com/user-attachments/assets/6cc34d6e-6098-49ed-876c-9afa34934021" />

 distributive law
 
<img width="392" height="111" alt="{3D7EE4AC-3357-49BC-BF31-8A3C69BF98C7}" src="https://github.com/user-attachments/assets/74561dc4-1387-46bc-9738-9d21e7a5f133" />

de morgan's law

<img width="374" height="386" alt="{500C2A5C-4FE9-49FA-8FC9-15E83B7B13DE}" src="https://github.com/user-attachments/assets/55623513-23a7-4a55-830b-bc2aa2725cec" />

absorption law

<img width="284" height="64" alt="{DB7D1B2D-75D8-4629-BE5B-4AFC8F9E1C67}" src="https://github.com/user-attachments/assets/2760ae06-944f-4d37-a457-04eb4842df20" />

associative law

<img width="225" height="217" alt="{8C9DE0D2-623E-4F80-A66E-725629895219}" src="https://github.com/user-attachments/assets/c9cc89a6-f5d9-4aa7-8a6e-97accf862501" />

commutative law

<img width="216" height="208" alt="{98474947-9B6F-4D4A-BFBA-3C4F28051439}" src="https://github.com/user-attachments/assets/2b217a49-301d-46f3-8f31-db949560da3d" />

null law

<img width="414" height="205" alt="{EBD76438-F9E8-4C0E-8E4F-D8A47AB27A5E}" src="https://github.com/user-attachments/assets/dffa6ea5-f996-4b32-bf69-175a00bc7b51" />

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

i)

module funct1(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));

endmodule

ii)

module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));

endmodule

**RTL realization**
**Output:**

i)

<img width="823" height="475" alt="{DE812631-A638-4F9F-A388-9D013C648BB7}" src="https://github.com/user-attachments/assets/ee4614b0-dc85-49b0-ba43-25cf0c81b380" />

ii)

<img width="790" height="513" alt="{C03D0E59-3A39-4193-8A41-4B828F52BB40}" src="https://github.com/user-attachments/assets/d3de8016-e2da-4d02-a975-ea825200ca54" />

**RTL**

**Timing Diagram**

i)

<img width="1003" height="456" alt="{BBCFC53B-075A-448E-BA4D-CECC6D8A7AC8}" src="https://github.com/user-attachments/assets/9eaf009b-aacf-4017-91b5-d3b9201f04ff" />

ii)

<img width="1099" height="462" alt="{AF9101D3-F237-4D83-AE3E-2DC8FBF93303}" src="https://github.com/user-attachments/assets/aa29269c-213b-4f5f-a26b-6e4fee174378" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

