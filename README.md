# My reading goals
Books I'm reading, want to read or have read.

Books I am reading or want to read [are open issues](https://github.com/imjacobclark/reading-list/issues).

Books I have completed [are closed issues](https://github.com/imjacobclark/reading-list/issues?q=is%3Aissue+is%3Aclosed).

My yearly book goals are milestones - [here are 2019's](https://github.com/imjacobclark/reading-list/milestone/1) goals.

Each book is labeled with its primary subject area (chosen by me) - [here are the books I want to read or ones I'm currently reading on `compilers`](https://github.com/imjacobclark/reading-list/issues?q=is%3Aopen+is%3Aissue+label%3Acompilers).

I will limit my reading to 3 books at a time. The label [in progress](https://github.com/imjacobclark/reading-list/issues?q=is%3Aopen+is%3Aissue+label%3Ain-progress) can be used to see what I'm activley reading.

# Running the program

## Install SBCL and quicklisp

```shell
$ brew install sbcl
$ curl -o /tmp/ql.lisp http://beta.quicklisp.org/quicklisp.lisp
$ sbcl --no-sysinit --no-userinit --load /tmp/ql.lisp \
       --eval '(quicklisp-quickstart:install :path ".quicklisp")' \
       --quit
$ sbcl --eval '(ql:add-to-init-file)' --quit
```
