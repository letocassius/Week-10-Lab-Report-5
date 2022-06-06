# Lab Repo

## How I found the tests with different results:
I used `vimdiff` to find the differences between the file's results. 

## Provide a link to the test-file with different-results
* [Test File 194](https://github.com/nidhidhamnani/markdown-parser/edit/main/test-files/194.md)
* [Test File 497](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/497.md))

## For test-file 194
* Neither implementations are correct.
* Expected output should be: `[my_(url)]`

<img width="1167" alt="image" src="https://user-images.githubusercontent.com/64039891/172086149-49df6409-aa0f-4884-a1ab-52cc57427236.png">
My implementation and the other implementation only recognizes. They only account for the `[]()` style. So hence,the `[]` and `[url]` outcomes are not being printed out. 


## For test-file 497
There s a different in the output of line 886 from my results comparing to 884 line in my partner's file. 
<img width="356" alt="image" src="https://user-images.githubusercontent.com/64039891/172077636-4b5b2b73-f9ca-44ad-8744-335852a2fbcc.png">

File content:
<img width="710" alt="image" src="https://user-images.githubusercontent.com/64039891/172077651-2b890d76-11cd-4f58-9dd2-97cffbece9c8.png">

## Bug
the correct output should be 'foo(and(bar)' neither are correct. My implementaton print out something, but the contentis is somthing that is not a link and it should not be printed out. The bug is caused since both implementations fail to recognized what the slash which is suppose to be a escape simble.
