CSCI 5828 - Spring 2024
Homework 3
Teammates: Adarsh Srinivasan, Varsha Natarajan
Due: 02/20/2024
   
List of commands:   
git init   
vi README.md   
   
0: master: commit 0: Edit README.md  
git add .
git commit -m "commit 0: Add README.md"      
git push

1: master: commit 1: ref commit 0    
[ Add `<br>` in README.md ]         
git add .    
git commit -m "commit 1: ref commit 0"      
git push

2: master: commit 2: ref commit 1
[ Editting README.md to make commit 2 ]   
git add .    
git commit -m "commit 2: ref commit 1"    
git push

3: bug_fix: commit 3:
git checkout <commit 0 ref>
git switch -c bug-fix

4: bug_fix: commit 4:   
[ Edit README.md ]   
git add .    
git commit -m "commit 4: ref commit 3"
git push   

5: bug_fix: commit 5:   
git merge main   
[Resolve merge conflicts]
git add .
git commit -m "commit 5: ref cmmit 2: Merge conflict"

6: bug_fix: commit 6: ref commit 5: 
[ Edit README.md ]
git add .
git commit -m "commit 6: ref commit 5"

7: bug_fix_experimental: commit 7    
git checkout bug-fix  
git checkout <commit 4 ref>   
git switch -c bug-fix-experimental   
[ Edit README.md ]   
git add .   
git commit -m "commit 7: ref commit 4"   
git push   

8: bug-fix-experimental: commit 8    
[ Edit README.md ]    
git add .   
git commit -m "commit 8: ref commit 7"   
git push

9: bug-fix-experimental: commit 9   
[ Edit README.md ]    
git add .   
git commit -m "commit 9: ref commit 8"    
git push   

10: master: commit 10:
[ Edit README.md ]
git add .
git commit -m "commit 10: ref commit 2"

11: bug-fix: commit 11: ref commit 9    
git merge bug-fix-experimental    
[ Resolve conflicts ]    
git add .    
git commit -m "commit 11: ref commit 9"    
git push    

12: bug-fix: commit 12: ref commit 11
[ Edit README.md ]    
git add .   
git commit -m "commit 12: ref commit 11"   
git push         

13: master: commit 13:    
git merge bug-fix    
[ Resolve conflicts ]   
git add .   
git commit -m "commit 13: ref commit 10 Merge conflict"    

14: master: commit 14: 
[ Edit README.md and attach the file ]
git add image README.md
git commit -m "commit 14: ref commit 13: final commit" 
git push

