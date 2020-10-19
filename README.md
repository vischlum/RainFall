# Rainfall
- [ISO](https://projects.intra.42.fr/uploads/document/document/1570/RainFall.iso)
- [PDF](https://cdn.intra.42.fr/pdf/pdf/9818/en.subject.pdf)

## Description
Second projet de la branche sécurité de 42 Born2Code.  
On démarre en se connectant en SSH avec `level0:level0`. À chaque niveau, il s'agit ensuite d'exploiter les failles du binaire `levelX` pour obtenir le mot de passe de l'utilisateur `levelX+1`.

Ce projet a été réalisé par [Louise Pieri](https://github.com/lpieri) et [Vincent Schlumberger](https://github.com/vischlum).

## Sommaire
- [Level 0](/level0/) : désassemblage basique avec `gdb`
- [Level 1](/level1/) : [*buffer overflow*](https://en.wikipedia.org/wiki/Buffer_overflow) pour écraser l'eip
- [Level 2](/level2/) : injection de [*shellcode*](https://en.wikipedia.org/wiki/Shellcode)
- [Level 3](/level3/) : [*format string*](https://en.wikipedia.org/wiki/Uncontrolled_format_string) pour écraser la valeur d'une variable
- [Level 4](/level4/) : *format string* permettant d'écrire plus que un ou deux octets
- [Level 5](/level5/) : *format string* pour rediriger l'exécution
- [Level 6](/level6/) : [*heap overflow*](https://en.wikipedia.org/wiki/Heap_overflow) basique
- [Level 7](/level7/) : utilisation combinée de deux *heap overflows* pour rediriger l'exécution
- [Level 8](/level8/) : *heap overflow* avec un [*stale pointer*](https://en.wikipedia.org/wiki/Stale_pointer_bug)
- [Level 9](/level9/) : désassemblage d'un binaire C++
- [bonus 0](/bonus0/) : injection de *shellcode*
- [bonus 1](/bonus1/) : utilisation d'un [*integer overflow*](https://en.wikipedia.org/wiki/Integer_overflow)
- [bonus 2](/bonus2/) : exploitation d'une faille de [`strcat`](https://linux.die.net/man/3/strcat)
- [bonus 3](/bonus3/) : exploitation d'une faille logique du binaire (recours à `atoi(argv[1])` pour clore la chaîne de caractère)
