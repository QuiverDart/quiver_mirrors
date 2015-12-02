Quiver Mirrors
==============

Utilities for working with mirrors.

[![Build Status](https://travis-ci.org/QuiverDart/quiver_mirrors.svg?branch=master)](https://travis-ci.org/QuiverDart/quiver_mirrors)
[![Coverage Status](https://img.shields.io/coveralls/QuiverDart/quiver_mirrors.svg)](https://coveralls.io/r/QuiverDart/quiver_mirrors)

## Documentation

[API Docs](http://www.dartdocs.org/documentation/quiver_mirrors/latest)

`getTypeName` returns the name of a Type instance.

`implements` and `classImplements` determine if an instance or ClassMirror,
respectively, implement the interface represented by a Type instance. They
implement the behavior of `is` for mirrors, except for generics.

`getMemberMirror` searches though a ClassMirror and its class hierarchy for
a member. This makes up for the fact that `ClassMirror.members` doesn't
contain members from interfaces or superclasses.

`Method` wraps an InstanceMirror and Symbol to create a callable that invokes
a method on the instance. It in effect closurizes a method reflectively.
