
# 0x03. Shell, init files, variables and expansions

0-alias => Create a script that creates an alias.

    Name: ls
    Value: rm *

1-hello_you => Create a script that prints hello user, where user is the current Linux user.


2-path => Add /action to the PATH. /action should be the last directory the shell looks into when looking for a program.


3-paths => Create a script that counts the number of directories in the PATH. 


4-global_variables => Create a script that lists environment variables


5-local_variables => Create a script that lists all local variables and environment variables, and functions.


6-create_local_variable => Create a script that creates a new local variable.

  Name: BEST
  Value: School

7-create_global_variable => Create a script that creates a new global variable.

    Name: BEST
    Value: School


8-true_knowledge => Write a script that prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new                         line.

9-divide_and_rule => Write a script that prints the result of POWER divided by DIVIDE, followed by a new line.

    POWER and DIVIDE are environment variables

    julien@production-503e7013:~$ export POWER=42784
    julien@production-503e7013:~$ export DIVIDE=32
    julien@production-503e7013:~$ ./9-divide_and_rule | cat -e
    1337$
    julien@production-503e7013:~$


10-love_exponent_breath => Write a script that displays the result of BREATH to the power LOVE

  BREATH and LOVE are environment variables
  The script should display the result, followed by a new line


11-binary_to_decimal => Write a script that converts a number from base 2 to base 10.

    The number in base 2 is stored in the environment variable BINARY
    The script should display the number in base 10, followed by a new line

    julien@production-503e7013:~/$ export BINARY=10100111001
    julien@production-503e7013:~/$ ./11-binary_to_decimal
    1337
    julien@production-503e7013:~/$


12-combinations => Create a script that prints all possible combinations of two letters, except oo.

    Letters are lower cases, from a to z
    One combination per line
    The output should be alpha ordered, starting with aa
    Do not print oo
    Your script file should contain maximum 64 characters

    julien@ubuntu:/tmp/0x03$ echo $((26 ** 2 -1))
    675
    julien@ubuntu:/tmp/0x03$ ./12-combinations | wc -l
    675
    julien@ubuntu:/tmp/0x03$ 
    julien@ubuntu:/tmp/0x03$ ./12-combinations | tail -303 | head -10
    oi
    oj
    ok
    ol
    om
    on
    op
    oq
    or
    os
    julien@ubuntu:/tmp/0x03$ 


13-print_float => Write a script that prints a number with two decimal places, followed by a new line.

    The number will be stored in the environment variable NUM.


100-decimal_to_hexadecimal => Write a script that converts a number from base 10 to base 16.

    The number in base 10 is stored in the environment variable DECIMAL
    The script should display the number in base 16, followed by a new line


101-rot13 => Write a script that encodes and decodes text using the rot13 encryption. Assume ASCII.

    julien@production-503e7013:~/shell/fun_with_the_shell$ cat quote
    "Everyone is a proponent of strong encryption."
    - Dorothy E. Denning
    julien@production-503e7013:~/shell/fun_with_the_shell$ ./101-rot13 < quote
    "Rirelbar vf n cebcbarag bs fgebat rapelcgvba."
    - Qbebgul R. Qraavat
    julien@production-503e7013:~/shell/fun_with_the_shell$ 


102-odd => Write a script that prints every other line from the input, starting with the first line.


103-water_and_stir => Write a shell script that adds the two numbers stored in the environment variables WATER and STIR and prints the result.

    WATER is in base water
    STIR is in base stir.
    The result should be in base bestchol

    julien@production-503e7013:~$ export WATER="ewwatratewa"
    julien@production-503e7013:~$ export STIR="ti.itirtrtr"
    julien@production-503e7013:~$ ./103-water_and_stir
    shtbeolhc
    julien@production-503e7013:~$
