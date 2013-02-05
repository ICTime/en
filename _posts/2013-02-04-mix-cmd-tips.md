---
layout: post
category : Linus  
analytics : false
title: Mix Commandline Tips 
tags : [tips ]
---
{% include JB/setup %}

## Outlook 
+ only show unread mails 	
		read:no  in search tabs 

## Sort 
+ number sort, and reverse the order
		sort -n -r

+ human readable sort 1K 2G, and sort by the second column
		sort -h -k 2
+ top 5 large files
		du -s * | sort -nr | head -5
+ sort based on two column 
		sort -n -k 6 -k 2 filename 
		sort -t: -k 6 -k 2 filename 

