# core.async

A Clojure library designed to provide facilities for async programming and communication.


## Releases and Dependency Information

Latest release: 0.2.382

* [All Released Versions](http://search.maven.org/#search%7Cgav%7C1%7Cg%3A%22org.clojure%22%20AND%20a%3A%22core.async%22)

[Leiningen](https://github.com/technomancy/leiningen) dependency information:

```clj
 [org.clojure/clojure "1.6.0"]
 [org.clojure/core.async "0.2.382"]
```

[Maven](http://maven.apache.org/) dependency information:

```xml
<dependency>
  <groupId>org.clojure</groupId>
  <artifactId>core.async</artifactId>
  <version>0.2.382</version>
</dependency>
```

## Documentation

* [Rationale](http://clojure.com/blog/2013/06/28/clojure-core-async-channels.html)
* [API docs](http://clojure.github.io/core.async/)
* [Code walkthrough](https://github.com/clojure/core.async/blob/master/examples/walkthrough.clj)

## Presentations

* [Rich Hickey on core.async](http://www.infoq.com/presentations/clojure-core-async)
* [Tim Baldridge on core.async](http://www.youtube.com/watch?v=enwIIGzhahw) from Clojure/conj 2013 ([code](https://github.com/halgari/clojure-conj-2013-core.async-examples)).
* Tim Baldridge on go macro internals - [part 1](https://www.youtube.com/watch?v=R3PZMIwXN_g) [part 2](https://www.youtube.com/watch?v=SI7qtuuahhU)
* David Nolen [core.async webinar](http://go.cognitect.com/core_async_webinar_recording)

## Contributing 

[Contributing to Clojure projects](http://clojure.org/contributing) requires a signed Contributor Agreement. Pull requests and GitHub issues are not accepted; please use the [core.async JIRA project](http://dev.clojure.org/jira/browse/ASYNC) to report problems or enhancements.

## License

Copyright © 2013 Rich Hickey and contributors

Distributed under the Eclipse Public License, the same as Clojure.

## Changelog

* Release 0.2.382 on 2016.06.13
  * Change default dispatch thread pool size to 8.
  * Add Java system property `clojure.core.async.pool-size` to set the dispatch thread pool size
  * [ASYNC-152](http://dev.clojure.org/jira/browse/ASYNC-152) - disable t.a.jvm's warn-on-reflection pass 
* Release 0.2.374 on 2015.11.11
  * [ASYNC-149](http://dev.clojure.org/jira/browse/ASYNC-149) - fix error compiling recur inside case in a go block
  * Updated tools.analyzer.jvm version (and other upstream deps)
  * Updated to latest clojurescript and cljsbuild versions
* Release 0.2.371 on 2015.10.28
  * [ASYNC-124](http://dev.clojure.org/jira/browse/ASYNC-124) - dispatch multiple pending takers from expanding transducer
  * [ASYNC-103](http://dev.clojure.org/jira/browse/ASYNC-103) - NEW promise-chan
  * [ASYNC-104](http://dev.clojure.org/jira/browse/ASYNC-104) - NEW non-blocking offer!, poll!
  * [ASYNC-101](http://dev.clojure.org/jira/browse/ASYNC-101) - async/reduce now respects reduced
  * [ASYNC-112](http://dev.clojure.org/jira/browse/ASYNC-112) - replace "transformer" with "transducer" in deprecation messages
  * [ASYNC-6](http://dev.clojure.org/jira/browse/ASYNC-6) - alts! docs updated to explicitly state ports is a vector
  * Support (try (catch :default)) in CLJS exception handling
  * Use cljs.test
  * Updated tools.analyzer.jvm version (and other upstream deps)
* Release 0.1.346.0-17112a-alpha on 2014.09.22
  * cljs nextTick relies on goog.async.nextTick
  * Updated docstring for put! re result on closed channel
* Release 0.1.338.0-5c5012-alpha on 2014.08.19
  * Add cljs transducers support
* Release 0.1.319.0-6b1aca-alpha on 2014.08.06
  * Add transducers support
  * NEW pipeline
* Release 0.1.303.0-886421-alpha on 2014.05.08
* Release 0.1.301.0-deb34a-alpha on 2014.04.29
* Release 0.1.298.0-2a82a1-alpha on 2014.04.25
* Release 0.1.278.0-76b25b-alpha on 2014.02.07
* Release 0.1.267.0-0d7780-alpha on 2013.12.11
* Release 0.1.262.0-151b23-alpha on 2013.12.10
* Release 0.1.256.0-1bf8cf-alpha on 2013.11.07
* Release 0.1.242.0-44b1e3-alpha on 2013.09.27
* Release 0.1.222.0-83d0c2-alpha on 2013.09.12
