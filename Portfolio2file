#!/bin/bash
#Joseph Parker
#10496326

sed -e 's/,/\t Height: /'\
    -e 's/,/\t Width: /'\
    -e 's/,/\t Area: /'\
    -e 's/,/\t Colour: /'\
    -e 's/^/Name: /'\
    -e '1d' rectangle.txt > rectangle_f.txt

#Using multiple statements through -e (meaning multiple sed statements can be applied).

#The s/ is followed by a comma as that is what is dividing the data. The first line selects
#the first comma and replaces it with the text 'Height :'. Just before that, the \t is added
#which allows for a tab break/space. This is to hep with formatting. The line is ended with
#a / to signal the end of that specific sed line. It is followed by a \ to indicate that it's
#the end of 1 of multiple sed statements. The second, third, and fourth sed statements follows
#the same format as the first.

#The -e 's/^/Name: /'\ line is to put the string 'Name: ' at the start of every line. The ^
#character denotes the start of the line.

#Finally, the '1d' in the final line of the code means to delete the very first line of
#rectangle.txt. The output is then saved to rectangle_f.txt.

exit 0
