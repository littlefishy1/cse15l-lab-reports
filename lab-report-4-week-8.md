# **Lab Report 4**
February 24, 2022
<br/><br/>
<br/><br/>
# Test code
<br/><br/>
The result for the first snippet should be [`google.com, google.com, ucsd.edu]. The result for the second snippet should be [a.com, a.com(()), example.com]. The result for the third snippet should be [https://ucsd-cse15l-w22.github.io/']. 
![image](6ebac096ed4ce4f30e561a71a9414df8.png)
# Own implementation 
[Repository](https://github.com/littlefishy1/markdown-parse)
<br/><br/>
![image](eaf690a5862db538c9b108f5942494b0.png)
For snippet 1, there could be code checking if there is one ` infront of the first bracket. If yes then then the first bracket should not be accounted for. If there are even number of ' then it would be ignored. for snippet 2, it would be a chFor snippet 3, there could be a change where the programs to remove the spaces. However, it would be a challenge to detect new lines in brackets and parenthesis because it would be hard to tell if the link includes brackets or it is the start of another link.