# eQual framework

eQual framework has the following specific features:
### call controllers in a similar way, whatever the context:
* within script 
* from command-line
* through an HTTP request

### use trivial scripts as controllers
```
<?php 
echo 'This is a valid controller';
```
see [this article](http://www.cedricfrancoys.be/dev/articles/trivial-script-as-controller/) for detailed explanations

### encourage self-documenting code
```
<?php
eQual::announce([
    'description'   => 'This script returns some JSON',
    'response'      => [
        'content-type'  => 'application/json',
        'charset'       => 'utf-8'
    ] 
]);
```

### categorize controllers as:
    1. Action handlers (do something)
    2. Data providers (get something)
    3.'App providers (show something)

### explicit data typing 

### HTTP compliant error handling   
see [this article](http://www.cedricfrancoys.be/dev/articles/errors-handling/)

## FAQ
To present it a little further, here is a quick review of Frequently Ask Questions.


### Why the name 'eQual' ?

eQual framework relates with the Babylon mythology and its name originates from the babylonian word '`eqlu`' which, in antique akkadian language, means 'field'.

The underlying idea being that this framework is an environment ready for some "crop" production and also that it puts a strong emphasis on equity and collaboration.

### Which programming language does it use ?

It is written in PHP. However, as described above, its logic is intendend to be language agnostic.

Moreover, while it can be manually extended, most features are available through the use of tools and scripts, and  natively interract with major API query languages (GraphQL, JSON-API, OData).
