# directorytree
Implement fake directory tree of system
- First of all, we need to create a Tree data structure. It cannot be binaryTree, as the file system could contain several childNodes (sub-folders) under a parentNode
- Once the Tree data structure is created, we could start creating functions like "Create", "List", "Move" and "Delete"
  -Create will scan the input string from the command line after the "CREATE" keyword, if it contains '/', then split the string by '/', and try to find the first string from the splited array in the existing tree. If could not find that string, create the node under the "ROOT". If it finds that string, try to do the same thing recursively
  -List will print out the whole tree structure
  -Move will first validate the target path and destination path do exist in the current tree. If they both exist, it will move the target path under the detination node as childNodes
  -Delete will first validate the target path does exist in the current tree. If it exists, it will remove the whole childNodes from the parentNodes using the given path
- Create the main() function to read command line as user input
