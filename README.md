# Linuxx-LP
<hr>

### <li>🟢 D1
    cal- calender
    cal 2023- 2023 calener
    echo- for ptinting

    date --date="2 year ago"
    touch-empty file create
    cat- create file for writing 


    history 8  =>check previous 8 executed command
    history -c =>clear history

    perform arthematic oprtation using expr and bc command-
    + expr 10 + 12
    - expr 12 - 10
    * expr 10 \* 10
    / expr 100 / 10

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
    mul=$(($a * $b))
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


    u=([1..9])
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

<!-- 
### <li>🟢 D12
### <li>🟢 D13
### <li>🟢 D14
### <li>🟢 D15
### <li>🟢 D16
### <li>🟢 D17
### <li>🟢 D18
### <li>🟢 D19
### <li>🟢 D20
### <li>🟢 D21
### <li>🟢 D22
-->
