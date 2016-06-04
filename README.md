#Symbolic Link vs. Hard Link

---


HARD LINK
---

A hard link that will point to the underlying inode of the source
file. This is not a pointer to a file but an actually directory entry
(a file) pointing the same inode.

<p style="background-color: #00ff00;">
Note: If you delete the source file the hard link still points to the
       inode and the inode is not removed</p>

	ln /path/to/source/file /path/to/linked/file



------------------------------------------------------------------------
SYMBOLIC LINK
------------------------------------------------------------------------

ln -s /path/to/source/file /path/to/linked/file

Creates a symbolic link that will point to the path of the source file. (Think window's shortcuts {needs citation}).

	-If you delete the source file the symlink points to a
         non-existing file and is broken



	
