---
layout: post
category : Linus  
analytics : false
title: Mix Commandline Tips 
tags : [tips ]
---
{% include JB/setup %}

##Outlook 
+ only show unread mails 	
		read:no  in search tabs 

##Sort 
+ number sort, and reverse the order
		sort -n -r

+ human readable sort 1K 2G, and sort by the second column
		sort -h -k 2
+ top 5 large files
		du -s * | sort -nr | head -5
+ sort based on two column 
		sort -n -k 6 -k 2 filename 
		sort -t: -k 6 -k 2 filename 

##Uniq 
+ count summary,  repeated lines only,  uniq lines only
		uniq -c
		uniq -u
		uniq -d
##Split 
+ This will output six 500-line chunks.
		split -l 500 myfile
+ 500 line, 000, 002
		split -l 500 -a 3 -d myfile prefix_
+ split 20M file, we can use k or m, prefix_aa prefix_ab
		split -b 20m my_file prefix_

##tar
		tar cvfz tarball.tgz  dir  --make tarball
		tar xvfz tarball.tgz       --extract from tarball 
		tar tvfz tarball.tgz       --list the files in tar ball

##Shell 
		!n  	--Will execute the line n of the history record.
		!-n 	--Will execute the command n lines back.
		!!  	--Will execute the last command. Same as !-1 or "up-arrow + return"
		!gzip   --will reexecute the most recent gzip command (string from the start)
		!$  	--is the last argument
		!:0     --is the previous command name
		!*      --is all the arguments
		!vim:$  --show the last vim command filename

## awk
+ General print 
		awk '$1>200'   -- only print lines which 1st column > 200
		awk '/Sanjay/' -- lines matching 'Sanjay'
		awk '$4 ~/Technology/'  --4th column match 'Technology'
		awk 'BEGIN { count=0;} $4 ~ /Technology/ { count++; } END { print "Total Number=",count;}'
+ Don't print $1/$2  
		awk '{$1=$2=""; print }' filename
		awk '{$1=$2=""}1' filename

##Mix lines 
+ delete lines which size is 0 
		lt | awk '{if($5==0) print $9}' | xargs -i rm {}
