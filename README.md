#YAP raptor Interface

This provides YAP a rdf reader using [raptor](http://librdf.org/raptor/)

###Compile

```shell
    $ cmake
    $ make
```

###Install

```shell
    $ make install 
```

Might require sudo

###Example Usage

```prolog
?- use_module(rdf).
?- rdf_load('example.rdf',user,example).
../example.rdf : 3 triples
?- example(Subject,Predicate,Object).
Object = 'http://www.example.org/tv_show',
Predicate = 'http://www.w3.org/1999/02/22-rdf-syntax-ns#type',
Subject = 'http://www.example.org/law_and_order_ci' ?
```