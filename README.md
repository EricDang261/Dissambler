The program should be ORG'ed at $1000.

At startup, the program should display whatever welcome messages you want to display and then prompt the user for the starting location and the ending location (in hexadecimal format) of the code to be disassembled. You need to clearly specify the expected input format for user inputs. If it's not clearly specified, then any encountered problems will get your points off. The program should scan the memory region and output the memory addresses of the instructions and the assembly language instructions contained in that region to the display. You should be able to actually disassemble your own program to the display! DO NOT embed test code into your disassembler code!

The display should show one screen of data at a time, hitting the ENTER key should display the next screen of information.

The program should be able to realize when it has an illegal instruction ( i.e, data ), and be able to deal with it until it can find instructions again to decode. Instructions that cannot be decoded, either because they do not disassemble as op codes or because you aren't able to decode them should be displayed as: 1000 DATA $WXYZ where $WXYZ is the hexadecimal number that couldn't be decoded. Your program should not crash because it can't decode an instruction. Remember, it is perfectly legal to have data and instructions interspersed, so it is very possible that you will hit data, and not an instruction.

Address displacements or offsets should be properly displayed as the address of the branch and display that value. It's the absolute address value, not the displacement value. For example: 1000 BRA 993 * Branch to address 993

When it completes the disassembly, the program should prompt the user to disassemble another memory image, or prompt the user to quit.
# run
To run this program, execute the Disaambler.x68 file. Then load the s68 test_demo into the program. Try inputting the starting address at 0x9000 and ending address at 0x938C.

# This is some result demo
![image](https://user-images.githubusercontent.com/62625277/172694524-f7119bac-f4ae-474d-b022-1074f40bf061.png)
![image](https://user-images.githubusercontent.com/62625277/172695085-568da168-dc2c-48a2-8b39-555b499196b4.png)
