# waterfilling
Host the Tor software with the waterfilling branch, a prototype of the
waterfilling technique implemented in Tor.

This source code  has been used to run tests in shadow for the research
presented in paper '' Waterfilling: Balancing the Tor network with
maximum diversity ''.

To look at the changes (git diff from tor-0.2.6.7):

\+ -  
31 0 src/common/util.c  
7 0 src/common/util.h  
2 0 src/or/config.c  
432 26 src/or/dirvote.c  
24 0 src/or/dirvote.h  
22 0 src/or/nodelist.c  
1 0 src/or/nodelist.h  
21 2 src/or/or.h  
47 7 src/or/routerlist.c  
53 0 src/or/routerparse.c  
201 3 src/test/test_dir.c  

To test in Shadow, compile the source code as usual and enable Waterfilling on directory servers by modifying
their torrrc file (add UseWaterfilling 1 and OptWaterfilling 1).  
Add also UseWaterfilling 1 on clients' torrc.


