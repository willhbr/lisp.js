# Lisp.js

Install for CLI:

    npm install @javanut13/lisp.js

Run it from the command line:

    lispjs -x my_lisp_file # execute the file
    lispjs -c my_lisp_file # print the JS version of the file
    lispjs -c my_lisp_file -o transpiled.js # Write the transpiled file

Include it in a webpage:

    <script src="lisp-web.min.js"></script>
    ...
    '(console.log "Hello world")'.evalLisp();
    '(console.log "Hello world")'.toJS();

### Syntax

    (:length my_array) ; get the length (or another property) from an object
    (.substring "Foobar" 3) ; call a method on an object
    (defn func [a b] (console.log (+ a b))) ; create a function

The syntax is mostly Clojure-esque.