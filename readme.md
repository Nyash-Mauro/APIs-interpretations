<h1>API Architecture and Protocols</h1>

### REST
REST (representational state transfer) is a very popular web API architecture. To be a REST API, an API must adhere to certain architectural constraints, or principles, including:

    Client-server architecture: the interface is separated from the backend and data storage. This allows for flexibility, and for different components to evolve independent of each other.
    Statelessness: no client context is stored on the server between requests.
    Cacheability: clients can cache responses, so a REST API response must explicitly state whether it can be cached or not.
    Layered system: the API will work whether it is communicating directly with a server, or through an intermediary such as a load balancer.

### JSON-RPC and XML-RPC
An RPC is a remote procedural call protocol. XML-RPC uses XML to encode its calls, while JSON-RPC uses JSON for the encoding. Both protocols are simple. A call can contain multiple parameters, and expects one result. They have a couple of key features, which require a different architecture to REST:

    They are designed to call methods, whereas REST protocols involve the transfer of documents (resource representations). Or, to put it another way, REST works with resources, whereas RPC is about actions.
    The URI identifies the server, but contains no information in its parameters, whereas in REST the URI contains details such as query parameters.


### SOAP
SOAP (simple object access protocol) is an established web API protocol. It is intended to be extensible, neutral (able to operate over a range of communication protocols, including HTTP, SMTP, TCP and more), and independent (it allows for any programming style) The SOAP specification includes:

    The processing model: how to process a SOAP message.
    Extensibility model: SOAP features and modules.
    Protocol binding rules: how to use SOAP with an underlying protocol, such as HTTP.
    Message construct: how to structure a SOAP message.