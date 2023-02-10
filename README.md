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
-------------------------27-01-2023
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
<!-- 

### <li> D4
### <li> D5
### <li> D6
### <li> D7
### <li> D8
### <li> D9
### <li> D10
### <li> D11
### <li> D12
### <li> D13
### <li> D14
### <li> D15
### <li> D16
### <li> D17
### <li> D18
### <li> D19
### <li> D20

-->
