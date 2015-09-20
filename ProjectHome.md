### Overview ###

Every so often, projects need to directly embed Linux system calls instead of calling the implementations in the system runtime library.

This project provides a header file that can be included into your application whenever you need to make direct system calls.

### How to include linux\_syscall\_support.h in your project ###

You can either copy the file into your project, or preferably, you can set up SVN to automatically pull from our source repository.

To do so, you will need to run
```
$ svn propset svn:externals 'lss http://linux-syscall-support.googlecode.com/svn/trunk/lss' include
```

This assumes that you have an _include_ directory where all your include files are located. Adjust the path as needed.

If you don't want to automatically track the development versions of **lss/linux\_syscall\_support.h**, feel free to at a "**-r**_NUM_" option before the URL.