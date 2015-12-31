# reverse-engineering
Experiments in reverse engineering

gcc -S foo.c  # Compile something into ASM

gcc -c -g -Wa,-a,-ad foo.c > foo.lst
