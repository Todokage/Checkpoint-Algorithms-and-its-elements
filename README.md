example 

LET
length_counter = 0
word_counter = 0
vowel_counter = 0
in_word = False

BEGIN
Repeat:
    Read ch (character)
    length_counter = length_counter + 1

    If ch is a vowel (lowercase or uppercase):
        vowel_counter = vowel_counter + 1

    If ch is a space or ch is '.':
        If in_word is True:
            word_counter = word_counter + 1
        in_word = False
    Else:
        in_word = True

Until ch is '.'

Print length_counter
Print word_counter
Print vowel_counter

END
