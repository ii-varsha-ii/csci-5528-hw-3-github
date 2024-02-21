CSCI 5828 - Spring 2024
Homework 3
Teammates: Adarsh Srinivasan, Varsha Natarajan
Due: 02/20/2024
   
3: bug_fix: commit 3:     
git checkout <commit 0 ref>     
git switch -c bug-fix      

4: bug_fix: commit 4:       
[ Edit README.md ]   

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
