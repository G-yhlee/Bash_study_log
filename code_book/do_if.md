```bash
    function do_if {
        VAR1="var1"
        VAR2="var2"
        if [ "$VAR1" = "$VAR2" ]; then
            echo "Strings are equal."
        else
            echo "Strings are not equal."
        fi
    }

```