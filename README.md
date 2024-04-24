[![Latest Stable Version](http://poser.pugx.org/opctim/php-nilsimsa/v)](https://packagist.org/packages/opctim/php-nilsimsa) [![Total Downloads](http://poser.pugx.org/opctim/php-nilsimsa/downloads)](https://packagist.org/packages/opctim/php-nilsimsa) [![Latest Unstable Version](http://poser.pugx.org/opctim/php-nilsimsa/v/unstable)](https://packagist.org/packages/opctim/php-nilsimsa) [![License](http://poser.pugx.org/opctim/php-nilsimsa/license)](https://packagist.org/packages/opctim/php-nilsimsa) [![PHP Version Require](http://poser.pugx.org/opctim/php-nilsimsa/require/php)](https://packagist.org/packages/opctim/php-nilsimsa)

# php-nilsimsa


### PHP library to calculate and compare Nilsimsa digests.

The Nilsimsa hash is a locality senstive hash function. Generally similar documents will have
similar Nilsimsa digests. The Hamming distance between the digests can be used to approximate
the similarity between documents. For further information consult
http://en.wikipedia.org/wiki/Nilsimsa_Hash and the references (particularly Damiani et al.)

----------------

**Implementation details:**

The Nilsimsa class takes in a data parameter which is the string of the document to digest
Calling the methods hexdigest() and digest() give the nilsimsa digests in hex or array format.
The helper function compare_digests takes in two digests and computes the Nilsimsa score.
You can also use compare_files() and compare_strings() to compare files and strings directly.

This code is a port of py-nilsimsa located at https://code.google.com/p/py-nilsimsa

**This repository has been forked from _beager/php-nilsimsa_. It has been cleaned up and 
restructured so it can be used as a composer package.**

@beager released this under the MIT license, (c) 2015 Bill Eager
