Download Link: https://assignmentchef.com/product/solved-cse-333-operating-systems-programming-assignment-1-2
<br>
<strong> </strong>(20 pts) A palindrome is a word, a phrase, or sequence that reads the same backwards as forwards. Write a shell script that will take one command line argument as string and decide if it is a palindrome. For example:

<strong>Ex:</strong>

<strong>$ ./myprog1.sh “apple” apple is not a palindrome</strong>

<strong>Ex:</strong>

<strong>$ ./myprog1.sh “ey edip adanada pide ye”  ey edip adanada pide ye is a palindrome</strong>

Your program should work on both lowercase and uppercase letters.

<strong>Ex:</strong>

<strong>$ ./myprog1.sh “Madam”</strong>

<strong>        Madam is a palindrome</strong>

<ol start="2">

 <li>(15 pts) Write a shell script that takes an optional pathname as parameter. If your program is run with no parameters, it will create a directory named <strong>cprogs</strong> under current working directory and move all of the files whose name ends with .c to this directory. If your program is run with an argument, it will create a directory names <strong>cprogs </strong>under given path and move all of the files whose name ends with .c under given path to this directory. For example:</li>

</ol>

<strong>Ex:</strong>

<strong>$ ./myprog2.sh </strong>

<strong>A directory named cprogs is created under current working directory.</strong>

<strong>All the files whose name ends with .c in the current working directory are moved into cprogs directory. </strong><strong>Ex:</strong>

<strong>$ ./myprog2.sh /home/zuhal/Desktop A directory named cprogs is created under /home/zuhal/Desktop. All the files whose name ends with .c in /home/zuhal/Desktop are moved into cprogs directory.</strong>

<ol start="3">

 <li>(15 pts) Write a shell script that will take two integer arguments. The first argument must be greater than the second one. The difference between the two arguments must be an even number. Then your program will draw a hollowed square with the first argument being the side of outer square and the second one being the side of the inner square. For example:</li>

</ol>

<strong>Ex:</strong>

<strong>$ ./myprogr3.sh 7 5</strong>

<strong>*******</strong>

<ul>

 <li><strong>*</strong></li>

 <li><strong>*</strong></li>

 <li><strong>*</strong></li>

 <li><strong>*</strong></li>

 <li><strong>*</strong></li>

</ul>

<strong>*******</strong>

<strong>Ex:</strong>

<strong>$ ./myprogr3.sh 8 2</strong>

<strong>********</strong>

<strong>********</strong>

<strong>********</strong>

<strong>***  ***</strong>

<strong>***  ***</strong>

<strong>********</strong>

<strong>********</strong>

<strong>********</strong>

<ol start="4">

 <li>(20 pts) Write a shell script that takes a wildcard and an optional pathname as an argument. If your program is run only with the wildcard as an argument, then it will search for the words that matches with this wildcard inside all the files whose name ends with .txt under current working directory and substitute them with their uppercase versions. If your program is run with two arguments, one being the wildcard and the other being the pathname, then your program search for the words that matches with this wildcard inside all the files whose name ends with .txt under given pathname and substitute them with their uppercase versions. Note that all of the occurrences of the same word will also be changed. For example:</li>

</ol>

<strong>Ex:</strong>

<strong>$ ./myprog4.sh “ek*”  The word “ekin” inside test.txt is substituted with “EKIN”.</strong>

<strong> The word “ekmek” inside test.txt is substituted with “EKMEK”.  The word “ekleme” inside deneme.txt is substituted with “EKLEME”.</strong>

<strong>Ex:</strong>

<strong>$ ./myprog4.sh “an*e” /home/zuhal/Desktop</strong>

<strong> The word “anne” inside /home/zuhal/Desktop/aile.txt is substituted with “ANNE”.</strong>

<strong> The word “anne” inside /home/zuhal/Desktop/aile.txt is substituted with “ANNE”.  The word “antre” inside ev.txt is substituted with “ANTRE”.</strong>

