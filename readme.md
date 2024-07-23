```
-----------------------------------------
-- 0
-----------------------------------------
➜  2024_07_git_properties_issue git:(main) ✗ ls my-module/build/resources/main/git.properties
ls: my-module/build/resources/main/git.properties: No such file or directory

-----------------------------------------
-- 1 => OK
-----------------------------------------
➜  2024_07_git_properties_issue git:(main) ✗ g clean assemble --console=plain
`
> Task :my-module:clean UP-TO-DATE
> Task :my-module:compileJava NO-SOURCE
> Task :my-module:generateGitProperties
> Task :my-module:processResources
> Task :my-module:classes
> Task :my-module:jar
> Task :my-module:assemble

BUILD SUCCESSFUL in 628ms
4 actionable tasks: 3 executed, 1 up-to-date


➜  2024_07_git_properties_issue git:(main) ✗ ls my-module/build/resources/main/git.properties
my-module/build/resources/main/git.properties

-----------------------------------------
-- 2 => OK
-----------------------------------------
➜  2024_07_git_properties_issue git:(main) ✗ g clean assemble --console=plain
> Task :my-module:clean
> Task :my-module:compileJava NO-SOURCE
> Task :my-module:generateGitProperties FROM-CACHE
> Task :my-module:processResources
> Task :my-module:classes
> Task :my-module:jar
> Task :my-module:assemble

BUILD SUCCESSFUL in 407ms
4 actionable tasks: 3 executed, 1 from cache


➜  2024_07_git_properties_issue git:(main) ✗ ls my-module/build/resources/main/git.properties
my-module/build/resources/main/git.properties

-----------------------------------------
-- 3 => NOK
-----------------------------------------
➜  2024_07_git_properties_issue git:(main) ✗ g clean assemble --console=plain
> Task :my-module:clean
> Task :my-module:compileJava NO-SOURCE
> Task :my-module:generateGitProperties FROM-CACHE
> Task :my-module:processResources
> Task :my-module:classes
> Task :my-module:jar
> Task :my-module:assemble

BUILD SUCCESSFUL in 387ms
4 actionable tasks: 3 executed, 1 from cache


➜  2024_07_git_properties_issue git:(main) ✗ ls my-module/build/resources/main/git.properties
ls: my-module/build/resources/main/git.properties: No such file or directory

-----------------------------------------
-- 4 => OK
-----------------------------------------
➜  2024_07_git_properties_issue git:(main) ✗ g clean assemble --console=plain
> Task :my-module:clean
> Task :my-module:compileJava NO-SOURCE
> Task :my-module:generateGitProperties FROM-CACHE
> Task :my-module:processResources
> Task :my-module:classes
> Task :my-module:jar
> Task :my-module:assemble

BUILD SUCCESSFUL in 373ms
4 actionable tasks: 3 executed, 1 from cache
➜  2024_07_git_properties_issue git:(main) ✗ ls my-module/build/resources/main/git.properties

-----------------------------------------
-- 5 => NOK
-----------------------------------------
my-module/build/resources/main/git.properties
➜  2024_07_git_properties_issue git:(main) ✗ g clean assemble --console=plain
> Task :my-module:clean
> Task :my-module:compileJava NO-SOURCE
> Task :my-module:generateGitProperties FROM-CACHE
> Task :my-module:processResources
> Task :my-module:classes
> Task :my-module:jar
> Task :my-module:assemble

BUILD SUCCESSFUL in 381ms
4 actionable tasks: 3 executed, 1 from cache

➜  2024_07_git_properties_issue git:(main) ✗ ls my-module/build/resources/main/git.properties
ls: my-module/build/resources/main/git.properties: No such file or directory

-----------------------------------------
-- 6 => OK
-----------------------------------------
➜  2024_07_git_properties_issue git:(main) ✗ g clean assemble --console=plain
> Task :my-module:clean
> Task :my-module:compileJava NO-SOURCE
> Task :my-module:generateGitProperties FROM-CACHE
> Task :my-module:processResources
> Task :my-module:classes
> Task :my-module:jar
> Task :my-module:assemble

BUILD SUCCESSFUL in 373ms
4 actionable tasks: 3 executed, 1 from cache
➜  2024_07_git_properties_issue git:(main) ✗ ls my-module/build/resources/main/git.properties

-----------------------------------------
-- 7 => NOK
-----------------------------------------
my-module/build/resources/main/git.properties
➜  2024_07_git_properties_issue git:(main) ✗ g clean assemble --console=plain
> Task :my-module:clean
> Task :my-module:compileJava NO-SOURCE
> Task :my-module:generateGitProperties FROM-CACHE
> Task :my-module:processResources
> Task :my-module:classes
> Task :my-module:jar
> Task :my-module:assemble

BUILD SUCCESSFUL in 381ms
4 actionable tasks: 3 executed, 1 from cache

➜  2024_07_git_properties_issue git:(main) ✗ ls my-module/build/resources/main/git.properties
ls: my-module/build/resources/main/git.properties: No such file or directory
```