**FLIMSY**
==========

**What is flimsy?**
-------------------

Flimsy is a small shell script which can install and run different versions of the [Clojure](http://clojure.org/) programming language.
It was inspired from the [RVM](https://rvm.io/) tool for Ruby.

Note that it is not supposed to replace [Leiningen](http://leiningen.org/)
but rather to make it more easy to run simple scripts with more than one Clojure version. It also makes it easy to install Clojure on some
broken systems (like Ubuntu 12.04)

**Dependencies**
----------------

Flimsy requires POSIX like envirnonment and wget. For Clojure itself you need to install Java as well and make sure that it can be found in PATH.

**Installing flimsy**
---------------------

To install flimsy you just need to download the flimsy script and put it in some place accessable through PATH.

**Getting started with Clojure**
--------------------------------

- To install and run a selected version of Clojure (like 1.5.1) you can use the following set of commands:

    flimsy install 1.5.1  
    flimsy use 1.5.1  

- You can also install more versions of Clojure and switch between them with the **use** command:

    flimsy install 1.4.0  
    flimsy install 1.3.0  
    flimsy use 1.4.0  

- You can start Clojure REPL or run a clojure script like this:

    flimsy repl  
    flimsy run sample_test.clj  
    flimsy run command_test.clj arg1 "arg 2"  

- You can list installed clojure versions or check the current version like this:

    flimsy list  
    flimsy ver  