<ol start="5">

 <li>(20 pts) Write a shell script that takes an optional pathname as an argument and a -R option. If your program is run with no arguments, then it will find all the files whose size is zero under current working directory and ask the user to delete them one by one. If your program is run with a pathname as an argument, then it will find all the files whose size is zero under given pathname and ask the user to delete them one by one. If -R option is given, then your program will work recursively. For example:</li>

</ol>

<strong>Ex:</strong>

<strong>$ ls -l</strong>

<strong>-r—w—- 1 std std 13107 Jun 20 2005 cask-of-amontillado.txt</strong>

<strong>-rw——- 1 std std 0 Jun 20 2005 french.txt drwx—— 14 std std 456 May 25 2007 shakespeare -rw——- 1 std std 0 Jun 20 2005 trees-and-other-poems.txt</strong>

<strong>$ ls -l shakespeare</strong>

<strong>-rw——- 1 std std 456 Jun 20 2005 barleby-scrivener.txt</strong>

<strong>-rw——- 1 std std 0 Jun 20 2005 calaveras-county.txt</strong>

<strong>$ myprogr5.sh -R</strong>

<strong>Do you want to delete french.txt? (y/n): y</strong>

<strong>1 file deleted</strong>

<strong>    Do you want to delete trees-and-other-poems.txt? (y/n): n</strong>

<strong>Do you want to delete calaveras-county.txt? (y/n): y</strong>

<strong>1 file deleted</strong>

<strong>Ex:</strong>

<strong>$ ls -l /home/zuhal/Desktop</strong>

<strong>-rwx—— 1 std std 0 Jun 20 2005 alice-in-wonderland.txt</strong>

<strong>-rw——- 1 std std 496769 Jun 20 2005 hawthorne.txt</strong>

<strong>-rw——- 1 std std 172541 Jun 20 2005 looking-glass.txt</strong>

<strong>drwx—— 14 std std 0 May 25 2007 stories -r——– 1 std std 0 Jun 20 2005 song-of-hiawatha.txt</strong>

<strong>$ myprogr5.sh /home/zuhal/Desktop</strong>

<strong>Do you want to delete alice-in-wonderland.txt? (y/n): y</strong>

<strong>1 file deleted</strong>

<strong>    Do you want to delete song-of-hiawatha.txt? (y/n): y</strong>

<strong>1 file deleted</strong>

Note that the directories are not deleted. Note also that you can use option and argument at the same time.

<ul>

 <li><strong>Bonus:</strong>You will get 10% extra credit if your program supports a <em>Menu</em> including all questions above. Example:</li>

</ul>

<strong>$ ./myprog.sh  </strong><strong>Please select an option:</strong>

<ol>

 <li><strong>Check for palindromes</strong></li>

 <li><strong>Move .c files</strong></li>

 <li><strong>Draw hollowed square</strong></li>

 <li><strong>Uppercase conversion</strong></li>

 <li><strong>Delete files</strong></li>

 <li><strong>Exit</strong></li>

</ol>

These options must be printed inside a loop until “Exit” option is selected. When user enters one choice, you should ask for the arguments if that option requires any.

<strong><em>Notes:</em></strong>

<ul>

 <li>You are required to consider all necessary error checking for the programs.</li>

 <li>No late homework will be accepted.</li>

 <li>In case of any form of <strong>copying and cheating</strong> on solutions, all parties will get <strong>ZERO</strong> You should submit your own work. In case of any forms of cheating or copying, both giver and receiver are equally culpable and suffer equal penalties.</li>

 <li>You have to work with a partner. Your partner will not be changed throughout the semester.</li>

 <li>(10 pts) You are required to submit a minimum 2-pages report and commented code (via e-mail: <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="5020223f3a3533242310373d31393c7e333f3d">[email protected]</a>).</li>

 <li>Your report should include explanations about implementations with screenshots of your sample executions. Your implementation detail should be provided in the source code comment.</li>

 <li>Please put your COMMENTED source codes and project report in a zip file and make sure that your zip file name contains your student IDs!</li>

</ul>

Ex: 150713852_150713853_Project1.zip

<ul>

 <li>If after 3 projects, your overall grade is higher than 100, it will be considered as 100.</li>

</ul>