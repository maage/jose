jose-alg(1) -- Lists all supported algorithms
=============================================

## SYNOPSIS

`jose alg` [-k KIND]

## OVERVIEW

The `jose alg` command lists the algorithms supported by all `jose` commands.

Since `jose` supports different kinds of algorithms (encryption, signing,
hashing, etc.), you can limit the kinds of algorithms you would like to see
using the `-k` option (which can be specified multiple times). For a list of
the different kinds of algorithms, use the `-k ?` option. If the `-k` option is
not used, all algorithms, regardless of their kind, will be listed.

## OPTIONS

* `-k` _KIND_, `--kind`=_KIND_ :
  Restrict algorithm list to a certain kind

* `-k` ?, `--kind`=? :
  List valid algorithm kinds

## EXAMPLES

List all encryption algorithms:

    $ jose alg -k encr
    A128CBC-HS256
    A128GCM
    A192CBC-HS384
    A192GCM
    A256CBC-HS512
    A256GCM

## AUTHOR

Nathaniel McCallum &lt;npmccallum@redhat.com&gt;
