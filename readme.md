# **Password-manager**
This is my project for IS IA-1.

A simple GUI is designed to simulate using a password manager.

The password vault is protected by a Master Password. This is only password you need to remember. The passwords for all of your other accounts are present inside the vault.

An SQLite database is used to store the Master password as well the contents of the vault.

When we use the application for the first time we can set up a new Master Password according to our choice.

After setting up a master password we get a key and option to copy the key to the clipboard.

This key protects us in case we forget our master password. It is used to reset password and erase the vault to prevent unauthorized access or attacks.

Once we enter the correct master password we are inside the vault. 

We can add Website name, username and password as entries in the vault.
All entries are displayed in the form of a list with rows and column structure.
There is an option to delete a particular entry if we so desire.

All the contents of the vault and the master password itself are stored in an encrypted format in the database. So if anyone accesses the database he won't be able to access any of the data.

The master password is stored in the SHA256 format which is a secure encryption algorithm.

The contents of the vault are stored and encrypted using the pbkdf2hmac format(Password based key derivation).