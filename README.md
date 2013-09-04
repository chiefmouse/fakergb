# FakerUK

FakerUK is a fork of Faker, itself a port of [Ruby Faker library](http://faker.rubyforge.org/) to the
clojure programming language.

It is useful when you want to generate fake but good-looking data, such as in
test scenarios or staging servers.

FakerUK has data (specifically first and last person names, and person name suffixes, more authentically British English.

This library will be - but is not yet - available via Clojars (and hence e.g. Leiningen) asap.

## Installation

The easiest way is to use Leiningen. Add the following dependency to your
project.clj file:

    [fakerUK "0.2.3"]


## Usage

    (ns test
      (:use fakerUK.name fakerUK.lorem))

    (def n (take 10 (names)))
    (def p (take 10 (paragraphs)))

There are several more namespaces for generating:

* Person names
* Company names
* Addresses
* Domains and emails
* Telephone numbers
* Text


