## 😉if you will talk for 5 min you will have to give here presentation for 25 minutes & i will laugh from there.

## See children what you will do you will do nothing only i do everthing & you only listen.

# Linuxx-LP
<hr>
---check current directory

echo "$PWD"
/home/kalyan

### <li>🟢 D1
    cal- calender
    cal 2023- 2023 calener
    echo- for ptinting

    date --date="2 year ago"
    touch-empty file create
    cat- create file for writing 


    history 8  =>check previous 8 executed command
    history -c =>clear history

    //new line
    echo -e "you are \n good"
    output->you are
	    good
	
    //wait for input
    echo -e "enter age \n"
    read age
   


    perform arthematic oprtation using expr and bc command-
    + expr 10 + 12
    - expr 12 - 10
    * expr 10 \* 10
    / expr 100 / 10


     cat - cat command allows us to create files, view contain of file, concatenate files and redirect output in terminal or files.
    cat myfile             (read content of myfile)
    cat myfile1 myfile2     (read content of myfile1 and myfile2)   
    cat –n myfile1 myfile2      (display content with line number)
    cat >myfile         (create new file named myfile and write into it)

    Grep command--(search for parcitular word in string)
    grep -o "class" rt.txt




### <li>🟢 D2
 
    create 2 text file and 2 directory
    touch a.txt 
    touch b.txt
    mkdir AB
    mkdir FG

    rm a.txt 
    rmdir myDirectory

    bash ui.sh //goto directory  
    ls  //see list
    cd AB //goto AB directory
    cd .. //come back from directory
  
  
    Print and do sum of two number using shell script nano
    nano file_name.sh
      ->write 
      echo "hello"
      expr 10 + 19

    bash file_name.sh
    output->  
    hello  
    29

    variable in shell:- 
    #! /bin/bash
    a="Welcome all"
    b=12

    unsetting a variable (i want to clear the value given to the variable)
    a="Welcome all"
    unset a 
    echo a ->will print nothing  
  
  
### <li>🟢 D3 
    positional parameter- function jaise

    nano filename.sh 

    echo "name $1"
    echo "age $2"
    echo "fullname $3"

    bash filename.sh
    name
    age 
    fullname 


    chmod +x filename.sh   (for permission)
    ./filename.sh kalyan 22 mishra    (error de raha h filhaal)
    or 
    bash filename.sh kalyan 22 mishra

    name kalyan 
    age mishra
    fullname 22

### <li>🟢 D4 
    -eq  check for equality
    -ne inequality
    -lt less than
    -le less than or equal 
    -gt greater than 
    -ge greater than or equal 

    checking for equality ---
    nano fname.sh

    #! /bin/bash
    a=10
    b=20
    if [ $a == $b ]
    then 
        echo "a is equal to b"
    else
        echo "a is not equal to b"
    fi 

    bash fname.sh 
    output- a is not equal to b


    --------------sum of number using variable-
    #! /bin/bash
    a=10
    b=12

    expr $a + $b 
    expr $a \* $b
    expr $a / $b 

### <li>🟢 D5

    -------------sum of number using function 
    #! /bin/bash

    a="$1"
    b="$2"

    expr $a + $b 
    expr $a \* $b
    expr $a / $b 

    chmod +x fname.sh
    bash fname.sh 10 12

    ------------------------less than, greater than, less or greater, etc-

    #! /bin/bash
    a=10
    b=20

    if [ $a -lt $b ]
    then 
        echo "a is less than b"
    else
        echo "a is greater than b"
    fi 

    /*Multiple if statement */

    --------------------CASE SWITCH-------------

    #! /bin/bash
    vehicle=$1
    case $vehicle in
    "car")
    echo "rent of $vehicle is 100 dallar";;

    "van")
    echo "rent of $vehicle is 80 dallar";;

    "bibycle")
    echo "rent of $vehicle is 5 dallar";;

    "truck")
    echo "rent of $vehicle is 160 dallar";;


    *) 
    echo "unknown vehicle";;
    esac


    bash fanme.sh car  can k jagah pr van krke dekho
    

### <li>🟢 D6

    #! /bin/bash
    echo "Enter a number"
    num=$1
    case $num in 
    [0-9])
        echo "single digit";;
    [1-9][0-9])
        echo "double digit";;
    [1-9][0-9][0-9])
        echo "three digit";;
    *)
    echo "barka number lag rha h";;
    esac



    bash fanme.sh 12
    //https://unix.stackexchange.com/questions/179218/how-to-enter-the-condition-to-check-0-or-more-than-0-in-case

