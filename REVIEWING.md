## Guideline for reviewing a pull request (PR)

1. Go the PR page.
2. Click "Files changed".
3. Check if the PR has changed/added any files that should not have been 
   changed/added. If it does, request to have that corrected. There can be 
   multiple ways within the PR page to request changes, for example, on the 
   main thread on the PR's page, by clicking the text bubble button (**under** 
   the green "Review changes" button), or if it's a .py file, you 
   can click on the "+" symbol at the beginning of a specific line to insert a 
   comment specific to that line.
4. Check if the newly added codes follow good coding practice, for example, 
   avoiding redundancies. If not, point those out to be fixed.
5. If you notice some code that can be rewritten to improve efficiency by a 
   significant amount, request to make that improvement.
6. Once you are done viewing a file, click "Viewed" for that file. 
7. Once you are done viewing all the files, click "Review changes", choose 
   between the three options: "Comment", "Approve", or  "Request changes" as 
   appropriate.
   - **If you choose "Request changes", then
   this PR cannot be merged until the requested changes have been made, and you
   will have to provide approval after the requested changes have been made
   (please be timely to provide your approval once that is done
   so that the PR can be merged in a timely manner).**
   - **If you choose "Comment", then the PR will not wait for your approval if there
   is at least one approval from any other reviewer. However, you can still provide approval
   if you would like to after your comments have been incorporated.**
9. You are only checking the correctness and appropriateness of the code. 
   You do not need to check goodness of model fit, stylistic elements in 
   the plots, etc.
10. **Please don't merge yourself and leave that task to @ajshajib.**
