## Lab Report 4
### Testing the Implementation of Two Versions of MarkdownParse
---

This lab report contains the following:
- A link to my lab group's Markdown Parser repository.
- A link to another lab group's Markdown Parser repository that my group reviewed.
- For three Markdown code snippets:
  - Expected Output
  - MarkdownParseTest Code
  - Actual outputs for both implementations of MarkdownParse.
  - Test results for both implementations of MarkdownParse.
  - Potential code fixes to achieve expected output, if necessary.

Screenshots will be included in spoilers as to not take up uncessary space. 

<details>
  <summary> » This is a spoiler, Click Me!</summary>
  This is the inside of a spoiler where images will be located!
  </details>

---

- My lab group's Markdown Parser repository: <a href="https://github.com/Mashyuf/markdown-parser" target="_blank">Mashyuf/markdown-parser</a>
- The reviewed Markdown Parser repository: <a href="https://github.com/cmy0357/markdown-parser" target="_blank">cmy0357/markdown-parser</a>

---

## Snippet 1

[Markdown Snippet](lab4resources/files/snippet1)

  For this snippet, both MarkdownParse implementations failed their tests. Both implementations included ```url.com``` when they should not have. I feel like this code change would be pretty small, less than 10 lines. The link should not have been included because since the backtick came first, it should parse as a code block. Of course, both implementations of MarkdownParse did not know this. The fix could be to check for a pair of backticks, with the first backtick occuring before the start of the URL syntax (before the opening bracket). My group's implementation of MarkdownParse also did not output ```ucsd.edu```, probably because of the closing bracket in the link title portion of the URL syntax. A fix for this could include skipping over brackets in the title portion if they do not complete a valid URL.
  
<details>
  <summary> » Expected Output</summary>
  [`google.com, google.com, ucsd.edu]
  <br /><img src="lab4resources/images/snippet1expected.png" alt="Snippet 1 Expected Output">
  </details>

<details>
  <summary> » Test Code</summary>
  <img src="lab4resources/images/snippet1testcode.png" alt="Snippet 1 Test Code">
  </details>

<details>
  <summary> » Our Actual Output</summary>
  <img src="lab4resources/images/oursnippet1actual.png" alt="Our Actual Output from Snippet 1">
  </details>
  
<details>
  <summary> » Our Failed Test</summary>
  <img src="lab4resources/images/ourtest1fail.png" alt="Our Failed Test 1">
  </details>
  
<details>
  <summary> » Their Actual Output</summary>
  <img src="lab4resources/images/theirsnippet1actual.png" alt="Their Actual Output from Snippet 1">
  </details>
  
<details>
  <summary> » Their Failed Test</summary>
  <img src="lab4resources/images/theirtest1fail.png" alt="Their Failed Test 1">
  </details>


## Snippet 2

[Markdown Snippet](lab4resources/files/snippet2)

  For this snippet, both MarkdownParse implementations failed their tests. Both implementations outputted ```a.com((``` instead of ```a.com(())```. I feel like this code change may be longer than 10 lines. It looks like both implementations completed the URL early, because of the extra parentheses. A potential fix for this could be to have MarkdownParse count its current position in the parentheses to ensure that it returns the link once the syntax has actually completed. My group's implementation of MarkdownParse also did not output ```example.com```, probably because of the extra brackets. The fix for this could be similar to that of the previous failure's solution; having the program count its current position in the brackets to ensure that it actually returns a link when one is present.
  
<details>
  <summary> » Expected Output</summary>
  [a.com, a.com(()), example.com]
  <br /><img src="lab4resources/images/snippet2expected.png" alt="Snippet 2 Expected Output">
  </details>

<details>
  <summary> » Test Code</summary>
  <img src="lab4resources/images/snippet2testcode.png" alt="Snippet 2 Test Code">
  </details>
  
<details>
  <summary> » Our Actual Output</summary>
  <img src="lab4resources/images/oursnippet2actual.png" alt="Our Actual Output from Snippet 2">
  </details>
  
<details>
  <summary> » Our Failed Test</summary>
  <img src="lab4resources/images/ourtest2fail.png" alt="Our Failed Test 2">
  </details>
  
<details>
  <summary> » Their Actual Output</summary>
  <img src="lab4resources/images/theirsnippet2actual.png" alt="Their Actual Output from Snippet 2">
  </details>
  
<details>
  <summary> » Their Failed Test</summary>
  <img src="lab4resources/images/theirtest2fail.png" alt="Their Failed Test 2">
  </details>
  
  
## Snippet 3

[Markdown Snippet](lab4resources/files/snippet3)

  For this snippet, both MarkdownParse implementations failed their tests. The second URL is the only one that should have been outputted. The first and last contain line breaks in their syntax, and the second to last's format is clearly incorrect. Unfortunately, my group's implementation returned no links, and the other group's returned three, with one combining another. Again, I feel like this code change may be longer than 10 lines. Like with the previous snippet, there could be a counter for the parentheses to ensure that only URLS with complete syntaxes are being returned (my group). This may be a smaller code change, but there could also be a check for line breaks in the link syntax to ensure that links with line breaks are not returned (other group).
  
<details>
  <summary> » Expected Output</summary>
  [https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule]
  <br /><img src="lab4resources/images/snippet3expected.png" alt="Snippet 3 Expected Output">
  </details>

<details>
  <summary> » Test Code</summary>
  <img src="lab4resources/images/snippet3testcode.png" alt="Snippet 3 Test Code">
  </details>

<details>
  <summary> » Our Actual Output</summary>
  <img src="lab4resources/images/oursnippet3actual.png" alt="Our Actual Output from Snippet 3">
  </details>
  
<details>
  <summary> » Our Failed Test</summary>
  <img src="lab4resources/images/ourtest3fail.png" alt="Our Failed Test 3">
  </details>
  
<details>
  <summary> » Their Actual Output</summary>
  <img src="lab4resources/images/theirsnippet3actual.png" alt="Their Actual Output from Snippet 3">
  </details>
  
<details>
  <summary> » Their Failed Test</summary>
  <img src="lab4resources/images/theirtest3fail.png" alt="Their Failed Test 3">
  </details>
