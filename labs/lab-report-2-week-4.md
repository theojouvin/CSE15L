## Lab Report 2
### Bugs, Symptoms, and Failure Inducing Inputs
---

Below, three code changes that occured during Lab 3 can be found.
The following are included with every code change to further understand their purpose:
- A screenshot of the code change differences from GitHub.
- A link to the test file containing a failure inducing input that prompted the code change.
- A screenshot of the symptom caused by the failure inducing input.
- A short description of the relationship between the bug, the symptom, and the failure-inducing input.

Screenshots will be included in spoilers as to not take up uncessary space. 

<details>
  <summary> » This is a spoiler, Click Me!</summary>
  This is the inside of a spoiler where images will be located!
  </details>

---

## 1. Infinite Loop

  [Test File](lab2files/test-file-inf-loop.md)

  When running a test file with an extra line at the bottom, or a file that does not contain an open or close bracket, the MarkdownParse program will loop infinitely. In this case, the failure inducing input is that of a lack of opening or closing brackets at all, or after a previously found close bracket if the file contains more text. The symptom is clear, the pogram will loop infinitely, causing Java to run out of memory. This occurs because MarkdownParse continues to loop for the next set of brackets and does nothing except for try again if nothing is found. The fix adds a case to MarkdownParse telling the program to break out of the loop if a new set of brackets are not found.
  
<details>
  <summary> » Code Change Difference</summary>
  <img src="lab2images/infloopccd.png" alt="Infinite Loop Code Change Difference">
  </details>

<details>
  <summary> » Symptom of Failure Inducing Input</summary>
  <img src="lab2images/infloopsymptom.png" alt="Infinite Loop Symptom">
  </details>


## 2. Any Parentheses

  [Test File](lab2files/test-file-any-parentheses.md)

  When running a test file with an extra line at the bottom, or a file that does not contain an open or close bracket, the MarkdownParse program will loop infinitely. In this case, the failure inducing input is that of a lack of opening or closing brackets at all, or after a previously found close bracket if the file contains more text. The symptom is clear, the pogram will loop infinitely, causing Java to run out of memory. This occurs because MarkdownParse continues to loop for the next set of brackets and does nothing except for try again if nothing is found. The fix adds a case to MarkdownParse telling the program to break out of the loop if a new set of brackets are not found.
  
<details>
  <summary> » Code Change Difference</summary>
  <img src="lab2images/anyparenthesesccd.png" alt="Any Parentheses Code Change Difference">
  </details>

<details>
  <summary> » Symptom of Failure Inducing Input</summary>
  <img src="lab2images/anyparenthesessymptom.png" alt="Any Parentheses Symptom">
  </details>
  
  
## 3. Any Text

  [Test File](lab2files/test-file-any-text.md)

  When running a test file with an extra line at the bottom, or a file that does not contain an open or close bracket, the MarkdownParse program will loop infinitely. In this case, the failure inducing input is that of a lack of opening or closing brackets at all, or after a previously found close bracket if the file contains more text. The symptom is clear, the pogram will loop infinitely, causing Java to run out of memory. This occurs because MarkdownParse continues to loop for the next set of brackets and does nothing except for try again if nothing is found. The fix adds a case to MarkdownParse telling the program to break out of the loop if a new set of brackets are not found.
  
<details>
  <summary> » Code Change Difference</summary>
  <img src="lab2images/anytextccd.png" alt="Any Text Code Change Difference">
  </details>

<details>
  <summary> » Symptom of Failure Inducing Input</summary>
  <img src="lab2images/anytextsymptom.png" alt="Any Text Symptom">
  </details>
