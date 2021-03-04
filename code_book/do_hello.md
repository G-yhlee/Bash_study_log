```bash
function do_hello {
    echo 'hello'
}
function do_hello2 {
    var='hello'
    echo $var
}

function do_hellos {
    for i in "hello1" "hello2" "hello3" ;
    do echo $i;
    done
}

function get_hello {
    var=$1
    echo 'hello '$var
    echo "hello $var"
}

function get_hellos {
    for i in $@ ;
    do echo "hello "$i;
    done
}

function do_high_order_hello {
    echo "high_order_hello start" 
    $1 $2
    # do_high_order_hello get_hello world
}

# 망가진 펑션
function do_high_order_hello2 {
    # get_hello
    echo "high_order_hello2 start" 
    var=($1 $2) # d
    echo $var
}

```