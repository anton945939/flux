# flux

A Clojure based Solr client, which supports Solr `7.4.0`.

## Installation (Leiningen)

To include the Flux library, add the following to your `:dependencies`:

    [net.expertsystem.lab.danton/flux "0.1.0"]

## Usage

To send a map.

    (:require [flux.http :as http]
           [flux.update :as update])
    (let [client (http/create page)]
    (.add client col (update/create-doc map) )
    (.commit client col)
    
## License

Copyright © 2013-2014 Matt Mitchell

Distributed under the Eclipse Public License, the same as Clojure.
