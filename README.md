# reverse-engineering
Experiments in reverse engineering

gcc -S simple.c  # Compile something into ASM

gcc -c -g -Wa,-a,-ad foo.c > foo.lst


### From the author

#### Use the following to compile to Intel instructions

    gcc -S -masm=intel simple.c
    cat simple.s  | grep -v "\.[A-z]"  ## show the asm without the . lines
