# payload-mimikatz-procdump-for-rubber-ducky:
 A payload for extract the passwords of a windows computer with mimikatz & procdump.

# Requeriments:
 1. Rubber ducky
 2. Twin duck firmware
 3. Any tool for compiling mimikatz.
 4. java

# Instructions:
 1. Compile mimikatz with your compiling tool.
 2. Edit the `inject.txt` for fitting better to your attack, the things you __must__ change are explained with comments for understanding better what you have to change, but not only the important things to change are explained ;).
 3. Now we can compile the `inject.txt` file, only run this command in the path of the inject.txt with your terminal: `java -jar ducky.jar -i inject.txt -o inject.bin` if your target doesn't use the US keyboard, you will need to look into the propierties folder for your target's keyboard, then you have to run this command instead: `java -jar ducky.jar -i inject.txt -o inject.bin -l HERE_THE_PATH_TO_THE_KEYBOARD_LANG_FILE`.
 4. Move __all__ files to your rubber ducky micro SD card.
