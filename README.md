# Prodigy-CS-Task-1
In this project, I developed a Python program to encrypt and decrypt user input utilizing the Caesar Cipher algorithm.


Task Overview
You were tasked with creating a Python program that implements the Caesar Cipher, a simple encryption technique where each letter in the plaintext is shifted by a fixed number of positions in the alphabet. The program needed to allow users to input a message and a shift value to perform both encryption and decryption.

Steps Taken
Understanding the Caesar Cipher Algorithm:

I began by understanding the Caesar Cipher algorithm, recognizing that it involves shifting each letter in the plaintext by a specified number of positions in the alphabet. 

caesar_cipher_encrypt Function:

- I created this function to handle the encryption process and set "text" and "shift" as parameters.
- Set "encrypted_text" as an empty string to accumulate the encrypted characters.
- Iterated over each character in the input text using a loop, checking if the character was alphabetic using "isalpha()".
- Calculated the effective shift using the modulo operation (shift % 26) and then applied the shift to the character's ASCII value.
- Ensured that the shift wrapped around the alphabet and converted the result back to a character.
- Created an else statement where non-alphabetic characters were added to the result unchanged.
- Returned the encrypted text.
  
caesar_cipher_decrypt Function:

- I created this function to handle the decryption process and reversed the shift by using the negative shift value.

main Function:

- The main function was used to handle user interaction and input.
- The function prompted the user to choose between encryption and decryption, then asked for the input message and shift value.
- Depending on the user's choice, it either called the caesar_cipher_encrypt or caesar_cipher_decrypt function.
  
Testing the Program:

After writing the code, I saved and executed it. I then tested the program by entering different messages and shift values, verifying that the encryption and decryption processes worked correctly.


Summary of Variables Used:

- text: The input message to be encrypted or decrypted.
- shift: The number of positions each letter is shifted in the alphabet.
- encrypted_text: The result of the encryption process.
- char: Each character in the input text.
- shift_amount: The effective shift value after applying the modulo operation to handle wrap-around.
- new_char: The shifted character after applying the Caesar Cipher logic.
- choice: The user's decision to either encrypt or decrypt the message.

Summary of Resources Used:

- https://www.scaler.com/topics/caesar-cipher-python/
- ChatGPT
- https://www.youtube.com/watch?v=x71kJyNvB5o
