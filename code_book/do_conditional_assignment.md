```bash
function ternary_operator_is_one {
    a=$(( $1 == 1 ? 1 : 0 ))
    echo $a
}

```