### <li>🟢 D7

    #! /bin/bash
    echo "Enter a number"
    num=$1
    case $num in 
    [0-9].[0-9])
        echo "decimal";;
    *)
    echo "invalid";;
    esac

    bash fanme.sh 1.2

    --------------------------
    for loop in shell------

    #! /bin/bash
    for i in 1 2 3 4 5
    do
        echo "hello $i"
    done

    bash fname.sh 
    print ->5 times hello1..till 5



    #! /bin/bash
    for i in {1..20}
    do
        echo "hello $i"
    done

    bash fname.sh 
    print ->5 times hello1..till 20
    
### <li>🟢 D8

    use for loop increment the value by 5
    #! /bin/bash
    for i in {1..20..5}
    do
        echo "hello $i"
    done



    decrement the value by 4
    use for loop increment the value by 5
    #! /bin/bash
    for i in {20..1..4}
    do
        echo "hello $i"
    done



    simple for loop

    #! /bin/bash
    for((i=0;i<=7;i++))
    do
        echo "$i"
    done
    
    -------------------factorial-----------------------

    #! /bin/bash
    ans=1
    for((i-=1;i<=5;i++))
    {
        ans= $((ans * i))
    }
    echo "$ans"

    120

    ------while loop------- (-le less then)

    #! /bin/bash
    x=1
    while [ $x -le 5 ]
    do
        echo "welcome $x times"
    x=$(($x+1))
    done



    -gt  (greater then)
    #! /bin/bash
    x=5
    while [ $x -ge 5 ]
    do
        echo "welcome $x times"
    x=$(($x-1))
    done

### <li>🟢 D9

    -ge  (greater then equal)

    #! /bin/bash
    x=5
    while [ $x -ge 5 ]
    do
        echo "welcome $x times"
    x=$(($x-1))
    done

    --------------------take two numer and multiply

    nano file.sh

    #! /bin/bash
    a=$1
    b=$2
    mul=$(($a * $b))  //OR mul=$((a*b))
    echo $mul

    or 
    expr $a \* $b 

    chmod +x file.sh
    bash file.sh 3 4

    --------------------new line print 
    echo -e "hwllo \n world"
    hello
    world

    echo "hwllo \n world"
    hello \n world

### <li>🟢 D10
    --------------------(sleep system call )method count decrement by 1 
    #! /bin/bash
    count=5
    while (( count>0 ))
    do 
    echo -e "$count\n"
    sleep 1
    (( count-- ))
    done

    output->after 1 1 second print from  5 to 1


    ---------compatiblity bracket only with operator-----

    #! /bin/bash
    echo -e "Please enter age: \n"
    read age
    if [ "$age" -gt 18 ] && [ "$age" -lt]
    then
    echo "valid age"
    else
    echo "invalid age"
    fi




    a=20
    b=100
    if (( $a < $b ))
        then
            echo "a is less than b"
        else
            echo "b is not less then a"
    fi
    ------------&& within comment-----------

    use -a to add && operator in single comment
    range=10
    if [$range -gt 20 -a $range -lt 30]
    
