# Paths

### You should already know about
* [Trees](../trees/README.md)

As we learned when we were talking about trees, paths are a sequence of nodes and edges connecting a node with a descendant. Usually when we talk about paths we are talking about files or resources on our computer, or on a server. If you think about it, the file system on your computer can be represented as a tree data structure. For example, on my computer I have a root folder that contains a Users folder. The Users folder contains an alarner folder and the alarner folder contains a bunch of other folders.

![Folder Tree](folder-tree.png)

If we were to visualize these folders (also sometimes called directories) as a tree, it might look something like this...

![Directory Tree](directory-tree.png)

The **path** to the alarner directory would look like this...

![Directory Tree Path](directory-tree-path.png)

When we describe paths in web development we commonly write them like `/Users/alarner`. Notice that as we traverse the path from top to bottom, each time we encounter a node we write the name of the node (the directory name) and each time we encounter an edge we write a `/`. The root node is special because of the way that your Mac names it. If you look at it in the Finder you will see that it's called Macintosh HD, but that's just a nick name. Its real name is `/`. That means if our path starts with a `/` then we are telling the computer to begin in the root directory. Paths that begin with a `/` are called **root relative** paths because they are relative to the root node of the directory tree.