# CipherDiary
A rudimentary diary that uses a text key to encipher entries.

The diary is a dictionary of text entries. Each entry is keyed by a user-specified title and references the content.
A key, either in the form of a text file or a string, must be specified prior to adding new entries or reading existing ones.
Entries are encoded by converting both the text input and key into ASCII, and then adding the key integers in sequence to the input ones.
If we run out of key integers, we simply go back to the beginning of the key.

e.g.

Key:<br>
'abcd' ([ 97, 98, 99, 100])<br>
Text:<br>
'hello' ([104, 101, 108, 108, 111])<br>
Encoded:<br>
[104+97, 101+98, 108+99, 108+100, 111+97] = [201,199,207,208,208]<br>

Details on usage can be found in the iPython notebook. 

Note: this is a very simplistic cipher, meant to provide a basic level of privacy, and not for highly sensitive information!
