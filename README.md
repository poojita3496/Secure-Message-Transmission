** Usage **
When you run the program, you will be prompted to enter:

A prime number 
𝑝
A generator 
𝑔
The sender's and receiver's private keys
The message to be sent

The program will then output the encrypted message and the MAC. 
The receiver will input the received encrypted message and MAC to verify the integrity and decrypt the message.

** How It Works **

Diffie-Hellman Key Exchange:
Both sender and receiver generate their public keys using a shared prime number and generator.
They compute a shared secret key independently.

Caesar Cipher:
The sender encrypts the original message by shifting each character by a predefined number (the shared secret key).
The encrypted message is sent along with a MAC.

Message Authentication Code (MAC):
A MAC is generated using SHA-256 by combining the original message and the shared secret key.
The receiver verifies the MAC to check the integrity of the received message.

** Requirements **
Python 3.x
hashlib library (comes pre-installed with Python)
Contributing
Contributions are welcome! Please feel free to submit a pull request or open an issue for any improvements or suggestions.
