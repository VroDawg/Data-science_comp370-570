## TASK 3:

## -How big is the dataset? About 4.7 megabytes in size.  Used ls -lh clean_dialog.csv

## -What’s the structure of the data? (i.e., what are the field and what are values in them) There are 4 attributes/columns labeled: 
## "title","writer","pony","dialog"     Used head -n 1 clean_dialog.csv
## -How many episodes does it cover? 197 episodes Used csvtool namedcol title clean_dialog.csv | tail -n +2 | sort -u | wc -l

## -During the exploration phase, find at least one aspect of the dataset that is unexpected – meaning that it seems like it could create issues for later analysis
## There are many episodes that share the same name but are different parts. One could interpret this as the same episode partitioned. So an issue would become wether we consider them as a unique single episode, or individual distinct ones.
