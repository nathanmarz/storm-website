---
layout: about
---

Storm was designed from the ground up to be usable with any programming language. At the core of Storm is a [Thrift](http://thrift.apache.org/) [definition](https://github.com/nathanmarz/storm/blob/master/storm-core/src/storm.thrift) for defining and submitting topologies. Since Thrift can be used in any language, topologies can be defined and submitted from any language.

Similarly, spouts and bolts can be defined in any language. Non-JVM spouts and bolts communicate to Storm over a [JSON-based protocol](https://github.com/nathanmarz/storm/wiki/Multilang-protocol) over stdin/stdout. Adapters that implement this protocol exist for [Ruby](https://github.com/nathanmarz/storm/blob/master/storm-core/src/multilang/rb/storm.rb), [Python](https://github.com/nathanmarz/storm/blob/master/storm-core/src/multilang/py/storm.py), [Javascript](https://github.com/Lazyshot/storm-node), [Perl](https://github.com/gphat/io-storm), and [PHP](https://github.com/lazyshot/storm-php).

*storm-starter* has an [example topology](https://github.com/nathanmarz/storm-starter/blob/master/src/jvm/storm/starter/WordCountTopology.java) that implements one of the bolts in Python.