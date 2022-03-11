# **Lab Report 5**
March 9, 2022
<br/><br/>
<br/><br/>
# Methods to find differences
<br/><br/>
I found the differences between the results by storing the results of bash scripts into two different text files and run ```diff -y``` between the two files. This command compares the results side by side and shows the differences
<br/><br/>
# Difference 1 (test-files/41.md)
<br/><br/>
Test file:

![image](5a9701bd2f8d72808e25b019669831ce.png)

Lab 9 implementation result:

![image](fe7f4e0fc665b088e7102c753732181d.png)

Own implementation result:

![image](144c7767e6866bade14d0331660af946.png)

Code need to be fixed:

![image](5a3967dab22c38942c226f1ed516fee6.png)

The Lab 9 implementation is correct. The bug in the code is that it does not check if there are spaces between the brackets. It straight adds the everything between the brackets. A fix to it is to just check if there are spaces between the brackets. If so, then do not add to toReturn.
<br/><br/>
# Difference 2 (test-files/41.md)
<br/><br/>

Test file:

![image](dcb050d68e8de61034e3e90df3e246e9.png)

Lab 9 implementation result:

![image](fe7f4e0fc665b088e7102c753732181d.png)

Own implementation result:

![image](310ba088157ba8063e5f731e5f1364fd.png)

Code need to be fixed:

![image](5a3967dab22c38942c226f1ed516fee6.png)

The Lab 9 implementation is correct. The bug in the code is that it does not check if there is a new line between the brackets. It straight adds the everything between the brackets. A fix to it is to just check if there are line changes between the brackets. If so, then do not add to toReturn.