### <li>🟢 D11

    ------------------array---------------------------

    #! /bin/bash
    name[0]="this"
    name[1]="name"
    name[2]="simple"
    echo "output: ${name[0]}"


    bash ab.sh
    this


    print all element
    #! /bin/bash
    name[0]="this"
    name[1]="name"
    name[2]="simple"
    echo "output: ${name[@]}"

    bash ab.sh
    this name simple


    u=({1..9})
    echo "${u[@]}"

    output->1 2 3 4 5 6 7 8 9 10


    u=({a..z})
    output-> a se z tak


    u=({a..z..Z})


    #! /bin/bash
    arr= ( "hello" 'thi' 34 34.3)
    echo "${arr[@]}"


    --------concatename the array-------------
    a=( 1 2 3 4 5 )
    b=( 3 4 5  6 )
    x=("${a[@]}" "${b[@]}")
    echo "${x[@]}"

    output-1 2 3 4 5 3 4 5  6


    print length of array 
    echo "${#x[@]}"

    print index of array
    echo "${!x[@]}"


    #! /bin/bash
    arr=(1 2 3 4 5 6 7 8)
    echo "Before addition of ele: ${arr[@]}"
    echo "Length is: ${#arr[@]}"
    arr [3]=23
    echo "After modefy at index 3: ${arr[@]}"
    arr[${#arr[@]}]=34  
    echo "After addition of ele: ${arr[@]}"

### <li>🟢 D12
    
    print array ele using while------------------------
    #! /bin/bash
    arr=( 1 3 2 5 3 6 )

    1=0
    echo "size is: ${#arr[@]}"
    while [ $i -lt ${#arr[@]} ]

    do
    echo ${arr[$i]}
    i=$(($i+1) )
    done
    ---------------------------------------------

    Q.wap in shell to sort the element in an array

    array=(5 3 8 1 4 6 9 7 2)
    # Sort the array
    sorted_array=($(echo "${array[@]}" | tr ' ' '\n' | sort -n))

    # Print the sorted array
    echo "Sorted Array: ${sorted_array[@]}"


    Q.wap in shell to create two files with cat and concatenate the content into 3rd file
    touch a.txt b.txt c.txt
    cat >>a.txt  =>This is a.txt file

    cp a.txt b.txt  //copy from file a.txt to b.txt
    cat b.txt  =>output->This is a.txt

    cat a.txt b.txt>>c.txt

    cat c.txt  //printing c.txt file
    output->
    This is a.txt file
    This is a.txt file

    Q.wap in shell to print the element of an array in reverse order
    =>nano file.sh

    #!/bin/bash
    array=( 5 3 8 1 4 )
    size=${#arr[@]}

    ((size--))
    while (( $size>=0 ))
    do 
        echo ${arr[size]}
        ((size--))
    done


    bash file.sh
    4
    1
    8
    3
    5

### <li>🟢 D13

    ---------------------function----------
    #! /bin/bash
    fun()
    {
        echo "hello all"
    }
    fun

    bash filename.sh
    -------passing parameter to function---------------------
    #! /bin/bash
    fun()
    {
        echo "hello all $1  $2"
        echo "hello you $1  $2"
    }
    fun abc bcd

    bash filename.sh
    output->hello all abc bcd
            hello you bcd abc
     
     
### <li>🟢 D14
    #! /bin/bash
    fun ()
    echo "$1 $2 $3 $4 $5"

    val=$1
    val2=$2
    val3=$3
    val4=$4
    val5=$5
    echo "Your entered values are:
    fun $val $val2 $val3 $val4 $val5

    chmox +x filename.sh
    bash filename.sh 1 2 3 4 5



    or 
    #! /bin/bash
    fun ()
    echo "$1 $2 $3 $4 $5"

    echo "enter five number"
    read val val2 val3 val4 val5
    echo "Your entered values are:
    fun $val $val2 $val3 $val4 $val5


    chmox +x filename.sh
    bash filename.sh

    output->
    enter five number:
    1 2 3 4 5

    -----------------------------------------
    Q. WAP ti define 3 functions and 2nd one statement should not get printed even on function call
    ! /bin/bash
    Fun () {
    cho "fun1"

    Fun1( ) {
    echo "fun2"
    }
    Fun2( ){
    echo "fun3"
    }
    Fun3 ( ) {
    echo "fun4"
    }

    Fun1
    un2
    Fun3
    exit
    Fun


    output->
    fun2
    fun3
    fun4

    fun1 will not get printed


### <li>🟢 D15

    ----------------perform m=sum and multiply--------------------------
    sum(){
        expr 1 + 2
    }
    mul(){
        expr 34 \* 34
    }
    sum 
    mul 
    -------------------perform bodmas using expr and BC command-----
    bc command is used for command line calculator. basic mathematic calcualtor

    ! /bin/bash
    sum( ) {
    expr $1 + $2
    echo "$1 + $2" | bc
    }

    subs( ) {
    expr $1 - $2
    }

    mul(){
    expr $1 \* $2
    }

    division( ){
    expr $1 / $2
    }

    sum 12 23
    subs 34 23
    mul 23 23
    division 24 12

### <li>🟢 D16
    -----------------------MID term question--------------------

    Q. WAP in shell and print 3 different date in function


    Q. find avg of the number from 1 to 10 using function

    avg_of_num(){
    i=1
    while [ $i -le 10 ]
    do
    sum=$(($sum + $i))
    i=$(($1+1))
    done
    avg=$(($sum / 10))
    echo "avg is: $avg"
    }
    avg_of num


    Q. WAP to find even and odd number using function

    Q. WAP in shell and implement nested function


    Q. WAP in shell scripting and perform recursion


    ----------------------
    https://www.cibgp.com/article_10898_98b20a1dbfbdb8f7084003b4a035911d.pdf
    https://www.researchgate.net/publication/320547139_E-Commerce_Merits_and_Demerits_A_Review_Paper
    file:///C:/Users/Asus/Downloads/A_REVIEW_PAPER_ON_E_COMMERCE%20(1).pdf
    https://www.sciencedirect.com/science/article/abs/pii/S0167739X21002211
    https://www.sciencedirect.com/science/article/pii/S1110016823000741

    mak ed, clos ed, 
    --------------------------Signal-------------------
    kill-l => see list of singnal 


    echo "pid is $$"
    while(( count < 10))
    do
        sleep 3
        ((count ++))
        echo "$count"
    done

    exit 0 


    using for loop

    echo "pid is $$"
    for(( count=10; count>=1; count-- ))
    do
        sleep 3
        echo "$count"
    done

    use ctrl+c to break it will call SIG INT 

### <li>🟢 D17
    -----------------count total parameter passed----------------------------------
    #!/bin/bash
    expr $1 + $2
    echo "total arg are $#"

    bash ab.sh 10 20 30
    output=> 
    30
    total arg are 3


    Asychronous signal- user given the signal
    synchronous signal- system given signal
    ------------------------Trap signal-------
    #!/bin/bash

    trap "echo exit1 is detected" 0
    echo "hello all"
    trap "echo second exit detected"

    output->
    hello all
    echo second exit detected

    on successful execution of program trap priority wala happen

    ---------------------------------
     touch-create
     pwd-where located
     ls ab.txt  =>check if file exist

     trap "rm ab.txt" sigint
     while ((count<5))
     do
        sleep 2
        echo "$count"
        ((count++))
     done

     ----------------------------------------

     #! /bin/bash
     trap "echo exit command is detected" SIGKILL
     echo "pid is $$"
     while((count<9))
        do
         sleep 2
         ((count++))
         echo "$count"
    done
    exit 0

    ------------------delete file when exit command ctrl+c pressed--------------------------
    create file abb.txt
    check directoty using pwd

    #! /bin/bash
    a=/root/abb.txt
    trap "rm -f $a; exit" 0 2 15
    echo "pid is $$"
    while((count<8))
    do
        sleep 2
        ((count++))
        echo "$count"
    done
    exit 0


    bash filename.sh
    ctrl+c  =>file have been deleted check using ls


### <li>🟢 D18
    -------------------user enter a file and check file exit or not---------------------------------
    touch tt.sh

    nano ab.sh


    -e  is for filename
    -d for directory
    -s check if file is empty


    #!/bin/bash
    echo -e "Enter the name of file: \c"
    read filename 
    if [ -e $filename ]
    then echo "$filename exist"
    else
    echo "$filename doesn't exist"
    fi


    explore- https://www.geeksforgeeks.org/shell-scripting-test-command/

    ------------------substring---------------------
    str="hello students"
    substr=${str:1:5}
    echo "$substr"


    output->ello

### <li>🟢 D19
---------------END TERM paper Swaal leak-------------------
    Q. WAP to print cube of a number

    #!/bin/bash
    a=5
    a=$(( $a * $a * $a ))
    echo $a

    Q. WAP to generate table of a number

    a=2
    while((i<=10))
    do
        expr $a \* $i 
        ((i++))
    done


    Q. Count number of argument and if it is >5 print "Too many argument passed"

    #!/bin/bash
    expr $1 + $2 + $3 + $4 + $5
    arg=$#
    if [ $arg -gt 5 ]
    then
       echo "Too many arguments"
    else
        echo "5 arg are there"
    fi

    bash ss.sh 1 2 3 4 5 7
    output->
    22
    Too many arguments


    Q. check if character is vowel or not

    str="a"
    if [[ $str == *[AEIOUaeiou]* ]]
    then
      echo "Vowel"
    else
        echo "consonent"
    fi


    output->a


    Q. WAP to print permissions of a directory
    -> ls -l directory

    mkdir temp
    ls -l temp
    output-> total 0

### <li>🟢 D20
    Q. Write a program in shell script and change a default file permission of a directory
    (file owner should get read, write, execute)
    (Group member should get execute)
    (Other should get read only)
    ans->https://www.pluralsight.com/blog/it-ops/linux-file-permissions


    Q. Write a program in shell and find the area of a circle
    r=10
    echo "Area of circle is: ";
    echo "3.14 * $r * $r" | bc


    Q. Write a program in shell and explain the functionality of different command line ($1 $0 etc)
    echo $0 ->sh 
    echo $$ PID
    echo *  saare files name

    Q. Write a program in shell and implement if else and concatenate two string
    a=$1
    b=$2
    if [ $a -ge $b ]
    then
    echo "A is greater than b"
    else
    echo "A is not greater then b"
    fi


    a="Hello"
    b="World"
    c="$a $b"
    echo $c

### <li>🟢 D21
    -------------------debug------------------------
    #!/bin/bash
    read -p "enter value " val
    if [ "$val" -gt "$a" ]
    then
    echo "positive number entered"
    else
    echo "input not positive"
    fi

    for debug-> bash -v abb.sh

    bash -n abb.sh  =>it will show all the symentic errors


    #!/bin/bash
    read -p "enter value " val
    if [ "$val" -gt "$a" ]
    then
    ''echo "positive number entered"  #this line has error
    else
    echo "input not positive"
    fi

    for debug-> bash -v abb.sh


    bash -n abb.sh


### <li>🟢 D22
    -------------------locate logical error
    #!/bin/bash
    a=4
    b=8
    c=$((a+B))
    echo $c

    bash filename.sh
    output->4 but it desired is 12 so, cant locate this logical error 

    so use bash -u filename.sh
    output- B: unbounded variable

    ------------------------Question on all flags-------

    Q. Write a program in shell invoke -n -v -x -u

    #!/bin/bash
    a=4
    b=8
    c=$((a+B))
    echo $c


    bash -n filename.sh
    no output bcoz -n doesnt locate logical it only give symentic err


    bash -u filename.sh
    B: unbounded variable


    bash -v abb.sh
    output->
    #!/bin/bash
    a=4
    b=8
    c=$((a+B))
    echo $c
    4


    bash -x filename.sh
    output-> only variable wala cheezen displayed (where var is getting expended)
    a=4
    b=8
    c=4
    echo 4
    4

    -----------------combning flags---------------------------
    #!/bin/bash
    read -p "enter value:" val
    a=0
    set -x
    if [ "$val" -gt "$a" ]
        echo "positive num entered"
    else
        echo "input not positive"
    fi
    set +x
    echo "script ended"

    ---------------------------------------------------

    Q. write a program in shell and invoke multple if
    #!/bin/bash
    read -p "enter value:" val 
    a=0
    set -x
    if [ "$val" -gt "$a" ]
        echo "positive number entered"
    else if [ "" ]
    

### <li>🟢 D23
    --------------------------------------ETE-----------------------------------------------------
    Q. WAP when user entered if it is even or odd
    #!/bin/bash
    a=$1
    if [ $a % 2 == 0 ]
        then
            echo "Even"
    else
        echo "odd"

    ----------------------

    Q. WAP to implement the function of any 20 command ls-l ls-lsh etc.
    Q. WAP to implement to check whether user is working in file or Directory.

    Q. WAP to reverse the string "we are working very hard"

    Q. WAP to generate table of 20 and stop the process at 20 * 3
    #!/bin/bash
    a=20
    i=1
    for((i=1; i<11; i++))
    do
        if [ $i == 3 ]
        then
          echo "stopped at 3*20"
          exit
      else
        expr $i \* $a 
      fi 
    done

### <li>🟢 D24
    ----------------------

    Q. WAP to trap any signal

    #!/bin/bash
    trap "echo exit is detected" 0
    echo "Hello all"
    exit 0

    ----------------------
    Q. WAP to display content of a file without cat command
    Q. what is an IPR (Itellectual propeitery rights)
    Q. Write a shell which accept two directory as an input and delete only those file from A2 that has identical namees in A1
    Q. implement the functionliay of and or not
    Q. WAP to calculate the gross salary of teaching and non teaching staff


    Q. WAp in shell and display the frequency of hello in the file
    touch ab.sh
    cat>>ab.sh 
    This is a simple hello file which is hello in the helo world of hello
    cat<ab.sh 
    output->aayega



### <li>🟢 D25
    ----------------------
    Q. WAP to find the sum of digits of a number
    #!/bin/bash
    a=1234
    sum=0

    while [ $a -ge 0 ]
    do
        sum=$((a % 10 + sum))
      a=$((a / 10))
    done
    echo $sum

    ----------------------

    Q. WAP to print "good morning" and "good afternoon" basis of time

    ------------------------------

    Q. WAP to reverse a number

    num=12345
    rev=0
    while [ $num -gt 0 ]
    do 
    rev=$(($num % 10 + $rev * 10))
    a=$(( $a / 10 ))
    done 
    echo $rev

    ------------------------------cA-----------------------
    heading 14, text size 12 ROMAN TIMES NEW
    chapter 1. Introduction
    Objective 
    System description (include figures and explain)

    man ls --ls manual

### <li>🟢 D26

    --------------------create man page of sigint-----------

    https://pastebin.com/q4FGD7R7


    -------TASK BLACK FRIDAY--------
    1. RCB and CBS demonestrate using any ubuntu program
    2. Handling multiple source file using make
    3. DEbugging using GDB


    ---------------GIT AND GITHUB
    issue solved
    https://itslinuxfoss.com/fix-temporary-failure-resolving-archive-ubuntu-com-error/

    sudo apt-get install git

    git --version

    ----------------uploading file on github----------------------

    git config --global user.name "kalyanMisrhra"
    git config --global user.email "user@gmail.com"

    git config --list 
    git clone https://github.com/thekalyan001/TempP
    cd TempP
    touch file.txt
    git add txx.txt
    git status txx.txt

	<!-- 
	=======
	    git commit -m "new commit"
	    git push origin main
	    username:*********
	    pss: ********token generated
	<!-- 
### <li>🟢 D27

	---------adding changes to any file and push to server-------------------

	touch file.txt  (make change)
	git add txx.txt
	git status txx.txt

	git commit -m "new commit"
	git push origin main
	username:thekalyan001
	pss:"TOKEN GENERATED"


	--------changing on server file making changes in lcoal (github)------------------------------
	open any file on github->edit the content of file =>commit change

	git pull origin main


	-------------------backtrack the commited changes-------------
	touch temp
	git add temp
	git status temp
	git reset temp


	----remove pushed file from server--------


	--------------BRANCHING-----------
	-check current branch name0
	git branch  
	(* denotes which branch youre curently in)

	----'create branch'
	git branch Brnach_name

	----'switch to another branch'
	git checkout Branch name

	---'push branch to remote repository'
	git push origin new_branch1


	---'delete branch'
	git push origin --delete new_branch1

### <li>🟢 D28
	---------------------TAGS----------------------------------

	-----------add tag-------------------
	git clone ......xyz
	cd xyz
	git pull  //bring all changes from remote to local
	git tag
	git tag -a v1.5 -m "my tag"
	git push origin v1.5 

	------------------
	sudo apt-get install gdb

	nano swap.cpp
	write program---
	g++ -g swap.cpp -o swap
	./swap ya ./a.out



	g++ -g swap.cpp -o swap
	b main
	b swap
	start

	f
	n- new line
	bt- back trace previous block me go

	---------------------------------------------
	
### <li>🟢 D29
        -------------gcc progeram
	nano add.cpp

	#incldue<iostream>
	using namespace std;
	int main(){
	  int a=10;
	  cout<<"a is: "<<a<<endl;
		return 0;
	}

	g++ add.cpp
	g++ -g add.cpp -o addOutput
	./a.out  or ./addOutput



    -----check if file exists
    if [[ -f "/home/kalyan/ab.sh" ]] ;
    then
     echo "File exist"
    else
     echo "File doesn't exist"
    fi

    --check if folder exists
    if [[ -d "/home/kalyan/abc" ]]


    -----Chekc if file is regular file or dir
    #!/bin/bash
    FILE=$1
    if [ -f $FILE ]
      then
        echo "It is reguler File"
        exit 0
    elif [ -d $FILE ]
       then
         echo "It is directory"
         exit 1
     else
        echo "Another type"
        exit 2
    fi

    bash filename.sh  /home/kalyan/ab.cpp  ->It is reguler File”
    bash filename.sh  /home/kalyan/Desktop ->It is directory



    --------------DEBUGGING------------
    commands->
    breakpoint b
    list       l
    frame      f
    next       n
    step       s
    backtrace  b
    print      p
    info       i
    watch b



    create ->swap.cpp

    #incldue<iostream>
    using namespace std;
    void swap(int x, int y){
        int t=x;
        x=y;
        y=t;
    }
    int main(){
        int a=10, b=5;
        swap(a,b);
        cout<<a<<" "<<b<<endl;
        return 0;
    }

    
    g++ -g swap.cpp -o swap
    gdb swap

    b main  //1st breakpoint on main
    b swap  //2nd breakpoint on swap

    start
    watch a
    watch b
    l  (to print the program)
    n  (next line)



<!-- 
### <li>🟢 D29
-->
