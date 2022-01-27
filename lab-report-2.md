# **Lab Report 2**
January 27, 2022
<br/><br/>
<br/><br/>
# Code Change 1
<br/><br/>
Code change diff:

![Image](2676711cfc672d09a3951ab99198a5c1.png)

[link to the file that caused the error](https://github.com/littlefishy1/markdown-parse/commit/0290a53148a94a4d8c0c6c63eff48edfce44e838)

Symptoms:

![Image](eb253b0610e392dd846e4b7de4610ee8.png)

The bug is that the loop only stops when the file does not end with ")" such that currentIndex is no longer smaller tham the length of the file. The symptom caused by it is that if the file does not end with ")" then the loop is going to be infinite and will never break. New.md is an example of such files which caused the symptoms.

<br/><br/>
# Code Change 2
<br/><br/>
Code change diff:

![Image](28d24a9265304f37365f8cfeefac3e16.png)

[link to the file that caused the error](https://github.com/littlefishy1/markdown-parse/blob/main/new3.md)

Symptoms: ![Image](28ff30074a359255287710a603fea240.png)

The bug is that the code accounts for brackets and parentheses for links. The symptom caused by it is that an image would be printed as a link when it is not supposed to be printed. New3.md is an example of image which would be printed as a link due to the bug.

<br/><br/>
# Code Change 3
<br/><br/>
Code change diff: 
![Image](96c0ae076cc8716a6213e4014989e5d8.png)

[link to the file that caused the error](https://github.com/littlefishy1/markdown-parse/blob/main/test-file8.md)


Symptoms: 

![Image](3aea010336a7ae43ec1e22b82c6c0324.png)

The bug is that the code did not account for the cases where the file start with "[". The symptom caused by it is that exception would be called when the nextOpenBracket-1 = -1 which would lead to an index of -1. test-file8.md is an example of such cases where the file starts with "[".