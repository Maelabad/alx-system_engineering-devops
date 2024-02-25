Let's GOOOOO



0. Create a SSH RSA key pair
mandatory
Score: 0.0% (Checks completed: 0.0%)

Read for this task:

    Linux and Mac OS users
    Windows users

man: ssh-keygen

You will soon have to manage your own servers concept page hosted on remote data centers. We need to set them up with your RSA public key so that you can access them via SSH.

Create a RSA key pair.

Requirements:

    Share your public key in your answer file 0-RSA_public_key.pub
    Fill the SSH public key field of your intranet profile with the public key you just generated
    Keep the private key to yourself in a secure location, you will use it later to connect to your servers using SSH. Some storing ideas are Dropbox, Google Drive, password manager, USB key. Failing to do so will prevent you to access your servers, which will prevent you from doing your projects
    If you decide to add a passphrase to your key, make sure to save this passphrase in a secure location, you will not be able to use your keys without the passphrase

SSH and RSA keys will be covered in depth in a later project.


##############################################################################################

6. Superstitious numbers
mandatory
Score: 0.0% (Checks completed: 0.0%)

Write a Bash script that displays numbers from 1 to 20 and:

    displays 4 and then bad luck from China for the 4th loop iteration
    displays 9 and then bad luck from Japan for the 9th loop iteration
    displays 17 and then bad luck from Italy for the 17th loop iteration

Requirements:

    You must use the while loop (for and until are forbidden)
    You must use the case statement


##############################################################################################


7. Clock
mandatory
Score: 0.0% (Checks completed: 0.0%)

Write a Bash script that displays the time for 12 hours and 59 minutes:

    display hours from 0 to 12
    display minutes from 1 to 59

Requirements:

    You must use the while loop (for and until are forbidden)

Note that in this example, we only display the first 70 lines using the head command.

##############################################################################################


8. For ls
mandatory
Score: 0.0% (Checks completed: 0.0%)

Write a Bash script that displays:

    The content of the current directory
    In a list format
    Where only the part of the name after the first dash is displayed (refer to the example)

Requirements:

    You must use the for loop (while and until are forbidden)
    Do not display hidden files



sylvain@ubuntu$ ls
100-read_and_cut              1-for_best_school         6-superstitious_numbers
101-tell_the_story_of_passwd  2-while_best_school       7-clock
102-lets_parse_apache_logs    3-until_best_school       8-for_ls
103-dig_the-data              4-if_9_say_hi                  9-to_file_or_not_to_file
10-fizzbuzz                   5-4_bad_luck_8_is_your_chance
sylvain@ubuntu$  ./8-for_ls
read_and_cut
tell_the_story_of_passwd
lets_parse_apache_logs
dig_the-data
fizzbuzz
for_best_school
while_best_school
until_best_school
if_9_say_hi
4_bad_luck_8_is_your_chance
superstitious_numbers
clock
for_ls
to_file_or_not_to_file
sylvain@ubuntu$ 




############################################################################################


9. To file, or not to file
mandatory
Score: 0.0% (Checks completed: 0.0%)

Write a Bash script that gives you information about the school file.

Requirements:

    You must use if and, else (case is forbidden)
    Your Bash script should check if the file exists and print:
        if the file exists: school file exists
        if the file does not exist: school file does not exist
    If the file exists, print:
        if the file is empty: school file is empty
        if the file is not empty: school file is not empty
        if the file is a regular file: school is a regular file
        if the file is not a regular file: (nothing)


###########################################################################################

10

Write a Bash script that displays numbers from 1 to 100.

Requirements:

    Displays FizzBuzz when the number is a multiple of 3 and 5
    Displays Fizz when the number is multiple of 3
    Displays Buzz when the number is a multiple of 5
    Otherwise, displays the number
    In a list format


#########################################################################################


11. Read and cut

help: read

Write a Bash script that displays the content of the file /etc/passwd.

Your script should only display:

    username
    user id
    Home directory path for the user

Requirements:

    You must use the while loop (for and until are forbidden)


#########################################################################################


13. Let's parse Apache logs

Apache is among the most popular web servers in the world, serving 50% of all active websites, no doubt that you will have to interact with it within your career.

As a Full-Stack Software Engineer, you have to master the art of parsing log files. Today we will do a simple parsing of Apache log access files.

Today the Customer Support department reported that a user reported that the site is being “buggy”. Not being a detailed description, you want to have a look at the Apache logs and gather data about the traffic.

Write a Bash script that displays the visitor IP along with the HTTP status code from the Apache log file.

Requirement:

    Format: IP HTTP_CODE
        in a list format
        See example
    You must use awk
    You are not allowed to use while, for, until and cut
    Download and commit the apache-access.log file along with your answers files







14. Dig the data
#advanced
Score: 0.0% (Checks completed: 0.0%)

Now that you’ve parsed the Apache log file, let’s sort the data so you can get a better idea of what is going on.

Using what you did in the previous exercise, write a Bash script that groups visitors by IP and HTTP status code, and displays this data.

Requirements:

    The exact format must be:
        OCCURENCE_NUMBER IP HTTP_CODE
        In list format
    Ordered from the greatest to the lowest number of occurrences
        See example
    You must use awk
    You are not allowed to use while, for, until and cut

sylvain@ubuntu$ ./103-dig_the-data | head -n 10
    141 130.0.236.153 200
    140 62.210.250.66 200
    117 103.243.26.232 404
    67 195.154.172.143 200
    60 78.154.190.29 200
    45 195.154.172.59 200
    41 62.210.248.185 200
    41 167.114.156.198 200
    36 2.1.201.36 304
    36 195.154.172.53 200



