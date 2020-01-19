node
{
 stage "1. Create a build output"
 sh "mkdir -p output"
 sh "mkdir -p input"
 writeFile file:"output/usefulfile.txt",text:"This is a useful file."
 writeFile file:"output/usefulfile.md",text:"This is a c."
 writeFile file:"output/git.html",text:"Thsi is a useless file from git repository."
 stage "2. Archive Build Output"
 writeFile file:"input/usefulfile.txt",text:"This is a useful file from SCM."
 writeFile file:"input/uselessfile.md",text:"This is a useless file from SCM."
 stage "3. Build the code"
 echo "Building the code from SCM"
 stage "4. Another step"
 sh "touch another.html"
 stage "5. Git step"
 sh "touch another_git_repo.html"
 }
 
