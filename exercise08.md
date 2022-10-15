# Exercise 8 - Viewing changes before committing

1. Ensure your working directory is clean

2. Add text to any one of your files

3. Delete different text from another of your files

4. Look at `git status`

5. View all the changes you've made

        git diff

6. Does the following command return anything? No

        git diff --staged

7. Add one of your changed files to the index

        git commit add <changed file>

8. What do these commands show?

        git diff
        this one shows the changes to the file that hasn't been added to the index
        diff --git a/fruits.txt b/fruits.txt
index 83dc3b9..c7c0089 100644
--- a/fruits.txt
+++ b/fruits.txt
@@ -1,5 +1,3 @@
  blueberry
  strawberry
- apple
  banana
- tomato
\ No newline at end of file
        
        git diff --staged
        
        this one shows the file, and its changes, that was added to the index
        
        git diff --staged
diff --git a/vegetables.txt b/vegetables.txt
index 832e7e1..fd19506 100644
--- a/vegetables.txt
+++ b/vegetables.txt
@@ -3,4 +3,6 @@ cucumber
 onion
 avocado
 lemon
-garlic
\ No newline at end of file
+garlic
+potato
+squash
\ No newline at end of file


9. Add the other changed file to the index

        git commit add <other changed file>

10. What do these commands show?

        git diff
        It shows nothing
        
        
        git diff --staged
        This one shows both files (and their changes).
        diff --git a/fruits.txt b/fruits.txt
index 83dc3b9..c7c0089 100644
--- a/fruits.txt
+++ b/fruits.txt
@@ -1,5 +1,3 @@
  blueberry
  strawberry
- apple
  banana
- tomato
\ No newline at end of file
diff --git a/vegetables.txt b/vegetables.txt
index 832e7e1..fd19506 100644
--- a/vegetables.txt
+++ b/vegetables.txt
@@ -3,4 +3,6 @@ cucumber
 onion
 avocado
 lemon
-garlic
\ No newline at end of file
+garlic
+potato
+squash
\ No newline at end of file

11. Commit the changes

12. Check that your working directory is clean

13. Create a new file named `clothing.txt`

14. Does the new untracked file show up in git diff? It does not

        git diff

15. Add and commit the new file
