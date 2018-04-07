# API Journey

# Table of Contents

- [Definitions](#definitions) - From the simplest definition of what a service does, all the way to the complete OpenAPI definition for each service.

- [Design](#design) - The consistent design of each service leverage existing patterns, as well as the web to deliver each service.

- [Caching](#caching) - What caching exists at the server, CDN, and DNS layers for each service to provide a higher level of performance?

- [Versioning](#versioning) - Plan for handling changes, and the inevitable evolution of each service, its definitions, and supporting code.

- [DNS](#dns) - The domain addressing being used for routing, management and auditing of all service traffic.

- [Deployment](#deployment) - Details services developed, and deployed, including frameworks and other libraries being used.

- [Orchestration](#orchestration) - Defining what the build, syndication, and orchestration of service deployments and integrations look like, and are executed.

- [Dependencies](#dependencies) - Identifying all backend service, code and infrastructure dependencies present for each service.

- [Search](#search) - Strategy for understanding what search will look like for each individual service, and play a role in larger, more comprehensive search across services.

- [Proxy](#proxy) - What proxies are in place to translate, cache, stream, and make services more efficient and secure?

- [Gateway](#gateway) - What gateways are in place to defend, protect, route, translate, and act as gatekeeper for service operations?

- [Virtualization](#virtualization) - Details how how services and their underlying data are mocked, virtualized, sandboxed, and made available for non-production usage.

- [Authentication](#authentication) - [What is involved with authentication across all services, including key-based approaches, basic authentication, JWT, and OAuth solutions.

- [Management](#management) - Information about how services are composed, limited, measured, reported upon, and managed consistently across all services.

- [Logging](#logging) - What is being logged as part of service operations, and what is required to participate in overall logging strategy?

- [Portal](#virtualization) - The strategy for how all services are required to be published to one or many public, private, and partner developer portals.

- [Documentation](#portal) - The requirements for what documentation is expected as part of each service presence, defining what the services delivers.

- [Support](#support) - Relevant support channels, points of contact, and best practices for receiving support as an API consumer.

- [Communications](#communications) - Information about the communication strategy around each service, and how blogs, social, and other channels should be leveraged.

- [Road Map](#road-map) - Details on a services road map, and what the future will hold, providing individual service, as well as larger organizational details on what is next.

- [Issues](#issues) - Expectations, communications, and transparency around what the current bugs, issues, and other active problems exist on a platform.

- [Change Log](#change-log) - Translating the road map, and issues into a log of activity that has occurred for each service, providing a history of the service.

- [Monitoring](#monitoring) - What is required when it comes to monitoring the availability and activity of each individual service.

- [Testing](#testing) - The tactical, as well as strategic testing that is involved with each service, ensuring it is meeting service level agreements.

- [Performance](#performance) - How is the performance of each service measured and report upon, providing a benchmark for the quality of service.

- [Observability](#observability) - What does observability of the service look like, providing transparency and accountability using all of its existing outputs?

- [Encryption](#encryption) - Details regarding what is expected regarding encryption on disk, as well as in transport for each service.

- [Security](#security) - Detailed strategy and processes regarding how each service is secured on a regular basis as part of operations.

- [Terms of Service](#terms-of-service) - Considerations, and legal requirements applied to each service as part of the overall, or individual terms of services.

- [Privacy](#privacy) - Details regarding the privacy of platform owners, developers, and end users as it pertains to service usage.

- [Service Level Agreements](#service-level-agreements) - Details regarding what service levels are required to be met when it comes to partner and public engagements.

- [Licensing](#licensing) - Information about backend server code, API surface area, data, and client licensing in play.

- [Branding](#branding) - What branding requirements are in place for the platforms and its partners when it comes to the service.

- [Regulation](#regulation) - Information regarding regulations in place that effect service operations, and are required as part of its usage.

- [Discovery](#discovery) - How are services catalogued and made discoverable, making them accessible to other systems, developers, as well as to internal, partner, or public groups.

- [Client](#client) - Information about clients being used to interface with and work with the service, allowing it to be put to use without code.

- [Command Line Interface](#command-line-interface) - The command line interface (CLI) tooling being used to developer or consume a service.

- [SDKs](#sdks) - What software development kits (SDK) are generated, or developed and maintained as part of a service’s operation?

- [Plugin](#plugin) - What platform plugins are developed and maintained as part of a services operations, allowing it to work with other platforms and services.

- [IDE](#ide) - Are there integrated development environment (IDE) integrations, libraries, plugins, or availability considerations for each service?

- [Browsers](#browsers) - Are there any browser plugins, add-ons, bookmarklets and integrations used as part of each service’s operation?

- [Embeddable](#embeddable) - Information about any embeddable badges, buttons, widgets, and other JavaScript enabled solutions built on top of a service?

- [Bots](#bots) - What type of automation and bot implementations are in development or being supported as part of a service’s operation?

- [Visualization](#visualization) - Are there specific visualizations that exist to help present the resources available within any service?

- [Analysis](#analysis) - How are logs, APIs, and other aspects of a service being used as part of wider analysis, and analytics strategy?

- [Aggregation](#aggregation) - Are there any aggregation solutions in place that involve the service, and depend on its availability?

- [Integration](#integration) - What 3rd party integrations are available for working with a service in existing integration platforms like IFTTT, and Zapier.

- [Network](#network) - Information about networks that are setup, used, and allocated for each service governing how it can be accessed and consumed.

- [Regions](#regions) - Which regions does a service operate within, making it available in specific regions, and jurisdictions–also which regions is it not allowed to operate within.

- [Webhooks](#webhooks) - Are there webhooks employed to respond to events that occur via the service, pushing data, and notification externally to consumers?

- [Migration](#migration) - What solutions are available for migrating an API between regions, cloud environments, and on-premise?

- [Backup](#backup) - What types of backups are in place to bring redundancy to the database, server, storage, and other essential aspects of a service’s operations?

- [Real Time](#real-time) - Are there Server-Sent Events (SSE), Websocket, Kafka, and other real time aspects of a service’s delivery?

- [Voice](#voice) - Are there any voice or speech enablement, integrating services with Alex, Siri, Google Home, or other conversational interface?

- [Spreadsheets](#spreadsheets) - What types of spreadsheet integrations, connectors, and publishing solutions are available for a service?

- [Investment](#investment) - Where do the funds for operating a service come from within a company, from external organizations, or VC funds?

- [Monetization](#monetization) - What does it cost to operate a service, breaking down the one time and recurring costs involved with delivering the service.

- [Plans](#plans) - Outline of plans involved with defining, measuring, reporting, and quantifying value generated around a service’s operation.

- [Partners](#partners) - An overview of partner program involved with a service’s operation, and how a wider partner strategy affects a service’s access and consumption.

- [Certification](#certification) - Are there certification channels available for applications and developers, defining the knowledge required to competently operate and integrate a service.

- [Evangelism](#evangelism) - What does internal, public, and partner evangelism efforts and requirements look like for a service, and its overall presence?

- [Showcase](#showcase) - How are developers and applications using a service showcased, and presented to the community, demonstrating the valuable around a service?

- [Deprecation](#deprecation) - What are the plans for deprecating a service, involved the road map and communication around the individual and overall deprecation of service(s).

- [Training](#training) - What training materials need to be developed, or already exist to support the service.

- [Governance](#governance) - How are all steps measured, quantified, aggregated, reported upon, and audited as part of a larger quality of service effort for each service.

<hr />

# Details

# Definitions
From the simplest definition of what a service does, all the way to the complete OpenAPI definition for each service. These are the artifacts that will guide each service through every step of the API lifecycle. API definitions are not just for documentation, or for generating code, they define the contract that a service delivers.

## Formats
Information regarding the different formats of definitions that are used across the entire API lifecycle, being applied across all of the stops along the journey.

- Web Concepts - APIs are built on the web, and there are numerous web concepts in play that should be considered as part of the API design process.

- Media Types - A media type (also MIME type and content type) is a two-part identifier for file formats and format contents transmitted on the Internet. The Internet Assigned Numbers Authority (IANA) is the official authority for the standardization and publication of these classifications.

- Specification - The root specification for the API definition format, providing a base set of rules for all services and tools that employ the spec.

- Schema - A representation of data model, used as part of an API request, or response, usually in JSON, but increasingly YAML, and Markdown are also used.

- Container File - Leveraging and approaching management of the container configuration files used as part of the container deliver process.

- Orchestration Artifacts - Being organized regarding how Jenkins, and other CI/CD configuration files are stored, configured, audited, and used across the lifecycle.

## Tooling
Defining the tooling that are available to work with definitions, providing a wide range of benefits to working with definitions across many areas in which the definitions are used.

- Generator - Generating an API definition format from an existing system or platform, outputting the portable machine readable format.

- Parser - Parses a machine readable API definition and makes ready for use in specific language, structure, or platform.

- Validator - Validates an API definition against its formal specification and schema, producing a valid or invalid response, with as much detail as possible.

- Converter - The conversion of an API definition from one format into another, allowing designers to share API definitions in any format.

- Command-Line - The usage of machine readable API definitions at the command line.

- Aggregator - Aggregation of APIs using a machine readable API definition format.

- Translator - Being able to translate an API definition format from one format to another, either manually or automatically.

- Merger - Tooling or other APIs that provide for the merging of common API definition formats, allowing the granularity of what elements get merged, or do not get merged. Ideally, this is an API, as well as simple web-based or desktop tooling for API providers and consumers.

- Difference - Providing side by side comparison of two API definitions, programmatically and visually helping identify between two API definitions. This allows for API architects, designers, and consumers to understand the completeness of two definitions, in relation to each other.

## Environment
Providing standardized environments for working with all of the definitions being used throughout the service delivery life cycle.

- Editors - API definition editor, allowing for the creation, import, and export of API definition formats, providing a simple, IDE like API editing experience.

- IDE Plugin - Providing integration with existing integrated development environments (IDE), giving developers API discovery, documentation, and integration tooling within the IDE.

- Forms - Dynamically generating an HTML form from an API definition, allow for the structure, and handling to be driven by an API definition.

- Github - Allowing for the import, publishing, and syncing of API definitions and schemas to Github for forking, and management using the social coding platform.

## Utilities

- Attribution - Where did the API definition originate? Is there a source where all or part of the API design came from? Providing design, or operational attribution, done via one of the API definitions.

- Annotation - Allowing for the annotation of API definitions, schemas, as part of the API life cycle.

- Proxy - Allowing for the proxying of API requests and responses using tools like Charles Proxy, or Prism from Stoplight, and generating of API definitions and schemas from the traffic.

# Design
The consistent design of each service leverage existing patterns, as well as focusing on the web to deliver services. Thinking critically, consistently, and practically about how we design the APIs, and evolve this practice with each version of our service.

## Healthy Practices
Good API design always begins with a set of healthy practices that transcend the technical, and help us deliver more meaningful solutions and services through the design of our programmatica interfaces.

- Use the Web - The web brings a lot of tools to the table, make sure and learn about existing web technologies, and put them to use across the API design process. APIs are just the next evolution in the web, where we think beyond just delivering data and content to the browser for human consumption, and think more about also working with mobile, device, and other types of applications, as well as system to system integration and automation.

- Simplicity - Consider simplicity at ever turn when designing APIs, providing the small possible unit of value you possibly can--simplicity goes a long way.

- Consistency - Employ consistent approaches to all aspects of API design, providing a familiar approach across all APIs published.

- Easy to Read - While APIs are for computers, they should be easy to read by humans, making documentation more accessible.

- Easy to Learn - Keeping APIs simple, and consistent, will contribute to them being easy to learn about for any potential API consumer.

- Hard to Misuse - When APIs do one thing, and does it well, you reduce the opportunity for misuse, and people putting them to work in unintended ways.

- Audience Focused - APIs should be designed with a specific audience in mind, providing a solution to a problem they are having.

- Experience Over Resource - Make APIs reflect how they will be used, and experienced, over where the API came from and how the resource it was derived from--despite what you may learn from the API design handbook.

- Naming - Intuitively naming things and making sure they make sense to other human beings, and avoiding acronyms, and other cryptic approaches to naming things.

- Case - Which case (lowercase, camelCase, ...) to use and when, while being as consistent as you can.

- Global design - Think outside your city, state, and country when it comes to designing your APIs. Don't just design for your bubble. Design as if people around the world will be putting your API resources to work in their applications.

## HTTP Requests
Defining common patterns that can be used across the request structure of all services, helping ensure consistent interfaces for putting platform services. to work.

- SSL - Transport Layer Security (TLS) and its predecessor, Secure Sockets Layer (SSL), both of which are frequently referred to as 'SSL', are cryptographic protocols designed to provide communications security over a computer network. Always support TLS / SSL by default when it comes to API operations, if at all possible.

- Host - Put sufficient thought into what the baseURL will be for making API calls. Increasingly this element can also be dynamic, like other aspects of API design.

- Resource - Consider how you craft your resources across all API operations. I do not subscribe to specific philosophies around this, just trying to provide a framework to think about this in.

- Action - Allow for standard actions to be taken across resource, but also reflect how APIs will be experienced, providing meaningful action to be taken around any API.

- Parameters - Standardize how parameters are crafted as part of API operations, using intuitive and consistent approaches.

- Body - Use the body of each request in a consistent way across API operations. The body provides much more room for more structured data and content.

- Pagination - Learn about common ways to paginate, and establish a single way to handle across API operations.

- Filtering - Consider how filtering will happen across all APIs, and establish a single way to filter API resources.

- Time Selection - Consider how time selection and series will be handled, and establish a single way for working with time in API operations.

- Sorting - Establish a single approach to how API responses can be sorted, and use across all API resources.

- Field Selection - Consider providing a way that API consumers can select which fields are included in API responses.

- Granularity - Always be aware of the granularity of your API endpoints, and each resource being exposed, keeping everything as small as possible.

- Scope - considering the overall scope and size of the API and its individual paths, keeping things as small and focused as they possibly can.

## HTTP Request Methods
Leverage the web, and utilizing all of the HTTP Request Methods that are available to work with, keeping the methods that are available for each service consistent with how the web works.

- ACL (RFC 3744) - The ACL method modifies the access control list (which can be read via the DAV:acl property) of a resource. Specifically, the ACL method only permits modification to ACEs that are not inherited, and are not protected. - http://webconcepts.info/concepts/http-method/

- BASELINE-CONTROL (RFC 3253) - A collection can be placed under baseline control with a BASELINE-CONTROL request. When a collection is placed under baseline control, the DAV:version-controlled-configuration property of the collection is set to identify a new version-controlled configuration. This version-controlled configuration can be checked out and then checked in to create a new baseline for that collection. - http://webconcepts.info/concepts/http-method/

- BIND (RFC 5842) - The BIND method modifies the collection identified by the Request-URI, by adding a new binding from the segment specified in the BIND body to the resource identified in the BIND body. - http://webconcepts.info/concepts/http-method/

- CHECKIN (RFC 3253) - A CHECKIN request can be applied to a checked-out version-controlled resource to produce a new version whose content and dead properties are copied from the checked-out resource. - http://webconcepts.info/concepts/http-method/

- CHECKOUT (RFC 3253) - A CHECKOUT request can be applied to a checked-in version-controlled resource to allow modifications to the content and dead properties of that version-controlled resource. - http://webconcepts.info/concepts/http-method/

- CONNECT (RFC 7231) - The CONNECT method requests that the recipient establish a tunnel to the destination origin server identified by the request-target and, if successful, thereafter restrict its behavior to blind forwarding of packets, in both directions, until the tunnel is closed. Tunnels are commonly used to create an end-to-end virtual connection, through one or more proxies, which can then be secured using TLS (Transport Layer Security). - http://webconcepts.info/concepts/http-method/

- COPY (RFC 4918) - The COPY method creates a duplicate of the source resource identified by the Request-URI, in the destination resource identified by the URI in the Destination header. The Destination header MUST be present. The exact behavior of the COPY method depends on the type of the source resource. - http://webconcepts.info/concepts/http-method/

- DELETE (RFC 7231) - The DELETE method requests that the origin server remove the association between the target resource and its current functionality. In effect, this method is similar to the rm command in UNIX: it expresses a deletion operation on the URI mapping of the origin server rather than an expectation that the previously associated information be deleted. - http://webconcepts.info/concepts/http-method/

- GET (RFC 7231) - The GET method requests transfer of a current selected representation for the target resource. GET is the primary mechanism of information retrieval and the focus of almost all performance optimizations. Hence, when people speak of retrieving some identifiable information via HTTP, they are generally referring to making a GET request. - http://webconcepts.info/concepts/http-method/

- HEAD (RFC 7231) - The HEAD method is identical to GET except that the server MUST NOT send a message body in the response (i.e., the response terminates at the end of the header section). The server SHOULD send the same header fields in response to a HEAD request as it would have sent if the request had been a GET, except that the payload header fields MAY be omitted. This method can be used for obtaining metadata about the selected representation without transferring the representation data and is often used for testing hypertext links for validity, accessibility, and recent modification. - http://webconcepts.info/concepts/http-method/

- LABEL (RFC 3253) - A LABEL request can be applied to a version to modify the labels that select that version. The case of a label name MUST be preserved when it is stored and retrieved. When comparing two label names to decide if they match or not, a server SHOULD use a case-sensitive URL-escaped UTF-8 encoded comparison of the two label names. - http://webconcepts.info/concepts/http-method/

- LINK (Internet Draft snell-link-method) - The LINK method is used to establish one or more relationships between the resource identified by the effective request URI and one or more other resources. - http://webconcepts.info/concepts/http-method/

- LOCK (RFC 4918) - The LOCK method is used to take out a lock of any access type and to refresh an existing lock. - http://webconcepts.info/concepts/http-method/

- MERGE (RFC 3253) - The MERGE method performs the logical merge of a specified version (the "merge source") into a specified version-controlled resource (the "merge target"). If the merge source is neither an ancestor nor a descendant of the DAV:checked-in or DAV:checked-out version of the merge target, the MERGE checks out the merge target (if it is not already checked out) and adds the URL of the merge source to the DAV:merge-set of the merge target. - http://webconcepts.info/concepts/http-method/

- MKACTIVITY (RFC 3253) - A MKACTIVITY request creates a new activity resource. A server MAY restrict activity creation to particular collections, but a client can determine the location of these collections from a DAV:activity-collection-set OPTIONS request. - http://webconcepts.info/concepts/http-method/

- MKCALENDAR (RFC 4791) - An HTTP request using the MKCALENDAR method creates a new calendar collection resource. A server MAY restrict calendar collection creation to particular collections. - http://webconcepts.info/concepts/http-method/

- MKCOL (RFC 4918) - MKCOL creates a new collection resource at the location specified by the Request-URI. If the Request-URI is already mapped to a resource, then the MKCOL MUST fail. During MKCOL processing, a server MUST make the Request-URI an internal member of its parent collection, unless the Request-URI is "/". If no such ancestor exists, the method MUST fail. When the MKCOL operation creates a new collection resource, all ancestors MUST already exist, or the method MUST fail with a 409 (Conflict) status code. - http://webconcepts.info/concepts/http-method/

- MKREDIRECTREF (RFC 4437) - The MKREDIRECTREF method requests the creation of a redirect reference resource. - http://webconcepts.info/concepts/http-method/

- MKWORKSPACE (RFC 3253) - A MKWORKSPACE request creates a new workspace resource. A server MAY restrict workspace creation to particular collections, but a client can determine the location of these collections from a DAV:workspace-collection-set OPTIONS request. - http://webconcepts.info/concepts/http-method/

- MOVE (RFC 4918) - The MOVE operation on a non-collection resource is the logical equivalent of a copy (COPY), followed by consistency maintenance processing, followed by a delete of the source, where all three actions are performed in a single operation. The consistency maintenance step allows the server to perform updates caused by the move, such as updating all URLs, other than the Request-URI that identifies the source resource, to point to the new destination resource. - http://webconcepts.info/concepts/http-method/

- OPTIONS (RFC 7231) - The OPTIONS method requests information about the communication options available for the target resource, at either the origin server or an intervening intermediary. This method allows a client to determine the options and/or requirements associated with a resource, or the capabilities of a server, without implying a resource action. - http://webconcepts.info/concepts/http-method/

- ORDERPATCH (RFC 3648) - The ORDERPATCH method is used to change the ordering semantics of a collection, to change the order of the collection's members in the ordering, or both. - http://webconcepts.info/concepts/http-method/

- PATCH (RFC 5789) - The PATCH method requests that a set of changes described in the request entity be applied to the resource identified by the Request-URI. The set of changes is represented in a format called a "patch document" identified by a media type. If the Request-URI does not point to an existing resource, the server MAY create a new resource, depending on the patch document type (whether it can logically modify a null resource) and permissions, etc. - http://webconcepts.info/concepts/http-method/

- POST (RFC 7231) - The POST method requests that the target resource process the representation enclosed in the request according to the resource's own specific semantics. - http://webconcepts.info/concepts/http-method/

- PRI (RFC 7540) - This method is never used by an actual client. This method will appear to be used when an HTTP/1.1 server or intermediary attempts to parse an HTTP/2 connection preface. - http://webconcepts.info/concepts/http-method/

- PROPFIND (RFC 4918) - The PROPFIND method retrieves properties defined on the resource identified by the Request-URI, if the resource does not have any internal members, or on the resource identified by the Request-URI and potentially its member resources, if the resource is a collection that has internal member URLs. - http://webconcepts.info/concepts/http-method/

- PROPPATCH (RFC 4918) - The PROPPATCH method processes instructions specified in the request body to set and/or remove properties defined on the resource identified by the Request-URI. - http://webconcepts.info/concepts/http-method/

- PUT (RFC 7231) - The PUT method requests that the state of the target resource be created or replaced with the state defined by the representation enclosed in the request message payload. A successful PUT of a given representation would suggest that a subsequent GET on that same target resource will result in an equivalent representation being sent in a 200 (OK) response. However, there is no guarantee that such a state change will be observable, since the target resource might be acted upon by other user agents in parallel, or might be subject to dynamic processing by the origin server, before any subsequent GET is received. A successful response only implies that the user agent's intent was achieved at the time of its processing by the origin server. - http://webconcepts.info/concepts/http-method/

- REBIND (RFC 5842) - The REBIND method removes a binding to a resource from a collection, and adds a binding to that resource into the collection identified by the Request-URI. The request body specifies the binding to be added (segment) and the old binding to be removed (href). It is effectively an atomic form of a MOVE request, and MUST be treated the same way as MOVE for the purpose of determining access permissions. - http://webconcepts.info/concepts/http-method/

- REPORT (RFC 3253) - A REPORT request is an extensible mechanism for obtaining information about a resource. Unlike a resource property, which has a single value, the value of a report can depend on additional information specified in the REPORT request body and in the REPORT request headers. - http://webconcepts.info/concepts/http-method/

- SEARCH (RFC 5323) - The client invokes the SEARCH method to initiate a server-side search. The body of the request defines the query. The server MUST emit an entity matching the WebDAV multistatus format. - http://webconcepts.info/concepts/http-method/

- TRACE (RFC 7231) - The TRACE method requests a remote, application-level loop-back of the request message. The final recipient of the request SHOULD reflect the message received, excluding some fields described below, back to the client as the message body of a 200 (OK) response with a Content-Type of "message/http". The final recipient is either the origin server or the first server to receive a Max-Forwards value of zero (0) in the request. - http://webconcepts.info/concepts/http-method/

- UNBIND (RFC 5842) - The UNBIND method modifies the collection identified by the Request-URI by removing the binding identified by the segment specified in the UNBIND body. - http://webconcepts.info/concepts/http-method/

- UNCHECKOUT (RFC 3253) - An UNCHECKOUT request can be applied to a checked-out version-controlled resource to cancel the CHECKOUT and restore the pre-CHECKOUT state of the version-controlled resource. - http://webconcepts.info/concepts/http-method/

- UNLINK (Internet Draft snell-link-method) - The UNLINK method is used to remove one or more relationships between the resource identified by the effective request URI and other resources. - http://webconcepts.info/concepts/http-method/

- UNLOCK (RFC 4918) - The UNLOCK method removes the lock identified by the lock token in the Lock-Token request header. The Request-URI MUST identify a resource within the scope of the lock. - http://webconcepts.info/concepts/http-method/

- UPDATE (RFC 3253) - The UPDATE method modifies the content and dead properties of a checked-in version-controlled resource (the "update target") to be those of a specified version (the "update source") from the version history of that version-controlled resource. - http://webconcepts.info/concepts/http-method/

- UPDATEREDIRECTREF (RFC 4437) - The UPDATEREDIRECTREF method requests the update of a redirect reference resource. - http://webconcepts.info/concepts/http-method/

- VERSION-CONTROL (RFC 3253) - A VERSION-CONTROL request can be used to create a version-controlled resource at the request-URL. It can be applied to a versionable resource or to a version-controlled resource. - http://webconcepts.info/concepts/http-method/

## Headers
Providing a list of standard HTTP headers that can be used as part of the API design process, educating developers of what is possible, and standardizing the usage of HTTP building blocks that are already making up the web, versus reinventing the wheel and implementing custom behaviors.

- A-IM (RFC 3229) - The A-IM request-header field is similar to Accept, but restricts the instance-manipulations that are acceptable in the response. A response may be the result of applying multiple instance-manipulations. When an A-IM request-header field includes one or more delta-coding values, the request MUST contain an If-None-Match header field, listing one or more entity tags from prior responses for the request-URI. - http://webconcepts.info/concepts/http-header/

- ALPN (RFC 7639) - Clients include the ALPN header field in an HTTP CONNECT request to indicate the application-layer protocol that a client intends to use within the tunnel, or a set of protocols that might be used within the tunnel. - http://webconcepts.info/concepts/http-header/

- Accept (RFC 7231) - The "Accept" header field can be used by user agents to specify response media types that are acceptable. Accept header fields can be used to indicate that the request is specifically limited to a small set of desired types, as in the case of a request for an in-line image. - http://webconcepts.info/concepts/http-header/

- Accept-Additions (RFC 2324RFC 7168) - In HTTP, the "Accept" request-header field is used to specify media types which are acceptable for the response. However, in HTCPCP, the response may result in additional actions on the part of the automated pot. For this reason, HTCPCP adds a new header field, "Accept-Additions".It has been observed that some users of blended teas have an occasional preference for teas brewed as an emulsion of cane sugar with hints of water. To allow for this circumstance, the Accept-Additions header field defined in the base HTCPCP specification is updated to allow the following options. - http://webconcepts.info/concepts/http-header/

- Accept-CH (Internet Draft ietf-httpbis-client-hints) - Servers can advertise support for Client Hints using the Accept-CH header field or an equivalent HTML meta element with http-equiv attribute. - http://webconcepts.info/concepts/http-header/

- Accept-CH-Lifetime (Internet Draft ietf-httpbis-client-hints) - Servers can ask the client to remember an origin-wide Accept-CH preference for a specified period of time to enable delivery of Client Hints on all subsequent requests to the origin, and on subresource requests initiated as a result of processing a response from the origin. - http://webconcepts.info/concepts/http-header/

- Accept-Charset (RFC 7231) - The "Accept-Charset" header field can be sent by a user agent to indicate what charsets are acceptable in textual response content. This field allows user agents capable of understanding more comprehensive or special-purpose charsets to signal that capability to an origin server that is capable of representing information in those charsets. - http://webconcepts.info/concepts/http-header/

- Accept-Datetime (RFC 7089) - The "Accept-Datetime" request header is transmitted by a user agent to indicate it wants to access a past state of an Original Resource. To that end, the "Accept-Datetime" header is conveyed in an HTTP request issued against a TimeGate for an Original Resource, and its value indicates the datetime of the desired past state of the Original Resource. - http://webconcepts.info/concepts/http-header/

- Accept-Encoding (RFC 7694RFC 7231) - Section 5.3.4 of RFC 7231 defines "Accept-Encoding" as a request header field only. This specification expands that definition to allow "Accept-Encoding" as a response header field as well. When present in a response, it indicates what content codings the resource was willing to accept in the associated request. A field value that only contains "identity" implies that no content codings were supported.The "Accept-Encoding" header field can be used by user agents to indicate what response content-codings are acceptable in the response. An "identity" token is used as a synonym for "no encoding" in order to communicate when no encoding is preferred. - http://webconcepts.info/concepts/http-header/

- Accept-Features (RFC 2295) - The Accept-Features request header can be used by a user agent to give information about the presence or absence of certain features in the feature set of the current request. Servers can use this information when running a remote variant selection algorithm. - http://webconcepts.info/concepts/http-header/

- Accept-Indefinite-Ranges (Internet Draft combs-http-indeterminate-range) - The Accept-Indefinite-Ranges request-header field allows the client to indicate its acceptance of indefinite-sized range requests for a resource. - http://webconcepts.info/concepts/http-header/

- Accept-Language (RFC 7231) - The "Accept-Language" header field can be used by user agents to indicate the set of natural languages that are preferred in the response. - http://webconcepts.info/concepts/http-header/

- Accept-Patch (RFC 5789) - This specification introduces a new response header Accept-Patch used to specify the patch document formats accepted by the server. Accept-Patch SHOULD appear in the OPTIONS response for any resource that supports the use of the PATCH method. The presence of the Accept-Patch header in response to any method is an implicit indication that PATCH is allowed on the resource identified by the Request-URI. - http://webconcepts.info/concepts/http-header/

- Accept-Post (W3C TR http://www.w3.org/TR/ldp) - The Accept-Post HTTP header SHOULD appear in the OPTIONS response for any resource that supports the use of the POST method. The presence of the Accept-Post header in response to any method is an implicit indication that POST is allowed on the resource identified by the Request-URI. The presence of a specific document format in this header indicates that that specific format is allowed on POST requests to the resource identified by the Request-URI. - http://webconcepts.info/concepts/http-header/

- Accept-Push-Policy (Internet Draft ruellan-http-accept-push-policy) - A client can express the desired push policy for a request by sending an "Accept-Push-Policy" header field in the request. The header field value contains the push policy that the client expects the server to use when processing the request. - http://webconcepts.info/concepts/http-header/

- Accept-Ranges (RFC 7233) - The "Accept-Ranges" header field allows a server to indicate that it supports range requests for the target resource. - http://webconcepts.info/concepts/http-header/

- Access-Control-Allow-Credentials (W3C TR http://www.w3.org/TR/cors) - The Access-Control-Allow-Credentials header indicates whether the response to request can be exposed when the omit credentials flag is unset. When part of the response to a preflight request it indicates that the actual request can include user credentials. - http://webconcepts.info/concepts/http-header/

- Access-Control-Allow-Headers (W3C TR http://www.w3.org/TR/cors) - The Access-Control-Allow-Headers header indicates, as part of the response to a preflight request, which header field names can be used during the actual request. - http://webconcepts.info/concepts/http-header/

- Access-Control-Allow-Methods (W3C TR http://www.w3.org/TR/cors) - The Access-Control-Allow-Methods header indicates, as part of the response to a preflight request, which methods can be used during the actual request. - http://webconcepts.info/concepts/http-header/

- Access-Control-Allow-Origin (W3C TR http://www.w3.org/TR/cors) - The Access-Control-Allow-Origin header indicates whether a resource can be shared based by returning the value of the Origin request header, "*", or "null" in the response. - http://webconcepts.info/concepts/http-header/

- Access-Control-Expose-Headers (W3C TR http://www.w3.org/TR/cors) - The Access-Control-Expose-Headers header indicates which headers are safe to expose to the API of a CORS API specification. - http://webconcepts.info/concepts/http-header/

- Access-Control-Max-Age (W3C TR http://www.w3.org/TR/cors) - The Access-Control-Max-Age header indicates how long the results of a preflight request can be cached in a preflight result cache. - http://webconcepts.info/concepts/http-header/

- Access-Control-Request-Headers (W3C TR http://www.w3.org/TR/cors) - The Access-Control-Request-Headers header indicates which headers will be used in the actual request as part of the preflight request. - http://webconcepts.info/concepts/http-header/

- Access-Control-Request-Method (W3C TR http://www.w3.org/TR/cors) - The Access-Control-Request-Method header indicates which method will be used in the actual request as part of the preflight request. - http://webconcepts.info/concepts/http-header/

- Age (RFC 7234) - The "Age" header field conveys the sender's estimate of the amount of time since the response was generated or successfully validated at the origin server. - http://webconcepts.info/concepts/http-header/

- Allow (RFC 7231) - The "Allow" header field lists the set of methods advertised as supported by the target resource. The purpose of this field is strictly to inform the recipient of valid request methods associated with the resource. - http://webconcepts.info/concepts/http-header/

- Alt-Svc (RFC 7838) - An HTTP(S) origin server can advertise the availability of alternative services to clients by adding an Alt-Svc header field to responses. - http://webconcepts.info/concepts/http-header/

- Alt-Used (RFC 7838) - The Alt-Used header field is used in requests to indicate the identity of the alternative service in use, just as the Host header field identifies the host and port of the origin. Alt-Used is intended to allow alternative services to detect loops, differentiate traffic for purposes of load balancing, and generally to ensure that it is possible to identify the intended destination of traffic, since introducing this information after a protocol is in use has proven to be problematic. - http://webconcepts.info/concepts/http-header/

- Alternates (RFC 2295) - The Alternates response header is used to convey the list of variants bound to a negotiable resource. This list can also include directives for any content negotiation process. If a response from a transparently negotiable resource includes an Alternates header, this header MUST contain the complete variant list bound to the negotiable resource. Responses from resources which do not support transparent content negotiation MAY also use Alternates headers. - http://webconcepts.info/concepts/http-header/

- Apply-To-Redirect-Ref (RFC 4437) - The optional Apply-To-Redirect-Ref header can be used on any request to a redirect reference resource. When it is present and set to "T", the request MUST be applied to the reference resource itself, and a 3xx response MUST NOT be returned. - http://webconcepts.info/concepts/http-header/

- Authentication-Control (RFC 8053) - The Authentication-Control header provides more precise control of the client behavior for Web applications using an HTTP authentication protocol. - http://webconcepts.info/concepts/http-header/

- Authentication-Info (RFC 7615) - HTTP authentication schemes can use the Authentication-Info response header field to communicate information after the client's authentication credentials have been accepted. This information can include a finalization message from the server (e.g., it can contain the server authentication). - http://webconcepts.info/concepts/http-header/

- Authorization (RFC 7616RFC 5849RFC 7235) - The client is expected to retry the request, passing an Authorization header field line with Digest scheme, which is defined according to the framework above. The values of the opaque and algorithm fields must be those supplied in the WWW-Authenticate response header field for the entity being requested.Protocol parameters can be transmitted using the HTTP "Authorization" header field as defined by RFC 2617 with the auth-scheme name set to "OAuth" (case insensitive).The "Authorization" header field allows a user agent to authenticate itself with an origin server - usually, but not necessarily, after receiving a 401 (Unauthorized) response. Its value consists of credentials containing the authentication information of the user agent for the realm of the resource being requested. - http://webconcepts.info/concepts/http-header/

- C-Ext (RFC 2774) - The C-Ext response header field is used to indicate that all hop-by-hop mandatory extension declarations in the request were fulfilled. - http://webconcepts.info/concepts/http-header/

- C-Man (RFC 2774) - A mandatory extension declaration indicates that the ultimate recipient MUST consult and adhere to the rules given by the extension when processing the message or reporting an error. Hop-by-hop extension declarations are meaningful only for a single HTTP connection. In HTTP/1.1, C-Man, C-Opt, and all header fields with matching header-prefix values defined by C-Man and C-Opt MUST be protected by a Connection header field. That is, these header fields are to be included as Connection header field directives. - http://webconcepts.info/concepts/http-header/

- C-Opt (RFC 2774) - An optional extension declaration indicates that the ultimate recipient of the extension MAY consult and adhere to the rules given by the extension when processing the message, or ignore the extension declaration completely. An agent may not be able to distinguish whether the ultimate recipient does not understand an extension referred to by an optional extension or simply ignores the extension declaration. Hop-by-hop extension declarations are meaningful only for a single HTTP connection. In HTTP/1.1, C-Man, C-Opt, and all header fields with matching header-prefix values defined by C-Man and C-Opt MUST be protected by a Connection header field. That is, these header fields are to be included as Connection header field directives. - http://webconcepts.info/concepts/http-header/

- C-PEP (W3C TR http://www.w3.org/TR/WD-http-pep) - PEP hop-by-hop extension declarations are meaningful only for a single transport-level connection. The C-PEP header field is a hop-by-hop header field and must not be communicated by proxies over further connections. - http://webconcepts.info/concepts/http-header/

- C-PEP-Info (W3C TR http://www.w3.org/TR/WD-http-pep) - PEP hop-by-hop policies are meaningful only for a single transport-level connection. The C-PEP-Info header field is a hop-by-hop header field and MUST NOT be communicated by proxies over further connections. - http://webconcepts.info/concepts/http-header/

- Cache-Control (RFC 7234) - The "Cache-Control" header field is used to specify directives for caches along the request/response chain. Such cache directives are unidirectional in that the presence of a directive in a request does not imply that the same directive is to be given in the response. - http://webconcepts.info/concepts/http-header/

- Cache-NT (Internet Draft drechsler-httpbis-improved-caching) - For precisely identifying transferred content independent of the used URL and independent of additional header fields in the context of content negotiation, the Cache-NT header field is used. The new header field carries an SHA-256 value. - http://webconcepts.info/concepts/http-header/

- Cal-Managed-ID (Internet Draft ietf-calext-caldav-attachments) - The Cal-Managed-ID response header field provides the value of the MANAGED-ID parameter corresponding to a newly added ATTACH property. It MUST be sent only in response to a successful POST request with an action set to attachment-add or attachment-update. - http://webconcepts.info/concepts/http-header/

- Clear-Site-Data (W3C TR http://www.w3.org/TR/clear-site-data) - The Clear-Site-Data HTTP response header field sends a signal to the user agent that it ought to remove all data of a certain set of types. - http://webconcepts.info/concepts/http-header/

- Close (RFC 7230) - The header field-name "Close" has been registered as "reserved", since using that name as an HTTP header field might conflict with the "close" connection option of the Connection header field. - http://webconcepts.info/concepts/http-header/

- Connection (RFC 7230) - The "Connection" header field allows the sender to indicate desired control options for the current connection. In order to avoid confusing downstream recipients, a proxy or gateway MUST remove or replace any received connection options before forwarding the message. - http://webconcepts.info/concepts/http-header/

- Content-Base (RFC 2068) - The Content-Base entity-header field may be used to specify the base URI for resolving relative URLs within the entity. This header field is described as Base in RFC 1808, which is expected to be revised. - http://webconcepts.info/concepts/http-header/

- Content-DPR (Internet Draft ietf-httpbis-client-hints) - The "Content-DPR" header field is a number that indicates the ratio between physical pixels over CSS px of the selected image response. - http://webconcepts.info/concepts/http-header/

- Content-Disposition (RFC 6266) - The Content-Disposition response header field is used to convey additional information about how to process the response payload, and also can be used to attach additional metadata, such as the filename to use when saving the response payload locally. - http://webconcepts.info/concepts/http-header/

- Content-Encoding (RFC 7231) - The "Content-Encoding" header field indicates what content codings have been applied to the representation, beyond those inherent in the media type, and thus what decoding mechanisms have to be applied in order to obtain data in the media type referenced by the Content-Type header field. Content-Encoding is primarily used to allow a representative's data to be compressed without losing the identity of its underlying media type. - http://webconcepts.info/concepts/http-header/

- Content-Language (RFC 7231) - The "Content-Language" header field describes the natural language(s) of the intended audience for the representation. Note that this might not be equivalent to all the languages used within the representation. - http://webconcepts.info/concepts/http-header/

- Content-Length (RFC 7230) - When a message does not have a Transfer-Encoding header field, a Content-Length header field can provide the anticipated size, as a decimal number of octets, for a potential payload body. For messages that do include a payload body, the Content-Length field-value provides the framing information necessary for determining where the body (and message) ends. For messages that do not include a payload body, the Content-Length indicates the size of the selected representation.. - http://webconcepts.info/concepts/http-header/

- Content-Location (RFC 7231) - The "Content-Location" header field references a URI that can be used as an identifier for a specific resource corresponding to the representation in this message payload. In other words, if one were to perform a GET request on this URI at the time of this message's generation, then a 200 (OK) response would contain the same representation that is enclosed as payload in this message. - http://webconcepts.info/concepts/http-header/

- Content-Range (Internet Draft combs-http-indeterminate-range RFC 7233) - The Content-Range entity-header is sent with a partial entity-body to specify where in the full entity-body the partial body should be applied.The "Content-Range" header field is sent in a single part 206 (Partial Content) response to indicate the partial range of the selected representation enclosed as the message payload, sent in each part of a multipart 206 response to indicate the range enclosed within each body part, and sent in 416 (Range Not Satisfiable) responses to provide information about the selected representation. - http://webconcepts.info/concepts/http-header/

- Content-Security-Policy (W3C TR http://www.w3.org/TR/CSP3W3C TR http://www.w3.org/TR/CSP2) - The Content-Security-Policy HTTP response header field is the preferred mechanism for delivering a policy from a server to a client.The Content-Security-Policy header field is the preferred mechanism for delivering a policy. - http://webconcepts.info/concepts/http-header/

- Content-Security-Policy-Pin (W3C TR http://www.w3.org/TR/csp-pinning) - The Content-Security-Policy-Pin header field is the mechanism for delivering a pinned policy that the user agent MUST enforce for any resource which is not delivered with a Content-Security-Policy header (as described in the "Pin a policy to response" algorithm). - http://webconcepts.info/concepts/http-header/

- Content-Security-Policy-Report-Only (W3C TR http://www.w3.org/TR/CSP3W3C TR http://www.w3.org/TR/CSP2) - The Content-Security-Policy-Report-Only HTTP response header field allows web developers to experiment with policies by monitoring (but not enforcing) their effects.The Content-Security-Policy-Report-Only header field lets servers experiment with policies by monitoring (rather than enforcing) a policy. - http://webconcepts.info/concepts/http-header/

- Content-Security-Policy-Report-Only-Pin (W3C TR http://www.w3.org/TR/csp-pinning) - The Content-Security-Policy-Report-Only-Pin header field is the mechanism for delivering a pinned policy that the user agent MUST monitor for any resource which is not delivered with a Content-Security-Policy-Report-Only header (as described in the "Pin a policy to response" algorithm). - http://webconcepts.info/concepts/http-header/

- Content-Signature (Internet Draft thomson-http-content-signature) - The Content-Signature header field carries a signature of the payload body of an HTTP message. This allows for content to be protected from modification. - http://webconcepts.info/concepts/http-header/

- Content-Translation-Type (RFC 8255) - The Content-Translation-Type field can be used in the individual language message parts to identify the type of translation. Based on the value of this field and the user's preferences, a conforming email client can determine which message part to display. - http://webconcepts.info/concepts/http-header/

- Content-Type (RFC 7231) - The "Content-Type" header field indicates the media type of the associated representation: either the representation enclosed in the message payload or the selected representation, as determined by the message semantics. The indicated media type defines both the data format and how that data is intended to be processed by a recipient, within the scope of the received message semantics, after any content codings indicated by Content-Encoding are decoded. - http://webconcepts.info/concepts/http-header/

- Content-Version (RFC 2068) - The Content-Version entity-header field defines the version tag associated with a rendition of an evolving entity. Together with the Derived-From field, it allows a group of people to work simultaneously on the creation of a work as an iterative process. The field should be used to allow evolution of a particular work along a single path rather than derived works or renditions in different representations. - http://webconcepts.info/concepts/http-header/

- Cookie (Internet Draft ietf-httpbis-rfc6265bis RFC 6265) - The user agent sends stored cookies to the origin server in the Cookie header.The user agent sends stored cookies to the origin server in the Cookie header. - http://webconcepts.info/concepts/http-header/

- Cookie2 (RFC 2965) - The Cookie2 request header facilitates interoperation between clients and servers that understand different versions of the cookie specification. - http://webconcepts.info/concepts/http-header/

- DASL (RFC 5323) - The DASL response header indicates server support for query grammars in the OPTIONS method. The value is a list of URIs that indicate the types of supported grammars. Note that although the URIs can be used to identify each supported search grammar, there is not necessarily a direct relationship between the URI and the XML element name that can be used in XML based SEARCH requests (the element name itself is identified by its namespace name (a URI reference) and the element's local name). - http://webconcepts.info/concepts/http-header/

- DAV (RFC 4918) - This general-header appearing in the response indicates that the resource supports the DAV schema and protocol as specified. As a request header, this header allows the client to advertise compliance with named features when the server needs that information. - http://webconcepts.info/concepts/http-header/

- DNT (W3C TR http://www.w3.org/TR/tracking-dnt) - The DNT header field is defined as the means for expressing a user's tracking preference via HTTP. - http://webconcepts.info/concepts/http-header/

- DPR (Internet Draft ietf-httpbis-client-hints) - The "DPR" header field is a number that, in requests, indicates the client's current Device Pixel Ratio (DPR), which is the ratio of physical pixels over CSS px of the layout viewport on the device. - http://webconcepts.info/concepts/http-header/

- Date (RFC 7231) - The "Date" header field represents the date and time at which the message was originated, having the same semantics as the Origination Date Field (orig-date) defined in Section 3.6.1 of RFC 5322. - http://webconcepts.info/concepts/http-header/

- Delta-Base (RFC 3229) - The Delta-Base entity-header field is used in a delta-encoded response to specify the entity tag of the base instance. A Delta-Base header field MUST be included in a response with an IM header that includes a delta-coding, if the request included more than one entity tag in its If-None-Match header field. Any response with an IM header that includes a delta-coding MAY include a Delta-Base header. - http://webconcepts.info/concepts/http-header/

- Depth (RFC 4918) - The Depth request header is used with methods executed on resources that could potentially have internal members to indicate whether the method is to be applied only to the resource ("Depth: 0"), to the resource and its internal members only ("Depth: 1"), or the resource and all its members ("Depth: infinity"). - http://webconcepts.info/concepts/http-header/

- Destination (RFC 4918) - The Destination request header specifies the URI that identifies a destination resource for methods such as COPY and MOVE, which take two URIs as parameters. - http://webconcepts.info/concepts/http-header/

- Digest (RFC 3230) - The Digest message header field provides a message digest of the instance described by the message. - http://webconcepts.info/concepts/http-header/

- Downlink (Internet Draft ietf-httpbis-client-hints) - The "Downlink" header field is a number that, in requests, indicates the client's maximum downlink speed in megabits per second (Mbps), as defined by the "downlinkMax" attribute in the W3C Network Information API. - http://webconcepts.info/concepts/http-header/

- EDIINT-Features (RFC 6017) - The EDIINT-Features header field indicates the originating user agent is capable of supporting the features listed. - http://webconcepts.info/concepts/http-header/

- EPR (W3C TR http://www.w3.org/TR/epr) - Servers may request the protections outlined by Entry Point Regulation (EPR) by sending an EPR HTTP response header field along with a response. - http://webconcepts.info/concepts/http-header/

- ETag (RFC 7232) - The "ETag" header field in a response provides the current entity-tag for the selected representation, as determined at the conclusion of handling the request. An entity-tag is an opaque validator for differentiating between multiple representations of the same resource, regardless of whether those multiple representations are due to resource state changes over time, content negotiation resulting in multiple representations being valid at the same time, or both. - http://webconcepts.info/concepts/http-header/

- Expect (RFC 7231) - The "Expect" header field in a request indicates a certain set of behaviors (expectations) that need to be supported by the server in order to properly handle this request. - http://webconcepts.info/concepts/http-header/

- Expect-CT (Internet Draft ietf-httpbis-expect-ct) - The "Expect-CT" header field is a new response header defined in this specification. It is used by a server to indicate that UAs should evaluate connections to the host emitting the header for CT compliance. - http://webconcepts.info/concepts/http-header/

- Expires (RFC 7234) - The "Expires" header field gives the date/time after which the response is considered stale. The presence of an Expires field does not imply that the original resource will change or cease to exist at, before, or after that time. - http://webconcepts.info/concepts/http-header/

- Ext (RFC 2774) - The Ext header field is used to indicate that all end-to-end mandatory extension declarations in the request were fulfilled. - http://webconcepts.info/concepts/http-header/

- Forwarded (RFC 7239) - The "Forwarded" HTTP header field is an OPTIONAL header field that, when used, contains a list of parameter-identifier pairs that disclose information that is altered or lost when a proxy is involved in the path of the request. - http://webconcepts.info/concepts/http-header/

- From (RFC 7231) - The "From" header field contains an Internet email address for a human user who controls the requesting user agent. - http://webconcepts.info/concepts/http-header/

- GET-Location (Internet Draft reschke-http-get-location) - The GET-Location entity header identifies a substitute resource that can be used in subsequent requests for the same information, but using the GET method. - http://webconcepts.info/concepts/http-header/

- HTTP2-Settings (RFC 7540) - A request that upgrades from HTTP/1.1 to HTTP/2 MUST include exactly one "HTTP2-Settings" header field. The "HTTP2-Settings" header field is a connection-specific header field that includes parameters that govern the HTTP/2 connection, provided in anticipation of the server accepting the request to upgrade. - http://webconcepts.info/concepts/http-header/

- HTTPS (W3C TR http://www.w3.org/TR/upgrade-insecure-requests) - The HTTPS HTTP request header field sends a signal to the server expressing the client’s preference for an encrypted and authenticated response, and that it can successfully handle the upgrade-insecure-requests directive in order to make that preference as seamless as possible to provide. - http://webconcepts.info/concepts/http-header/

- Hobareg (RFC 7486) - The server MUST add a header field to the response message when the registration has succeeded in order to indicate the new state. The header to be used is "Hobareg", and the value when registration has succeeded is to be "regok". When registration is in an intermediate state (e.g., on an HTTP response for an interstitial page), the server MAY add this header with a value of "reginwork". - http://webconcepts.info/concepts/http-header/

- Host (RFC 7230) - The "Host" header field in a request provides the host and port information from the target URI, enabling the origin server to distinguish among resources while servicing requests for multiple host names on a single IP address. - http://webconcepts.info/concepts/http-header/

- IM (RFC 3229) - The IM response-header field is used to indicate the instance-manipulations, if any, that have been applied to the instance represented by the response. Typical instance manipulations include delta encoding and compression. - http://webconcepts.info/concepts/http-header/

- If (RFC 4918) - The If request header is intended to have similar functionality to the If-Match header defined in Section 14.24 of RFC 2616. However, the If header handles any state token as well as ETags. A typical example of a state token is a lock token, and lock tokens are the only state tokens defined in this specification. - http://webconcepts.info/concepts/http-header/

- If-Match (RFC 7232) - The "If-Match" header field makes the request method conditional on the recipient origin server either having at least one current representation of the target resource, when the field-value is "*", or having a current representation of the target resource that has an entity-tag matching a member of the list of entity-tags provided in the field-value. - http://webconcepts.info/concepts/http-header/

- If-Modified-Since (RFC 7232) - The "If-Modified-Since" header field makes a GET or HEAD request method conditional on the selected representation modification date being more recent than the date provided in the field-value. Transfer of the selected representation data is avoided if that data has not changed. - http://webconcepts.info/concepts/http-header/

- If-None-Match (RFC 7232) - The "If-None-Match" header field makes the request method conditional on a recipient cache or origin server either not having any current representation of the target resource, when the field-value is "*", or having a selected representation with an entity-tag that does not match any of those listed in the field-value. - http://webconcepts.info/concepts/http-header/

- If-Range (RFC 7233) - If a client has a partial copy of a representation and wishes to have an up-to-date copy of the entire representation, it could use the Range header field with a conditional GET (using either or both of If-Unmodified-Since and If-Match.) However, if the precondition fails because the representation has been modified, the client would then have to make a second request to obtain the entire current representation. The "If-Range" header field allows a client to "short-circuit" the second request. Informally, its meaning is: if the representation is unchanged, send me the part(s) that I am requesting in Range; otherwise, send me the entire representation. - http://webconcepts.info/concepts/http-header/

- If-Schedule-Tag-Match (RFC 6638) - The If-Schedule-Tag-Match request header field is used with a method to make it conditional. Clients can set this header to the value returned in the Schedule-Tag response header, or the CALDAV:schedule-tag property, of a scheduling object resource previously retrieved from the server to avoid overwriting "consequential" changes to the scheduling object resource. - http://webconcepts.info/concepts/http-header/

- If-Unmodified-Since (RFC 7232) - The "If-Unmodified-Since" header field makes the request method conditional on the selected representation last modification date being earlier than or equal to the date provided in the field-value. This field accomplishes the same purpose as If-Match for cases where the user agent does not have an entity-tag for the representation. - http://webconcepts.info/concepts/http-header/

- Key (Internet Draft ietf-httpbis-key) - The "Key" response header field describes the request attributes that the server has used to select the current representation. As such, its semantics are similar to the "Vary" response header field, but it allows more fine-grained description, using "key modifiers". - http://webconcepts.info/concepts/http-header/

- Label (RFC 3253) - For certain methods (e.g. GET, PROPFIND), if the request-URL identifies a version-controlled resource, a label can be specified in a Label request header to cause the method to be applied to the version selected by that label from the version history of that version-controlled resource. - http://webconcepts.info/concepts/http-header/

- Last-Event-ID (W3C TR http://www.w3.org/TR/eventsource) - The Last-Event-ID HTTP header specifies the value of the event source's last event ID string, encoded as UTF-8. - http://webconcepts.info/concepts/http-header/

- Last-Modified (RFC 7232) - The "Last-Modified" header field in a response provides a timestamp indicating the date and time at which the origin server believes the selected representation was last modified, as determined at the conclusion of handling the request. - http://webconcepts.info/concepts/http-header/

- Link (RFC 8288) - The Link header field provides a means for serialising one or more links into HTTP headers. - http://webconcepts.info/concepts/http-header/

- Link-Template (Internet Draft nottingham-link-template) - The Link-Template entity-header field provides a means for serialising one or more links into HTTP headers. It is semantically equivalent to the Link header field, except that it uses URI Templates to convey the structure of links. - http://webconcepts.info/concepts/http-header/

- Location (RFC 7231) - The "Location" header field is used in some responses to refer to a specific resource in relation to the response. The type of relationship is defined by the combination of request method and status code semantics. - http://webconcepts.info/concepts/http-header/

- Lock-Token (RFC 4918) - The Lock-Token request header is used with the UNLOCK method to identify the lock to be removed. - http://webconcepts.info/concepts/http-header/

- MIME-Version (RFC 7231) - HTTP is not a MIME-compliant protocol. However, messages can include a single MIME-Version header field to indicate what version of the MIME protocol was used to construct the message. Use of the MIME-Version header field indicates that the message is in full conformance with the MIME protocol (as defined in RFC 2045). Senders are responsible for ensuring full conformance (where possible) when exporting HTTP messages to strict MIME environments. - http://webconcepts.info/concepts/http-header/

- Man (RFC 2774) - A mandatory extension declaration indicates that the ultimate recipient MUST consult and adhere to the rules given by the extension when processing the message or reporting an error. - http://webconcepts.info/concepts/http-header/

- Max-Forwards (RFC 7231) - The "Max-Forwards" header field provides a mechanism with the TRACE and OPTIONS request methods to limit the number of times that the request is forwarded by proxies. - http://webconcepts.info/concepts/http-header/

- Memento-Datetime (RFC 7089) - The "Memento-Datetime" response header is used by a server to indicate that a response reflects a prior state of an Original Resource. Its value expresses the datetime of that state. - http://webconcepts.info/concepts/http-header/

- Negotiate (RFC 2295) - The Negotiate request header can contain directives for any content negotiation process initiated by the request. - http://webconcepts.info/concepts/http-header/

- Nice (Internet Draft thomson-http-nice) - The "Nice" header field indicates that a request is less important than a request that doesn't bear this header. - http://webconcepts.info/concepts/http-header/

- OData-EntityId (OASIS Standard odata-v4.0-part1-protocol) - A response to a create or upsert operation that returns 204 No Content MUST include an OData-EntityId response header. The value of the header is the entity-id of the entity that was acted on by the request. - http://webconcepts.info/concepts/http-header/

- OData-Isolation (OASIS Standard odata-v4.0-part1-protocol) - The OData-Isolation header specifies the isolation of the current request from external changes. The only supported value for this header is snapshot. - http://webconcepts.info/concepts/http-header/

- OData-MaxVersion (OASIS Standard odata-v4.0-part1-protocol) - Clients SHOULD specify an OData-MaxVersion request header. If specified the service MUST generate a response with an OData-Version less than or equal to the specified OData-MaxVersion. - http://webconcepts.info/concepts/http-header/

- Opt (RFC 2774) - An optional extension declaration indicates that the ultimate recipient of the extension MAY consult and adhere to the rules given by the extension when processing the message, or ignore the extension declaration completely. An agent may not be able to distinguish whether the ultimate recipient does not understand an extension referred to by an optional extension or simply ignores the extension declaration. - http://webconcepts.info/concepts/http-header/

- Optional-WWW-Authenticate (RFC 8053) - The Optional-WWW-Authenticate header enables a non-mandatory authentication, which is not possible under the current HTTP authentication mechanism. - http://webconcepts.info/concepts/http-header/

- Ordering-Type (RFC 3648) - When a collection is created, the client MAY request that it be ordered and specify the semantics of the ordering by using the new Ordering-Type header with a MKCOL request. For collections that are ordered, the client SHOULD identify the semantics of the ordering with a URI in the Ordering-Type header, although the client MAY simply set the header value to DAV:custom to indicate that the collection is ordered but the semantics of the ordering are not being advertised. - http://webconcepts.info/concepts/http-header/

- Origin (W3C TR http://www.w3.org/TR/cors) - The Origin header indicates where the cross-origin request or preflight request originates from. - http://webconcepts.info/concepts/http-header/

- Origin-Cookie (Internet Draft west-origin-cookies) - The user agent includes stored cookies whose "origin-flag" is set in the "Origin-Cookie" request header. When the user agent generates an HTTP request, it MUST NOT attach more than one "Origin-Cookie" header field. - http://webconcepts.info/concepts/http-header/

- Overwrite (RFC 4918) - The Overwrite request header specifies whether the server should overwrite a resource mapped to the destination URL during a COPY or MOVE. - http://webconcepts.info/concepts/http-header/

- P3P (W3C TR http://www.w3.org/TR/P3P) - Any document retrieved by HTTP may point to a policy reference file through the use of a new response header, the P3P header. If a site is using P3P headers, it SHOULD include this on responses for all appropriate request methods, including HEAD and OPTIONS requests. The P3P header gives one or more comma-separated directives. - http://webconcepts.info/concepts/http-header/

- PEP (W3C TR http://www.w3.org/TR/WD-http-pep) - PEP end-to-end declarations must be transmitted to the ultimate recipient of the declaration. The PEP header field is an end-to-end header field. - http://webconcepts.info/concepts/http-header/

- PEP-Info (W3C TR http://www.w3.org/TR/WD-http-pep) - PEP end-to-end policies MUST be transmitted to the ultimate recipient of a message. - http://webconcepts.info/concepts/http-header/

- POE (Internet Draft nottingham-http-poe) - The POE HTTP header is a request-header field whose field-value indicates the version of POE that a client supports. - http://webconcepts.info/concepts/http-header/

- POE-Links (Internet Draft nottingham-http-poe) - The POE-Links HTTP header is an entity-header field whose field-value is a comma-separated list of quoted URI-references (without fragment identifiers) that the origin server asserts to be POE resources. The contents of the POE-Links response header SHOULD correspond to links found in the content of the response body. - http://webconcepts.info/concepts/http-header/

- Position (RFC 3648) - When a new member is added to a collection with a client-maintained ordering (for example, with PUT, COPY, or MKCOL), its position in the ordering can be set with the new Position header. The Position header allows the client to specify that an internal member URI should be first in the collection's ordering, last in the collection's ordering, immediately before some other internal member URI in the collection's ordering, or immediately after some other internal member URI in the collection's ordering. - http://webconcepts.info/concepts/http-header/

- Pragma (RFC 7234) - The "Pragma" header field allows backwards compatibility with HTTP/1.0 caches, so that clients can specify a "no-cache" request that they will understand (as Cache-Control was not defined until HTTP/1.1). When the Cache-Control header field is also present and understood in a request, Pragma is ignored. - http://webconcepts.info/concepts/http-header/

- Prefer (RFC 7240) - The Prefer request header field is used to indicate that particular server behaviors are preferred by the client, but not required for successful completion of the request. Prefer is similar in nature to the Expect header field with the exception that servers are allowed to ignore stated preferences. - http://webconcepts.info/concepts/http-header/

- Preference-Applied (RFC 7240) - The Preference-Applied response header MAY be included within a response message as an indication as to which Prefer tokens were honored by the server and applied to the processing of a request. - http://webconcepts.info/concepts/http-header/

- Public (RFC 2068) - The Public response-header field lists the set of methods supported by the server. The purpose of this field is strictly to inform the recipient of the capabilities of the server regarding unusual methods. The methods listed may or may not be applicable to the Request-URI; the Allow header field MAY be used to indicate methods allowed for a particular URI. - http://webconcepts.info/concepts/http-header/

- Range (RFC 7233) - The "Range" header field on a GET request modifies the method semantics to request transfer of only one or more subranges of the selected representation data, rather than the entire selected representation data. - http://webconcepts.info/concepts/http-header/

- Redirect-Ref (RFC 4437) - The Redirect-Ref header is used in all 3xx responses from redirect reference resources. The value is the link target as specified during redirect reference resource creation. - http://webconcepts.info/concepts/http-header/

- Referer (RFC 7231) - The "Referer" header field allows the user agent to specify a URI reference for the resource from which the target URI was obtained (i.e., the "referrer", though the field name is misspelled). - http://webconcepts.info/concepts/http-header/

- Report-To (W3C TR http://www.w3.org/TR/reporting-1) - The Report-To HTTP response header field instructs the user agent to store reporting endpoints for an origin. - http://webconcepts.info/concepts/http-header/

- Retry-After (RFC 7231) - Servers send the "Retry-After" header field to indicate how long the user agent ought to wait before making a follow-up request. When sent with a 503 (Service Unavailable) response, Retry-After indicates how long the service is expected to be unavailable to the client. When sent with any 3xx (Redirection) response, Retry-After indicates the minimum time that the user agent is asked to wait before issuing the redirected request. - http://webconcepts.info/concepts/http-header/

- SOAPAction (W3C TR http://www.w3.org/TR/SOAP) - The SOAPAction HTTP request header field can be used to indicate the intent of the SOAP HTTP request. The value is a URI identifying the intent. SOAP places no restrictions on the format or specificity of the URI or that it is resolvable. An HTTP client MUST use this header field when issuing a SOAP HTTP Request. - http://webconcepts.info/concepts/http-header/

- Safe (RFC 2310) - The Safe response header field is used by origin servers to indicate whether repeating the received HTTP request is safe in the sense of Section 9.1.1 (Safe Methods) of the HTTP/1.1 specification. For the purpose of this specification, a HTTP request is considered to be a repetition of a previous request if both requests are issued by the same user agent, and apply to the same resource, and have the same request method, and both have no request body, or both have request bodies which are byte-wise identical after decoding of any content and transfer codings. - http://webconcepts.info/concepts/http-header/

- Save-Data (Internet Draft ietf-httpbis-client-hints) - The "Save-Data" header field is a token that, in requests, indicates client's preference for reduced data usage, due to high transfer costs, slow connection speeds, or other reasons. - http://webconcepts.info/concepts/http-header/

- Schedule-Reply (RFC 6638) - The Schedule-Reply request header is used by a client to indicate to a server whether or not a scheduling operation ought to occur when an "Attendee" deletes a scheduling object resource. In particular, it controls whether a reply scheduling message is sent to the "Organizer" as a result of the removal. There are situations in which unsolicited scheduling messages need to be silently removed (or ignored) for security or privacy reasons. This request header allows the scheduling object resource to be removed if such a need arises. - http://webconcepts.info/concepts/http-header/

- Schedule-Tag (RFC 6638) - The Schedule-Tag response header provides the current value of the CALDAV:schedule-tag property value. - http://webconcepts.info/concepts/http-header/

- Sec-COWL (W3C TR http://www.w3.org/TR/COWL) - The Sec-COWL HTTP request and response headers are used by user agents and servers to convey label metadata to servers and user agents, respectively. - http://webconcepts.info/concepts/http-header/

- Sec-WebSocket-Accept (RFC 6455) - The Sec-WebSocket-Accept header field is used in the WebSocket opening handshake. It is sent from the server to the client to confirm that the server is willing to initiate the WebSocket connection. - http://webconcepts.info/concepts/http-header/

- Sec-WebSocket-Extensions (RFC 6455) - The Sec-WebSocket-Extensions header field is used in the WebSocket opening handshake. It is initially sent from the client to the server, and then subsequently sent from the server to the client, to agree on a set of protocol-level extensions to use for the duration of the connection. - http://webconcepts.info/concepts/http-header/

- Sec-WebSocket-Key (RFC 6455) - The Sec-WebSocket-Key header field is used in the WebSocket opening handshake. It is sent from the client to the server to provide part of the information used by the server to prove that it received a valid WebSocket opening handshake. - http://webconcepts.info/concepts/http-header/

- Sec-WebSocket-Protocol (RFC 6455) - The Sec-WebSocket-Protocol header field is used in the WebSocket opening handshake. It is sent from the client to the server and back from the server to the client to confirm the subprotocol of the connection. This enables scripts to both select a subprotocol and be sure that the server agreed to serve that subprotocol. - http://webconcepts.info/concepts/http-header/

- Sec-WebSocket-Version (RFC 6455) - The Sec-WebSocket-Version header field is used in the WebSocket opening handshake. It is sent from the client to the server to indicate the protocol version of the connection. This enables servers to correctly interpret the opening handshake and subsequent data being sent from the data, and close the connection if the server cannot interpret that data in a safe manner. The Sec-WebSocket-Version header field is also sent from the server to the client on WebSocket handshake error, when the version received from the client does not match a version understood by the server. In such a case, the header field includes the protocol version(s) supported by the server. - http://webconcepts.info/concepts/http-header/

- Security-Scheme (RFC 2660) - All S-HTTP compliant agents must generate the Security-Scheme header in the headers of all HTTP messages they generate. This header permits other agents to detect that they are communicating with an S-HTTP compliant agent and generate the appropriate cryptographic options headers. - http://webconcepts.info/concepts/http-header/

- Server (RFC 7231) - The "Server" header field contains information about the software used by the origin server to handle the request, which is often used by clients to help identify the scope of reported interoperability problems, to work around or tailor requests to avoid particular server limitations, and for analytics regarding server or operating system use. - http://webconcepts.info/concepts/http-header/

- Server-Timing (W3C TR http://www.w3.org/TR/server-timing) - The Server-Timing header field is used to communicate one or more metrics and descriptions for the given request-response cycle. - http://webconcepts.info/concepts/http-header/

- Service-Worker (W3C TR http://www.w3.org/TR/service-workers-1) - An HTTP request to fetch a service worker's script resource will include the Service-Worker header. It indicates that this request is a service worker's script resource request. - http://webconcepts.info/concepts/http-header/

- Service-Worker-Allowed (W3C TR http://www.w3.org/TR/service-workers-1) - An HTTP response to a service worker's script resource request can include the Service-Worker-Allowed header. It indicates that the user agent will override the path restriction, which limits the maximum allowed scope url that the script can control, to the given value. - http://webconcepts.info/concepts/http-header/

- Set-Cookie (Internet Draft ietf-httpbis-rfc6265b is RFC 6265) - The Set-Cookie HTTP response header is used to send cookies from the server to the user agent.The Set-Cookie HTTP response header is used to send cookies from the server to the user agent. - http://webconcepts.info/concepts/http-header/

- Set-Cookie2 (RFC 2965) - The origin server initiates a session, if it so desires. To do so, it returns an extra response header to the client, Set-Cookie2. - http://webconcepts.info/concepts/http-header/

- Signature (Internet Draft cavage-http-signatures) - The "signature" HTTP Header is based on the model that the sender must authenticate itself with a digital signature produced by either a private asymmetric key (e.g., RSA) or a shared symmetric key (e.g., HMAC). The scheme is parameterized enough such that it is not bound to any particular key type or signing algorithm. However, it does explicitly assume that senders can send an HTTP 'Date' header. - http://webconcepts.info/concepts/http-header/

- Slug (RFC 5023) - Slug is an HTTP entity-header whose presence in a POST to a Collection constitutes a request by the client to use the header's value as part of any URIs that would normally be used to retrieve the to-be-created Entry or Media Resources. - http://webconcepts.info/concepts/http-header/

- Status-URI (RFC 2518) - The Status-URI response header may be used with the 102 (Processing) status code to inform the client as to the status of a method. - http://webconcepts.info/concepts/http-header/

- Strict-Transport-Security (RFC 6797) - The Strict-Transport-Security HTTP response header field (STS header field) indicates to a UA that it MUST enforce the HSTS Policy in regards to the host emitting the response message containing this header field. - http://webconcepts.info/concepts/http-header/

- SubOK (Internet Draft mogul-http-dupsup) - The SubOK request header field is used to provide directives from an end-client to a proxy cache regarding the possible substitution of an instance body from a cached response for one resource instance for the instance body of the resource instance specified by the client's request. - http://webconcepts.info/concepts/http-header/

- Subst (Internet Draft mogul-http-dupsup) - The Subst response-header field MUST be used by a proxy to supply the URI of the original source of an entity-body, if the source is different from the client's Request-URI, and if the client's request included the "inform" directive in a SubOK request header field. - http://webconcepts.info/concepts/http-header/

- Sunset (Internet Draft wilde-sunset-header) - The Sunset HTTP response header field allows a server to communicate the fact that a resource is expected to become unresponsive at a specific point in time. It provides information for clients which they can use to control their usage of the resource. The Sunset header contains a single timestamp which advertises the point in time when the resource is expected to become unresponsive. - http://webconcepts.info/concepts/http-header/

- Surrogate-Capability (W3C TR http://www.w3.org/TR/edge-arch) - The Surrogate-Capabilities request header allows surrogates to advertise their capabilities with capability tokens. Capability tokens indicate sets of operations (e.g., caching, processing) that a surrogate is willing to perform. They follow the form of product tokens in HTTP. - http://webconcepts.info/concepts/http-header/

- Surrogate-Control (W3C TR http://www.w3.org/TR/edge-arch) - The Surrogate-Control response header allows origin servers to dictate how surrogates should handle response entities, with control directives. Currently defined directives control processing and cache behavior. - http://webconcepts.info/concepts/http-header/

- TCN (RFC 2295) - The TCN response header is used by a server to signal that the resource is transparently negotiated. - http://webconcepts.info/concepts/http-header/

- TE (RFC 7230) - The "TE" header field in a request indicates what transfer codings, besides chunked, the client is willing to accept in response, and whether or not the client is willing to accept trailer fields in a chunked transfer coding. - http://webconcepts.info/concepts/http-header/

- TTL (RFC 8030) - An application server MUST include the TTL (Time-To-Live) header field in its request for push message delivery. The TTL header field contains a value in seconds that suggests how long a push message is retained by the push service. - http://webconcepts.info/concepts/http-header/

- Timeout (RFC 4918) - Clients MAY include Timeout request headers in their LOCK requests. However, the server is not required to honor or even consider these requests. - http://webconcepts.info/concepts/http-header/

- Title (RFC 4229) - The title of the document. Not part of the document. Isomorphic with the element in HTML. - http://webconcepts.info/concepts/http-header/

- Topic (RFC 8030) - A push message topic is a string carried in a Topic header field. A topic is used to correlate push messages sent to the same subscription and does not convey any other semantics. - http://webconcepts.info/concepts/http-header/

- Trailer (RFC 7230) - When a message includes a message body encoded with the chunked transfer coding and the sender desires to send metadata in the form of trailer fields at the end of the message, the sender SHOULD generate a Trailer header field before the message body to indicate which fields will be present in the trailers. - http://webconcepts.info/concepts/http-header/

- Transfer-Encoding (RFC 7230) - The Transfer-Encoding header field lists the transfer coding names corresponding to the sequence of transfer codings that have been (or will be) applied to the payload body in order to form the message body. - http://webconcepts.info/concepts/http-header/

- Tunnel-Protocol (Internet Draft ietf-httpbis-tunnel-protocol) - Clients include the Tunnel-Protocol header field in an HTTP CONNECT request to indicate the application layer protocol that will be used within the tunnel, or the set of protocols that might be used within the tunnel. - http://webconcepts.info/concepts/http-header/

- URI (RFC 2068) - The URI header field has, in past versions of this specification, been used as a combination of the existing Location, Content-Location, and Vary header fields as well as the future Alternates field. Its primary purpose has been to include a list of additional URIs for the resource, including names and mirror locations. However, it has become clear that the combination of many different functions within this single field has been a barrier to consistently and correctly implementing any of those functions. Furthermore, we believe that the identification of names and mirror locations would be better performed via the Link header field. The URI header field is therefore deprecated in favor of those other fields. - http://webconcepts.info/concepts/http-header/

- Upgrade (RFC 7230) - The "Upgrade" header field is intended to provide a simple mechanism for transitioning from HTTP/1.1 to some other protocol on the same connection. A client MAY send a list of protocols in the Upgrade header field of a request to invite the server to switch to one or more of those protocols, in order of descending preference, before sending the final response. - http://webconcepts.info/concepts/http-header/

- Urgency (RFC 8030) - An application server MAY include an Urgency header field in its request for push message delivery. This header field indicates the message urgency. The push service MUST NOT forward the Urgency header field to the user agent. A push message without the Urgency header field defaults to a value of "normal". - http://webconcepts.info/concepts/http-header/

- User-Agent (RFC 7231) - The "User-Agent" header field contains information about the user agent originating the request, which is often used by servers to help identify the scope of reported interoperability problems, to work around or tailor responses to avoid particular user agent limitations, and for analytics regarding browser or operating system use. - http://webconcepts.info/concepts/http-header/

- Variant-Vary (RFC 2295) - The Variant-Vary response header can be used in a choice response to record any vary information which applies to the variant data (the entity body combined with some of the entity headers) contained in the response, rather than to the response as a whole. - http://webconcepts.info/concepts/http-header/

- Variants (Internet Draft draft-nottingham-variants) - The Variants HTTP response header field is used to indicate what other representations are available for a given resource at the time that the response is produced. - http://webconcepts.info/concepts/http-header/

- Vary (RFC 7231) - The "Vary" header field in a response describes what parts of a request message, aside from the method, Host header field, and request target, might influence the origin server's process for selecting and representing this response. The value consists of either a single asterisk ("*") or a list of header field names (case-insensitive). - http://webconcepts.info/concepts/http-header/

- Via (RFC 7230) - The "Via" header field indicates the presence of intermediate protocols and recipients between the user agent and the server (on requests) or between the origin server and the client (on responses), similar to the "Received" header field in email (Section 3.6.7 of RFC 5322). Via can be used for tracking message forwards, avoiding request loops, and identifying the protocol capabilities of senders along the request/response chain. - http://webconcepts.info/concepts/http-header/

- Viewport-Width (Internet Draft ietf-httpbis-client-hints) - The "Viewport-Width" header field is a number that, in requests, indicates the layout viewport width in CSS px. - http://webconcepts.info/concepts/http-header/

- WWW-Authenticate (RFC 7616 RFC 7235) - If a server receives a request for an access-protected object, and an acceptable Authorization header is not sent, the server responds with a "401 Unauthorized" status code, and a WWW-Authenticate header as per the framework defined above.The "WWW-Authenticate" header field consists of at least one challenge that indicates the authentication scheme(s) and parameters applicable to the effective request URI. It MUST be included in 401 (Unauthorized) response messages and MAY be included in other response messages to indicate that supplying credentials (or different credentials) might affect the response. - http://webconcepts.info/concepts/http-header/

- Want-Digest (RFC 3230) - The Want-Digest message header field indicates the sender's desire to receive an instance digest on messages associated with the Request-URI. - http://webconcepts.info/concepts/http-header/

- Warning (RFC 7234) - The "Warning" header field is used to carry additional information about the status or transformation of a message that might not be reflected in the status code. This information is typically used to warn about possible incorrectness introduced by caching operations or transformations applied to the payload of the message. - http://webconcepts.info/concepts/http-header/

- Width (Internet Draft ietf-httpbis-client-hints) - The "Width" header field is a number that, in requests, indicates the resource width in physical px (i.e. intrinsic size of an image). - http://webconcepts.info/concepts/http-header/

- X-Frame-Options (RFC 7034) - The X-Frame-Options HTTP header field indicates a policy that specifies whether the browser should render the transmitted resource within a or an . Servers can declare this policy in the header of their HTTP responses to prevent clickjacking attacks, which ensures that their content is not embedded into other pages or frames. - http://webconcepts.info/concepts/http-header/

## HTTP Response
Planning for what each API response will provide, embracing common messages, schema, and thinking constantly about what services should be delivering.

- Body - The response body, which might include hypermedia, and other media types, providing a structure response to each API request.

- CORS - Considering the need and presence of mechanisms to enable client-side cross-origin requests, which might limit responses made from alternate domains.

- JSONP - Using JSONP to enable sharing of data bypassing same-origin policy, and make API responses available in client side applications.

- Schema - The JSON Schema, MSON, or other machine readable approach to defining the underlying data model of the API response.

- Sorting - How to sort a collection of resources, allowing for the response details to be delivered in a specific order.

- Pagination - Considering how large volumes of data will be delivered, and consumers will be requesting different pages.

- Links - Links to related API paths, other URLs for putting to use as part of the API response, setting the stage for what can come next.

## HTTP Status Codes
Providing lists of HTTP status codes that should be used across services, supporting the web, and providing consistent responses that other systems and applications will be able to consistently understand the response being returned.

- 100 (RFC 7231) - The 100 (Continue) status code indicates that the initial part of a request has been received and has not yet been rejected by the server. The server intends to send a final response after the request has been fully received and acted upon. - http://webconcepts.info/concepts/http-status-code/

- 101 (RFC 7231) - The 101 (Switching Protocols) status code indicates that the server understands and is willing to comply with the client's request, via the Upgrade header field, for a change in the application protocol being used on this connection. The server MUST generate an Upgrade header field in the response that indicates which protocol(s) will be switched to immediately after the empty line that terminates the 101 response. - http://webconcepts.info/concepts/http-status-code/

- 102 (RFC 2518) - The 102 (Processing) status code is an interim response used to inform the client that the server has accepted the complete request, but has not yet completed it. This status code SHOULD only be sent when the server has a reasonable expectation that the request will take significant time to complete. As guidance, if a method is taking longer than 20 seconds (a reasonable, but arbitrary value) to process the server SHOULD return a 102 (Processing) response. The server MUST send a final response after the request has been completed. - http://webconcepts.info/concepts/http-status-code/

- 103 (RFC 8297) - The 103 (Early Hints) status code indicates the client that the server is likely to send a final request with the headers included in the informational response. - http://webconcepts.info/concepts/http-status-code/

- 200 (RFC 7231) - The 200 (OK) status code indicates that the request has succeeded. The payload sent in a 200 response depends on the request method. - http://webconcepts.info/concepts/http-status-code/

- 201 (RFC 7231) - The 201 (Created) status code indicates that the request has been fulfilled and has resulted in one or more new resources being created. The primary resource created by the request is identified by either a Location header field in the response or, if no Location field is received, by the effective request URI. - http://webconcepts.info/concepts/http-status-code/

- 202 (RFC 7231) - The 202 (Accepted) status code indicates that the request has been accepted for processing, but the processing has not been completed. The request might or might not eventually be acted upon, as it might be disallowed when processing actually takes place. There is no facility in HTTP for re-sending a status code from an asynchronous operation. - http://webconcepts.info/concepts/http-status-code/

- 203 (RFC 7231) - The 203 (Non-Authoritative Information) status code indicates that the request was successful but the enclosed payload has been modified from that of the origin server's 200 (OK) response by a transforming proxy. - http://webconcepts.info/concepts/http-status-code/

- 204 (RFC 7231) - The 204 (No Content) status code indicates that the server has successfully fulfilled the request and that there is no additional content to send in the response payload body. Metadata in the response header fields refer to the target resource and its selected representation after the requested action was applied. - http://webconcepts.info/concepts/http-status-code/

- 205 (RFC 7231) - The 205 (Reset Content) status code indicates that the server has fulfilled the request and desires that the user agent reset the "document view", which caused the request to be sent, to its original state as received from the origin server. - http://webconcepts.info/concepts/http-status-code/

- 206 (RFC 7233) - The 206 (Partial Content) status code indicates that the server is successfully fulfilling a range request for the target resource by transferring one or more parts of the selected representation that correspond to the satisfiable ranges found in the request's Range header field. - http://webconcepts.info/concepts/http-status-code/

- 207 (RFC 4918) - The 207 (Multi-Status) status code provides status for multiple independent operations. - http://webconcepts.info/concepts/http-status-code/

- 208 (RFC 5842) - The 208 (Already Reported) status code can be used inside a DAV: propstat response element to avoid enumerating the internal members of multiple bindings to the same collection repeatedly. For each binding to a collection inside the request's scope, only one will be reported with a 200 status, while subsequent DAV:response elements for all other bindings will use the 208 status, and no DAV:response elements for their descendants are included. - http://webconcepts.info/concepts/http-status-code/

- 226 (RFC 3229) - The server has fulfilled a GET request for the resource, and the response is a representation of the result of one or more instance-manipulations applied to the current instance. The actual current instance might not be available except by combining this response with other previous or future responses, as appropriate for the specific instance-manipulation(s). - http://webconcepts.info/concepts/http-status-code/

- 300 (RFC 7231) - The 300 (Multiple Choices) status code indicates that the target resource has more than one representation, each with its own more specific identifier, and information about the alternatives is being provided so that the user (or user agent) can select a preferred representation by redirecting its request to one or more of those identifiers. In other words, the server desires that the user agent engage in reactive negotiation to select the most appropriate representation(s) for its needs. - http://webconcepts.info/concepts/http-status-code/

- 301 (RFC 7231) - The 301 (Moved Permanently) status code indicates that the target resource has been assigned a new permanent URI and any future references to this resource ought to use one of the enclosed URIs. Clients with link-editing capabilities ought to automatically re-link references to the effective request URI to one or more of the new references sent by the server, where possible. - http://webconcepts.info/concepts/http-status-code/

- 302 (RFC 7231) - The 302 (Found) status code indicates that the target resource resides temporarily under a different URI. Since the redirection might be altered on occasion, the client ought to continue to use the effective request URI for future requests. - http://webconcepts.info/concepts/http-status-code/

- 303 (RFC 7231) - The 303 (See Other) status code indicates that the server is redirecting the user agent to a different resource, as indicated by a URI in the Location header field, which is intended to provide an indirect response to the original request. A user agent can perform a retrieval request targeting that URI (a GET or HEAD request if using HTTP), which might also be redirected, and present the eventual result as an answer to the original request. Note that the new URI in the Location header field is not considered equivalent to the effective request URI. - http://webconcepts.info/concepts/http-status-code/

- 304 (RFC 7232) - The 304 (Not Modified) status code indicates that a conditional GET or HEAD request has been received and would have resulted in a 200 (OK) response if it were not for the fact that the condition evaluated to false. In other words, there is no need for the server to transfer a representation of the target resource because the request indicates that the client, which made the request conditional, already has a valid representation; the server is therefore redirecting the client to make use of that stored representation as if it were the payload of a 200 (OK) response. - http://webconcepts.info/concepts/http-status-code/

- 305 (RFC 7231) - The 305 (Use Proxy) status code was defined in a previous version of HTTP/1.1 and is now deprecated. - http://webconcepts.info/concepts/http-status-code/

- 306 (RFC 7231) - The 306 status code was defined in a previous version of HTTP/1.1, is no longer used, and the code is reserved. - http://webconcepts.info/concepts/http-status-code/

- 307 (RFC 7231) - The 307 (Temporary Redirect) status code indicates that the target resource resides temporarily under a different URI and the user agent MUST NOT change the request method if it performs an automatic redirection to that URI. Since the redirection can change over time, the client ought to continue using the original effective request URI for future requests. - http://webconcepts.info/concepts/http-status-code/

- 308 (RFC 7538) - The 308 (Permanent Redirect) status code indicates that the target resource has been assigned a new permanent URI and any future references to this resource ought to use one of the enclosed URIs. - http://webconcepts.info/concepts/http-status-code/

- 400 (RFC 7231) - The 400 (Bad Request) status code indicates that the server cannot or will not process the request due to something that is perceived to be a client error (e.g., malformed request syntax, invalid request message framing, or deceptive request routing). - http://webconcepts.info/concepts/http-status-code/

- 401 (RFC 7235) - The 401 (Unauthorized) status code indicates that the request has not been applied because it lacks valid authentication credentials for the target resource. The server generating a 401 response MUST send a WWW-Authenticate header field (Section 4.1) containing at least one challenge applicable to the target resource. - http://webconcepts.info/concepts/http-status-code/

- 402 (RFC 7231) - The 402 (Payment Required) status code is reserved for future use. - http://webconcepts.info/concepts/http-status-code/

- 403 (RFC 7231) - The 403 (Forbidden) status code indicates that the server understood the request but refuses to authorize it. A server that wishes to make public why the request has been forbidden can describe that reason in the response payload (if any). - http://webconcepts.info/concepts/http-status-code/

- 404 (RFC 7231) - The 404 (Not Found) status code indicates that the origin server did not find a current representation for the target resource or is not willing to disclose that one exists. A 404 status code does not indicate whether this lack of representation is temporary or permanent; the 410 (Gone) status code is preferred over 404 if the origin server knows, presumably through some configurable means, that the condition is likely to be permanent. - http://webconcepts.info/concepts/http-status-code/

- 405 (RFC 7231) - The 405 (Method Not Allowed) status code indicates that the method received in the request-line is known by the origin server but not supported by the target resource. The origin server MUST generate an Allow header field in a 405 response containing a list of the target resource's currently supported methods. - http://webconcepts.info/concepts/http-status-code/

- 406 (RFC 7231) - The 406 (Not Acceptable) status code indicates that the target resource does not have a current representation that would be acceptable to the user agent, according to the proactive negotiation header fields received in the request, and the server is unwilling to supply a default representation. - http://webconcepts.info/concepts/http-status-code/

- 407 (RFC 7235) - The 407 (Proxy Authentication Required) status code is similar to 401 (Unauthorized), but it indicates that the client needs to authenticate itself in order to use a proxy. The proxy MUST send a Proxy-Authenticate header field containing a challenge applicable to that proxy for the target resource. The client MAY repeat the request with a new or replaced Proxy-Authorization header field. - http://webconcepts.info/concepts/http-status-code/

- 408 (RFC 7231) - The 408 (Request Timeout) status code indicates that the server did not receive a complete request message within the time that it was prepared to wait. A server SHOULD send the "close" connection option in the response, since 408 implies that the server has decided to close the connection rather than continue waiting. If the client has an outstanding request in transit, the client MAY repeat that request on a new connection. - http://webconcepts.info/concepts/http-status-code/

- 409 (RFC 7231) - The 409 (Conflict) status code indicates that the request could not be completed due to a conflict with the current state of the target resource. This code is used in situations where the user might be able to resolve the conflict and resubmit the request. The server SHOULD generate a payload that includes enough information for a user to recognize the source of the conflict. - http://webconcepts.info/concepts/http-status-code/

- 410 (RFC 7231) - The 410 (Gone) status code indicates that access to the target resource is no longer available at the origin server and that this condition is likely to be permanent. If the origin server does not know, or has no facility to determine, whether or not the condition is permanent, the status code 404 (Not Found) ought to be used instead. - http://webconcepts.info/concepts/http-status-code/

- 411 (RFC 7231) - The 411 (Length Required) status code indicates that the server refuses to accept the request without a defined Content-Length. The client MAY repeat the request if it adds a valid Content-Length header field containing the length of the message body in the request message. - http://webconcepts.info/concepts/http-status-code/

- 412 (RFC 7232) - The 412 (Precondition Failed) status code indicates that one or more conditions given in the request header fields evaluated to false when tested on the server. This response code allows the client to place preconditions on the current resource state (its current representations and metadata) and, thus, prevent the request method from being applied if the target resource is in an unexpected state. - http://webconcepts.info/concepts/http-status-code/

- 413 (RFC 7231) - The 413 (Payload Too Large) status code indicates that the server is refusing to process a request because the request payload is larger than the server is willing or able to process. The server MAY close the connection to prevent the client from continuing the request. - http://webconcepts.info/concepts/http-status-code/

- 414 (RFC 7231) - The 414 (URI Too Long) status code indicates that the server is refusing to service the request because the request-target is longer than the server is willing to interpret. - http://webconcepts.info/concepts/http-status-code/

- 415 (RFC 7231) - The 415 (Unsupported Media Type) status code indicates that the origin server is refusing to service the request because the payload is in a format not supported by this method on the target resource. The format problem might be due to the request's indicated Content-Type or Content-Encoding, or as a result of inspecting the data directly. - http://webconcepts.info/concepts/http-status-code/

- 416 (RFC 7233) - The 416 (Range Not Satisfiable) status code indicates that none of the ranges in the request's Range header field (Section 3.1) overlap the current extent of the selected resource or that the set of ranges requested has been rejected due to invalid ranges or an excessive request of small or overlapping ranges. - http://webconcepts.info/concepts/http-status-code/

- 417 (RFC 7231) - The 417 (Expectation Failed) status code indicates that the expectation given in the request's Expect header field could not be met by at least one of the inbound servers. - http://webconcepts.info/concepts/http-status-code/

- 418 (RFC 2324) - Any attempt to brew coffee with a teapot should result in the error code "418 I'm a teapot". The resulting entity body MAY be short and stout. - http://webconcepts.info/concepts/http-status-code/

- 421 (RFC 7540) - The 421 (Misdirected Request) status code indicates that the request was directed at a server that is not able to produce a response. This can be sent by a server that is not configured to produce responses for the combination of scheme and authority that are included in the request URI. - http://webconcepts.info/concepts/http-status-code/

- 422 (RFC 4918) - The 422 (Unprocessable Entity) status code means the server understands the content type of the request entity (hence a 415 (Unsupported Media Type) status code is inappropriate), and the syntax of the request entity is correct (thus a 400 (Bad Request) status code is inappropriate) but was unable to process the contained instructions. For example, this error condition may occur if an XML request body contains well-formed (i.e., syntactically correct), but semantically erroneous, XML instructions. - http://webconcepts.info/concepts/http-status-code/

- 423 (RFC 4918) - The 423 (Locked) status code means the source or destination resource of a method is locked. This response SHOULD contain an appropriate precondition or postcondition code, such as 'lock-token-submitted' or 'no-conflicting-lock'. - http://webconcepts.info/concepts/http-status-code/

- 424 (RFC 4918) - The 424 (Failed Dependency) status code means that the method could not be performed on the resource because the requested action depended on another action and that action failed. For example, if a command in a PROPPATCH method fails, then, at minimum, the rest of the commands will also fail with 424 (Failed Dependency). - http://webconcepts.info/concepts/http-status-code/

- 426 (RFC 7231) - The 426 (Upgrade Required) status code indicates that the server refuses to perform the request using the current protocol but might be willing to do so after the client upgrades to a different protocol. The server MUST send an Upgrade header field in a 426 response to indicate the required protocol(s). - http://webconcepts.info/concepts/http-status-code/

- 428 (RFC 6585) - The 428 status code indicates that the origin server requires the request to be conditional. - http://webconcepts.info/concepts/http-status-code/

- 429 (RFC 6585) - The 429 status code indicates that the user has sent too many requests in a given amount of time ("rate limiting"). - http://webconcepts.info/concepts/http-status-code/

- 431 (RFC 6585) - The 431 status code indicates that the server is unwilling to process the request because its header fields are too large. The request MAY be resubmitted after reducing the size of the request header fields. - http://webconcepts.info/concepts/http-status-code/

- 451 (RFC 7725) - This status code indicates that the server is denying access to the resource as a consequence of a legal demand. The server in question might not be an origin server. This type of legal demand typically most directly affects the operations of ISPs and search engines. - http://webconcepts.info/concepts/http-status-code/

- 500 (RFC 7231) - The 500 (Internal Server Error) status code indicates that the server encountered an unexpected condition that prevented it from fulfilling the request. - http://webconcepts.info/concepts/http-status-code/

- 501 (RFC 7231) - The 501 (Not Implemented) status code indicates that the server does not support the functionality required to fulfill the request. This is the appropriate response when the server does not recognize the request method and is not capable of supporting it for any resource. - http://webconcepts.info/concepts/http-status-code/

- 502 (RFC 7231) - The 502 (Bad Gateway) status code indicates that the server, while acting as a gateway or proxy, received an invalid response from an inbound server it accessed while attempting to fulfill the request. - http://webconcepts.info/concepts/http-status-code/

- 503 (RFC 7231) - The 503 (Service Unavailable) status code indicates that the server is currently unable to handle the request due to a temporary overload or scheduled maintenance, which will likely be alleviated after some delay. The server MAY send a Retry-After header field to suggest an appropriate amount of time for the client to wait before retrying the request. - http://webconcepts.info/concepts/http-status-code/

- 504 (RFC 7231) - The 504 (Gateway Timeout) status code indicates that the server, while acting as a gateway or proxy, did not receive a timely response from an upstream server it needed to access in order to complete the request. - http://webconcepts.info/concepts/http-status-code/

- 505 (RFC 7231) - The 505 (HTTP Version Not Supported) status code indicates that the server does not support, or refuses to support, the major version of HTTP that was used in the request message. The server is indicating that it is unable or unwilling to complete the request using the same major version as the client, other than with this error message. The server SHOULD generate a representation for the 505 response that describes why that version is not supported and what other protocols are supported by that server. - http://webconcepts.info/concepts/http-status-code/

- 506 (RFC 2295) - The 506 status code indicates that the server has an internal configuration error: the chosen variant resource is configured to engage in transparent content negotiation itself, and is therefore not a proper end point in the negotiation process. - http://webconcepts.info/concepts/http-status-code/

- 507 (RFC 4918) - The 507 (Insufficient Storage) status code means the method could not be performed on the resource because the server is unable to store the representation needed to successfully complete the request. This condition is considered to be temporary. If the request that received this status code was the result of a user action, the request MUST NOT be repeated until it is requested by a separate user action. - http://webconcepts.info/concepts/http-status-code/

- 508 (RFC 5842) - The 508 (Loop Detected) status code indicates that the server terminated an operation because it encountered an infinite loop while processing a request with "Depth: infinity". This status indicates that the entire operation failed. - http://webconcepts.info/concepts/http-status-code/

- 510 (RFC 2774) - The policy for accessing the resource has not been met in the request. The server should send back all the information necessary for the client to issue an extended request. It is outside the scope of this specification to specify how the extensions inform the client. - http://webconcepts.info/concepts/http-status-code/

- 511 (RFC 6585) - The 511 status code indicates that the client needs to authenticate to gain network access. - http://webconcepts.info/concepts/http-status-code/

## Error handling
Going beyond the HTTP status code and making sure there is a plan for handling of error codes, and providing consistent behavior when it comes to things going wrong in delivering services.

- Error Codes - The visual code for the error beyond an individual status code.

- Errors Message - Providing a human readable error message for each type of error returned.

- Problem Details for HTTP APIs -  	This document defines a "problem detail" as a way to carry machine-readable details of errors in a HTTP response, to avoid the need to invent new error response formats for HTTP APIs. - http://webconcepts.info/specs/IETF/RFC/7807

# Caching
What caching exists at the server, CDN, and DNS layers for each service to provide a higher level of performance?

## HTTP Cache Directives
Providing a list of the HTTP Cache Directives that should be adopted as part of the caching of services being delivered.

- immutable (RFC 8246) - When present in an HTTP response, the immutable Cache-Control extension indicates that the origin server MUST NOT update the representation of that resource during the freshness lifetime of the response. - http://webconcepts.info/concepts/http-cache-directive/

- inv-maxage (Internet Draft nottingham-linked-cache-inv) - When present, the 'inv-maxage' cache-control extension indicates the number of seconds that caches who implement Linked Cache invalidation can consider responses fresh for, provided they are not invalidated. - http://webconcepts.info/concepts/http-cache-directive/

- max-age (RFC 7234) - The "max-age" request directive indicates that the client is unwilling to accept a response whose age is greater than the specified number of seconds. Unless the max-stale request directive is also present, the client is not willing to accept a stale response. The "max-age" response directive indicates that the response is to be considered stale after its age is greater than the specified number of seconds. - http://webconcepts.info/concepts/http-cache-directive/

- max-stale (RFC 7234) - The "max-stale" request directive indicates that the client is willing to accept a response that has exceeded its freshness lifetime. If max-stale is assigned a value, then the client is willing to accept a response that has exceeded its freshness lifetime by no more than the specified number of seconds. If no value is assigned to max-stale, then the client is willing to accept a stale response of any age. - http://webconcepts.info/concepts/http-cache-directive/

- min-fresh (RFC 7234) - The "min-fresh" request directive indicates that the client is willing to accept a response whose freshness lifetime is no less than its current age plus the specified time in seconds. That is, the client wants a response that will still be fresh for at least the specified number of seconds. - http://webconcepts.info/concepts/http-cache-directive/

- must-revalidate (RFC 7234) - The "must-revalidate" response directive indicates that once it has become stale, a cache MUST NOT use the response to satisfy subsequent requests without successful validation on the origin server. - http://webconcepts.info/concepts/http-cache-directive/

- no-cache (RFC 7234) - The "no-cache" request directive indicates that a cache MUST NOT use a stored response to satisfy the request without successful validation on the origin server. The "no-cache" response directive indicates that the response MUST NOT be used to satisfy a subsequent request without successful validation on the origin server. This allows an origin server to prevent a cache from using it to satisfy a request without contacting it, even by caches that have been configured to send stale responses. - http://webconcepts.info/concepts/http-cache-directive/

- no-store (RFC 7234) - The "no-store" directive indicates that a cache MUST NOT store any part of either this request or any response to it. This directive applies to both private and shared caches. "MUST NOT store" in this context means that the cache MUST NOT intentionally store the information in non-volatile storage, and MUST make a best-effort attempt to remove the information from volatile storage as promptly as possible after forwarding it. - http://webconcepts.info/concepts/http-cache-directive/

- no-transform (RFC 7234) - The "no-transform" directive indicates that an intermediary (whether or not it implements a cache) MUST NOT transform the payload. - http://webconcepts.info/concepts/http-cache-directive/

- only-if-cached (RFC 7234) - The "only-if-cached" request directive indicates that the client only wishes to obtain a stored response. If it receives this directive, a cache SHOULD either respond using a stored response that is consistent with the other constraints of the request, or respond with a 504 (Gateway Timeout) status code. If a group of caches is being operated as a unified system with good internal connectivity, a member cache MAY forward such a request within that group of caches. - http://webconcepts.info/concepts/http-cache-directive/

- private (RFC 7234) - The "private" response directive indicates that the response message is intended for a single user and MUST NOT be stored by a shared cache. A private cache MAY store the response and reuse it for later requests, even if the response would normally be non-cacheable. - http://webconcepts.info/concepts/http-cache-directive/

- proxy-revalidate (RFC 7234) - The "proxy-revalidate" response directive has the same meaning as the must-revalidate response directive, except that it does not apply to private caches. - http://webconcepts.info/concepts/http-cache-directive/

- public (RFC 7234) - The "public" response directive indicates that any cache MAY store the response, even if the response would normally be non-cacheable or cacheable only within a private cache. - http://webconcepts.info/concepts/http-cache-directive/

- s-maxage (RFC 7234) - The "s-maxage" response directive indicates that, in shared caches, the maximum age specified by this directive overrides the maximum age specified by either the max-age directive or the Expires header field. The s-maxage directive also implies the semantics of the proxy-revalidate response directive. - http://webconcepts.info/concepts/http-cache-directive/

- stale-if-error (RFC 5861) - The stale-if-error Cache-Control extension indicates that when an error is encountered, a cached stale response MAY be used to satisfy the request, regardless of other freshness information. - http://webconcepts.info/concepts/http-cache-directive/

- stale-while-revalidate (RFC 5861) - When present in an HTTP response, the stale-while-revalidate Cache-Control extension indicates that caches MAY serve the response in which it appears after it becomes stale, up to the indicated number of seconds. - http://webconcepts.info/concepts/http-cache-directive/

# Versioning
Plan for handling changes, and the inevitable evolution of each service, its definitions, and supporting code, establishing common and consistent approaches to approaching and communicating around the versioning of everything service related.

## Version Scope         
Putting together a plan for how the different scopes of versioning will be adopted, applied, and communicated across all layers, and stops along the API lifecycle.

- MAJOR version when you make incompatible API changes,

- MINOR version when you add functionality in a backwards-compatible manner,

- PATCH version when you make backwards-compatible bug fixes.         

## Version Concepts         
Effectively communicating the different concepts at play when it comes to versioning effectively, and making sure the versioning cycles have minimal impacts on clients, while still allowing the platform to move forward effectively.      

- Taking Away - You MUST NOT take anything away (related: Minimal Surface Principle , Robustness Principle)

- Processing - You MUST NOT change processing rules

- Optional - You MUST NOT make optional things required   

- New Features — New products or services, including new nodes, edges, and fields.

- All Changes — Changes to existing products or services (not including Deprecations).

- Deprecations — Existing products or services that are being removed.

- 90-Day Breaking Changes — Changes and deprecations that will take effect 90 days after the version release date.

- Robustness Principle - Anything you add MUST be optional   

# DNS
The domain addressing being used for routing, management and auditing of all service traffic, opening up this layer of the stack to be accessible as part of the API lifecycle.

## Domain(s)
Details regarding what domains are available for making available for service deployment, allowing for consistent, and meaningful addressing and deployment of services.

- Base URL for API - Providing a simple base URL for accessing API resources -- api.example.com is one common pattern.

- Base URL for Portal - Providing a simple base URL for accessing the developer portal -- developer.example.com is one common pattern.

## Addressing
Providing guidance and information regarding the addressing needed for delivering services consistently across an organization, while allowing them to be scalable and available in support of platform operations.

- Domain - Management of a single domain, and its administrative information.

- Record - Management of all types of records for a single domain.

- Zone - Manage the zones for any particular domain.

- Registration - Being able to register new domains, purchase, and manage ownership and registrar.

- Cache - Allow for domain level caching of all requests made through the domain.

- IP Address - Ability to manage IP address information, and perform lookups.

- Geo / Regions - Manage geographic specific details about domain operation.

- Forwarding - Enabling the ability to forward domains.

- Private - Allowing for the management of a private DNS deployment.

## Notifications
Providing a notification and messaging layer for the DNS involved with delivering services efficiently and reliably to users, making sure platform operators are aware of all activity and events.

- Webhooks - Providing notifications via webhooks when it comes to DNS events.

- Email - Provide notifications about DNS layer via emails.

- SMS - Provide notifications about DNS layer via SMS.

## Security
Considering the security implications present at the DNS layer, and making sure it is included in the comprehensive API security strategy.

- Threat Analysis - Providing systems that will automate the analysis of threats to DNS.

- Threat Intelligence - Give access to the actual intelligence behind threats to DNS.

- Whitelist / Blacklist - Being able to establish whitelists and blacklists of domains, IP addresses, and other criteria for DNS level defense.

- Denial of Service (DDOS) - DNS tools for identifying and defending against a denial of service (DOS) attack.

## Stability
Consider what it will take to ensure the DNS layer of delivering services is reliable, redundant, and can be included as part of the wider SLA being put forth.

- Health Monitors - The ability to monitor domain health and availability, and receive notifications, or take actions based upon.

- DNS Failover - Allowing for failover at the DNS level, providing redundancy and failover of
DNS infrastructure.

- Latency Based Routing - Being able to route DNS traffic to different locations based upon latency of networks.

- Verification - Ability to verify availability, and health of DNS infrastructure, and certifying for other parties.

- Service Level Agreement - Providing a service level agreement for DNS customers.

## Awareness
Ensuring there is awareness of all activity occurring at the DNS layer, and providing the services and tools needed to establish and maintain this awareness.

- Analytics - Providing analytics about DNS configuration and operations an operation through visual interface.

- Reporting - Provide self-service reporting tools on DNS activity and services.

- History - Give access to DNS activity history allowing for the search and browsing of all services in the past.

## Utility
Some of the the more utility aspects of managing DNS that don't fit into their own category currently, so they are aggregated into a single list for consumption.

- Diagnostic - Providing diagnostic tools for DNS setup.

- Batch Requests - Allowing for batch request submissions of DNS changes.

- Templates - Providing the ability to create and use templates when configuring DNS.

- Import - Allowing for the import of DNS configuration using portable formats.

- Export - Allowing for the export of DNS configuration using portable formats.

- API - A set of API resources available for managing all aspects of DNS operations, so that DNS for API operations can be automated.

- Command Line Interface - Providing a command line interface for managing DNS services.

# Deployment
The myriad of ways in which APIs are deployed from existing backend system, databases, filesystems, and proxying, and building facades of older legacy, or 3rd party services. There are often too many ways to deploy an API, making it a difficult area to easily bring into focus and lead developers and business stakeholders through.

## Database
The backend database schema, infrastructure, and other relevant information regarding how data is managed, and leveraged to deploy APIs, and deliver the resources needed to make the services work.

- ODBC - Providing a general ODBC solution that allows for quick access to tables and fields, making data available through an API from any ODBC compliant database.

- JDBC - Providing a general JDBC solution that allows for quick access to tables and fields, making data available through an API from any ODBC compliant JDBC.

 - MySQL - Providing a connection to MySQL database that allows for quick access to tables and fields, making data available through an API from the backend database.

 - SQL Server - Providing a connection to SQL Server database that allows for quick access to tables and fields, making data available through an API from the backend database.

 - Oracle - Providing a connection to Oracle database that allows for quick access to tables and fields, making data available through an API from the backend database.

 - PostGres - Providing a connection to PostGres database that allows for quick access to tables and fields, making data available through an API from the backend database.

 - Aurora - Providing a connection to Aurora database that allows for quick access to tables and fields, making data available through an API from the backend database.

 - SimpleDB - Providing a connection to SimpleDB data store that allows for quick access to tables and fields, making data available through an API from the backend database.

 - IBM DB2 - Providing a connection to IBM DB2 database that allows for quick access to tables and fields, making data available through an API from the backend database.

 - SAP - Providing a connection to SAP database that allows for quick access to tables and fields, making data available through an API from the backend database.

 - MariaDB - Providing a connection to MariaDB database that allows for quick access to tables and fields, making data available through an API from the backend database.

 - MongoDB - Providing a connection to MongoDB database that allows for quick access to tables and fields, making data available through an API from the backend database.

 - Redis - Providing a connection to Redis database that allows for quick access to tables and fields, making data available through an API from the backend database.

## Connector
Providing ready to go connectors that allow developers to easily deploy web APIs from existing resources without coding, or with as light of a touch as possible when it comes to needing engineering resources.

### Common Connectors
Some of the most common connections for taking existing backend resources and turning them into APIs, often times without having to write code, and something that non-developers can do.

- HTTP - Providing a ready to go HTTP connector for working with other HTTP services, and then transforming them into a new API for different audience or purposes.

- RSS - Providing a ready to go RSS connector for working with other RSS feeds, and then transforming them into a new API for different audience or purposes.

- Atom - Providing a ready to go Atom connector for working with other Atom feeds, and then transforming them into a new API for different audience or purposes.

- FTP - Providing a ready to go FTP connector for connecting to an existing FTP location and publishing available files via a web API.

- SFTP - Providing a ready to go SFTP connector for connecting to an existing FTP location and publishing available files via a web API.

- SOAP - Providing a ready to go SOAP connector for working with other existing SOAP services, and enabling them to be transformed into a new API for different audience or purposes.

- IMAP - Providing a ready to go connector for IMAP, allowing email services to be securely accessed and served up via a new web API.

- POP - Providing a ready to go connector for POP, allowing email services to be securely accessed and served up via a new web API.

- LDAP - Providing a ready to go connector for LDAP, allowing email services to be securely accessed and served up via a new web API.

- File System - Providing a connector that helps abstract away a file system store, and offer up as a web API, making it easier to provide access to the local or network file system.

### 3rd Party Connectors
Providing a list of all the 3rd party connectors that are available and enable the deploying of APIs from existing services that are being consumed outside the firewall. Providing a common way to abstract away the service and make available as part of service stacks.

- SalesForce - Providing a ready to go connector for working with the SalesForce API, allowing an existing 3rd party service in use to be made available via a web API.

- Netsuite - Providing a ready to go connector for working with the Netsuite API, allowing an existing 3rd party service in use to be made available via a web API.

- Hubspot - Providing a ready to go connector for working with the Hubspot API, allowing an existing 3rd party service in use to be made available via a web API.

- SugarCRM - Providing a ready to go connector for working with the SugarCRM API, allowing an existing 3rd party service in use to be made available via a web API.

- Zoho - Providing a ready to go connector for working with the Zoho API, allowing an existing 3rd party service in use to be made available via a web API.

- Hubspot - Providing a ready to go connector for working with the Hubspot API, allowing an existing 3rd party service in use to be made available via a web API.

- Marketo - Providing a ready to go connector for working with the Marketo API, allowing an existing 3rd party service in use to be made available via a web API.

- Concur - Providing a ready to go connector for working with the Concur API, allowing an existing 3rd party service in use to be made available via a web API.

## Proxy
A lightweight, service or tool-based approach to getting in the way of an existing service and applying transformations on it before the results are accessed via consistent services delivered using APIs.

- Reverse Proxy - An intermediary for servers to be contacted by any client, allowing for transformations and filtering before delivery.

- Forward Proxy - An intermediary for clients to contact any server, allowing for transformations and filtering before delivery.

- Authentication - Details regarding what authentication flows are available within the proxy, allowing for integration with as many common approaches to API authentication.

- Service - What 3rd party services are available for delivering proxy services in association with a platform's operation, providing a sanctioned commercial service.

- Tools - What open source tooling is available for delivering proxy services in association with a platform's operation, providing a vetted solution for delivering the proxy.

- Proxy Endpoint: The resulting endpoint of the proxied source, allowing access to the results of any proxied API being targeted.

- Target Endpoint - The URL of the target being proxied, allowing for the backend connection of existing resources, and the delivered via proxy.

- Conditional - Providing solutions for applying conditional logic to what flows through the proxy, allowing anyone to set conditions of its operation.

- Scripting - Allowing for scripts to be added and executed at runtime by the proxy, allowing for custom transformations to occur as part of proxying.

- Policies - Enabling a policy framework that allows standardized policies to be applied to a variety of use cases, and conditions, helping organize how a policy does what it does.

- Caching - Enabling the caching of data, and content flowing through the proxy, and use as part of performance, reliability, and historical access to proxied resources.  

- Circuit Breaking - Providing fault tolerance within a proxy, allowing it to respond in a constructive way when their targets and sources fail.

## Gateway
A heavier duty implementation that provides a doorway to new or existing services, providing more robust solutions for accessing backend services via web APIs.

- Authentication - Details regarding what authentication flows are available within the gateway, allowing for integration with as many common approaches to API authentication.

- Definitions - Allowing for the importing and exporting of API definitions and schema to define, evolve, and make the structure of APIs portable.

- Connectors - Enabling the easy connection to backend resources that have already been defined, allowing anyone to quickly connect, and make available as a web API.

- Service - What 3rd party services are available for delivering gateway services in association with a platform's operation, providing a sanctioned commercial service.

- Tools - What open source tooling is available for delivering gateway services in association with a platform's operation, providing a vetted solution for delivering the gateway.

## Search
Leveraging search services and tooling to index and make existing resources accessible, allowing for documents, structured, and unstructured data to be deployed as web APIs.

- Authentication - Information about authenticating at disk, and existing APIs, content sources, and services, accommodating the majority of common ways to authenticate.

- Connectors - Enabling the easy connection to document stores, storage solutions, and existing CDN to allow for indexing and delivery as web APIs, in a scalable and consistent way.

- Indexing - Allowing for indexing of structured and unstructured data for inclusion in search indexes which can then be leverage by a variety API driven services.

- Service - What 3rd party services are available for delivering search services in association with a platform's operation, providing a sanctioned search solution.

- Tools - What open source tooling is available for delivering search services in association with a platform's operation, providing a vetted solution for delivering the search services.

## Scraping
Obtaining content through scraping of web pages, and then allowing for the transformation of data and contained obtained, and deliver as simpler web APIs.

### Content Harvesting & Extraction
Defining how content and data will be harvested and extracting consistently across scraping operations.

- Concept Extraction - Extracting topics that are present as tags from extracted content

- Summarization - Providing a summarization of content that is extracted from a URL.

- Entity Extraction - Locate and classify named entities, such as the names of persons, organizations, locations from extracted content.

- Taxonomy & Classification - Identifying potential categories, and classifications present in extracted content.

- Relation Extraction - Detection and classification of semantic relationship identified within extracted text from URL.

- Article Extraction - Extraction of news and blog article from the content retrieved from a URL.

- Discussion Extraction - Extraction of structured and threaded conversations such as forums, and comments from extracted content.

- Date Extraction - Pulling of the dates from an article, blog post, and other content published via a URL.

- Author Extraction - Pulling of author names from an article, blog post, and content published by a specific individual.

- Product Extraction - The extraction of specific product related information like title, description, pricing, and images from content extracted from web pages.

- Related Phrases - Identifying related phrases with content extracted from website URL.

- Pagination Extraction - Identifying the breadcrumbs, and pagination for URLs where content is being extracted and providing necessary details to navigate and harvest as needed.

- Dictionaries - Provide the ability to create, access, and manage dictionaries from extracted content, and for applying to content that is harvested.

### Crawling
Establishing common practices for crawling of websites for discovery and targeting of content for consumption via scraping processes.

- Seed URLs - Allowing users to provide URLs that seed the web crawling process.

- Pseudo-URLs - Allow for the ability to provide URL patterns that will applied during the crawling process

- Scripting - Allow for scripting as part of the web crawling cycle.

- Conditional Expressions - Allow for the defining of conditional expressions that can be applied during the web crawling process.

- XPath - Allow the application of XPath when processing XML files during the web crawling process.

- RegEx - Opening up the ability to apply regular expression as part of evaluation during the crawling process.

- Injection - Allow for the injection of data and content into the crawling of web pages.

- Timeout - Giving users control over defining timeout limitations to be applied during the crawling cycle.

### Content Storage & Access
Defining how scraped content is organized as part of a wider scraping and harvesting workflow intending to get needed resources for making available via APIs.

- Content Latest Index - Providing access to the latest content crawled and harvest against a domain or list of domains.

- Historical Index - Allowing access to historical content that has been retrieved crawling and scraping URLs.

- Storage - Offering storage for content, data, and media that is scraped from URLs.

- Search - Providing search tools for access content that is scraped from URLs.

### Automation & Orchestration
Allowing for the automation and orchestration of the scraping process enabling it to be scaled, and automated to the needs of services.

- API - Provide an API for programmatically managing all aspects of the scraping and crawling process.

- Webhooks - Provide a webhook architecture for triggering or being notified of specific events when scraping and crawling.

- Command Line Interface - Offering a standardize command line interface set of options and commands for working with the scraping workflow.

### DNS
Allowing for the management of DNS associated with scraping, allowing for domains to be efficiently targeted, and excluded depending on what is needed.

- Domain Lists - Providing lists of domains, and subdomains to seed scraping and harvesting activities.

- Domain Metadata - Providing details about domains that can be used in the scraping and crawling process.

### Document Processing
Enabling the process of common types of documents for storing content and data, allowing the scripting to process contained documentations and make available via APIs.

- Feed Detection - Identifying the types of different documents and feeds available via URLs.

- PDF Extraction - The extraction of content from PDF documents harvested from URLs.

- Word Documents - Extraction of content from Word documents that are harvest via URLs.

### Integrations
Organizing a master list of 3rd party integrations available as part of the scraping services and tooling, allowing it to be further refined, processed, and made available across the lifecycle.

- Dropbox - Integration of crawling and scraping activities into Dropbox.

- Amazon S3 - Integration of crawling and scraping activities into Amazon S3.

- Google Sheets - Integration of crawling and scraping activities into Google Sheets.

- Plot.ly - Integration of crawling and scraping activities into Plot.ly.

- Silk - Integration of crawling and scraping activities into Silk.

- Tableau - Integration of crawling and scraping activities into Tableau.

### International
Making the scraping process as flexible as possible when it comes to identifying languages, and adjusting to different geographic regions being targeted.

- Language Detection - Providing language detection resources for applying against content and data that is extracted from URLs.

- Geo IP Address - Providing the ability to harvest and scrape content and data from specific IP addresses located in specific geographic regions and countries.

### Machine Learning
Defining what type of machine learning resources can be applied as part of the scraping process, building in intelligence and evolving how scraping of data and content occurs.

- Semantic Text Analysis - Relating syntactic structures, from text to the level of the writing as a whole, to their language-independent meanings.

- Semantic Similarity - Look for the similarities that exist after relating syntactic structures in content to the level of the writing as a whole, to their language-independent meanings.

- Sentiment Analysis - Identify and categorize opinions expressed in content to interpret it's attitude towards a particular topic, product, etc., is positive, negative, or neutral.

- Emotion Analysis - Evaluating content for signs of human emotion presence such as sad or happy, complimenting and augmenting sentiment analysis.

### Media Acquisition
Enabling scraping operations to be able to target and work with a variety of media objects, allowing them to be able to work with a variety of content sources, and make sense of many formats.

- Image Extraction - The extraction of images from content pulled from URLs.

- Video Extraction - The extraction of videos from content pulled from URLs.

- Image Tagging - Tagging of images with specific topics when extracted from URLs.

- Image Color Extraction - Identifying of colors present in images extracted from URLs.

- Face Detection - Identifying faces within images and photos extracted from URLs.

- Barcode Recognition - Identifying barcodes that are present in images extracted from URLs.

- License Plate Recognition - The identification of vehicle license plates identified in photos and images extracted from URLs.

### Structured Data Extraction
Being able to work with structured data as part of the extraction process, making sure that data is consumed in the most meaningful and efficient way as possible.

- HTML Table Extraction - Pulling of HTML tables from content extracted via URLs.

- Spreadsheet Extraction - Extraction of structured data from spreadsheets harvested from URLs.

- CSV Files - Identification and processing of CSV files extracted from URLs.

- JSON Files - Identification and processing of JSON files extracted from URLs.

- Microformats Parsing - The parsing of common microformats from content extracted from URLs.

- XML Extraction - The extraction of structured data from XML files harvested from URLs.

### Utilities
Some other scraping items that will contribute to being able to effectively scrape and harvest content from across the web, for use in deploying services.

- Proxies - Allowing for the deployment, configuration, and operation of proxies that get applied as part of scraping and crawling.

- Cookies - Provide tooling for managing and configuration cookies that are used as part of scraping and crawling.

- Headers - Giving control over what headers are sent as part of the scraping and crawling process.

- User Agents - Allow for the customization of the user agent that identifies scraping and crawling tooling.

- IP Address - Provide the ability to select from different IP address pools, change, and optimize IP addresses used in the scraping and crawling process.

- Logging - Providing logging for scraping and crawling with the ability to search, and configure as needed.

- Batch Calls - Provide the ability to make more than one call at once, tackling multiple objects at once.

- Scheduler - Enable the ability control the schedule for the execution of scraping and crawling jobs.

- Low Latency - Allow for low latency scraping and crawling, limiting the impact on targets.     

### Analytics
Providing a set of analytics for the scraping and harvesting process, allowing for domains, and other aspects of the process, ensuring the effectiveness of activity, and ingesting the highest quality sources as possible.

- Reporting - Providing reporting on crawling and scraping activities.

- URL Metrics - Provide metrics on specific URLs, offering detail on its activity.

- Spam Score - Providing a spam score for domains or URLs included as part of crawling and spider process.

- Rankings - Providing rankings that can be applied to domains, URLs, content, data, media, and other building blocks of the crawling and scraping activities.     

## Compute
How is the underlying compute delivered for each service using containers, serverless, cloud, and on-premise infrastructure.

- Instance Sizes - Making available a variety of instance sizes, and establish standard practices for evaluation and deployment of compute instance sizes.

- GPU Instances - In addition to a standard set of instance sizes, there are GPU instance for media, machine learning, and other more intensive compute situations.

- IAM - Defining what the identity and access management layer and policies look like for access compute resources allocated for API deployment.

- Regional Capacity - Opening up the opportunity for multi-region deployment, establishing common practices for thinking about about one or many regions can be leveraged for compute deployment.

- Auto Scaling - Setting the stage for auto scaling of compute resources will occur, allowing the autoscaling of underlying compute for all services.

- Load Balancing - Documenting what the process is for the load balancing of compute resources, so that API resources can be scaled out horizontally, and across regions.

- Networking - Outlining what is the standard process for network setup, configuration, and management for each available service.

- Machine Images - Establishing a regular imaging, update, patches, and maintenance definition for the underlying compute employed by search service.

- Backups - Enabling the backing up of the compute layer, allowing for easy recovery, and scaling from images, but also recurring backup sources.

- Security Groups - Establishing security groups as part of wider security strategy, and identifying logical groups for each group of services.

## Storage
What does storage of all heavy objects, media, and other assets involved with the delivery of services.

- Object Storage - Allowing for the storage of any size objects in the cloud, and allocating a portion of it for centralized storage across services, but determining relative security and access control management when it comes to delivering microservices.

- IAM - Defining what the identity and access and management layer and policies look like for access compute resources allocated for API deployment.

- Backup Storage - Ensuring there is a lower cost storage options for data that won't be accessed very often, but should remain available and usable, but at a lower rate.

- Bucket Stores - Allowing for buckets to be created for storing of different types of information, and isolating service storage to individually defined buckets.

- Interoperability - Enabling the interoperability of storage across storage API providers, allowing for single service access to objects stored across multiple providers.

- Migration - Powering the migration of data from other locations, allowing for large volumes of data to be migrated from an existing location on recurring or one time basis.

## Containers
Providing standard practices for defining, deploying, and managing the deployment of services using common containerization services and tooling, making services as modular as scalable as they can be.

- Image Registry - Establishing a container image registry with available container images, and instructions for how images are meant to be deployed in support of services.

- IAM - Defining what the identity and access management layer and policies look like for access compute resources allocated for API deployment.

- Security - Establish what the security practices are for scanning, auditing, and executing after deploying APIs within container, as well as on a regular schedule.

- Policies - Defining policies that can be applied at the container level, guiding how they are used to power different types of services.

- Network - Allowing for the configuration of the underlying network for each container that is powering different types of services.

- Volumes - Establish storage volumes using one of the designated storage services, providing isolated, but universally accessible and scalable storage volumes.

- Orchestration - Identify the tools available for orchestrating container deployment across a variety of locations, regions, but working towards a larger API lifecycle strategy.

- Secrets - Providing secrets storage at the container level, allow each API to securely store and access tokens, passwords, and other secrets.

- Configuration - Define what the configuration options are for each container, allowing each one to be customized, and adjusted to meet the needs of each service.

## Frameworks
The essential code scaffolding that can be used to deploy consistent APIs, using a full toolbox of common API patterns used across the industry.

### REST API Frameworks
Providing a robust list of API frameworks for deploying REST API services, providing a common framework that leverages the web for making services available.

- PHP - A REST API framework for easily deploying APIs, and handles all the most common elements of deploying an API, in the PHP language.

- Python - A REST API framework for easily deploying APIs, and handles all the most common elements of deploying an API, in the Python language.

- Ruby - A REST API framework for easily deploying APIs, and handles all the most common elements of deploying an API, in the Ruby language.

- Node.js - A REST API framework for easily deploying APIs, and handles all the most common elements of deploying an API, using the Node.js language.

- C Sharp - A REST API framework for easily deploying APIs, and handles all the most common elements of deploying an API, in the C Sharp (#) language.

- Java - A REST API framework for easily deploying APIs, and handles all the most common elements of deploying an API, using the Java language.

- Go - A REST API framework for easily deploying APIs, and handles all the most common elements of deploying an API, in the Go language.

### GraphQL API Frameworks
Providing a robust list of API frameworks for deploying GraphQL API services, providing a common framework for delivering the API while also providing a query language layer on top of all services.

- PHP - A GraphQL API framework for easily deploying APIs, and handles all the most common elements of deploying an API, in the PHP language.

- Python - A GraphQL API framework for easily deploying APIs, and handles all the most common elements of deploying an API, in the Python language.

- Ruby - A GraphQL API framework for easily deploying APIs, and handles all the most common elements of deploying an API, in the Ruby language.

- Node.js - A GraphQL API framework for easily deploying APIs, and handles all the most common elements of deploying an API, using the Node.js language.

- C Sharp - A GraphQL API framework for easily deploying APIs, and handles all the most common elements of deploying an API, in the C Sharp (#) language.

- Java - A GraphQL API framework for easily deploying APIs, and handles all the most common elements of deploying an API, using the Java language.

- Go - A GraphQL API framework for easily deploying APIs, and handles all the most common elements of deploying an API, in the Go language.

### gRPC API Frameworks
Providing a robust list of API frameworks for deploying gRPC API services, providing a common framework for delivering the API while increasing efficiency, performance, and leveraging HTTP/2 as a transport.

- PHP - A gRPC API framework for easily deploying APIs, and handles all the most common elements of deploying an API, in the PHP language.

- Python - A gRPC API framework for easily deploying APIs, and handles all the most common elements of deploying an API, in the Python language.

- Ruby - A gRPC API framework for easily deploying APIs, and handles all the most common elements of deploying an API, in the Ruby language.

- Node.js - A gRPC API framework for easily deploying APIs, and handles all the most common elements of deploying an API, using the Node.js language.

- C Sharp - A gRPC API framework for easily deploying APIs, and handles all the most common elements of deploying an API, in the C Sharp (#) language.

- Java - A gRPC API framework for easily deploying APIs, and handles all the most common elements of deploying an API, using the Java language.

- Go - A gRPC API framework for easily deploying APIs, and handles all the most common elements of deploying an API, in the Go language.

## Serverless
Powering the serverless deployment of services, using scalability scripts and functions to drive each service, and individual API paths.

### Core Functionality
Running scripts in a variety of programming languages individually as the backend for each services API path.

- Java - Enabling the deployment of scripts written in the Java programming language, which can be independently scaled, and used by each service, and its individual paths.

- Node.js - Enabling the deployment of scripts written in the Node.js programming language, which can be independently scaled, and used by each service, and its individual paths.

- C# - Enabling the deployment of scripts written in the C# programming language, which can be independently scaled, and used by each service, and its individual paths.

- Go - Enabling the deployment of scripts written in the Go programming language, which can be independently scaled, and used by each service, and its individual paths.

- Groovy - Enabling the deployment of scripts written in the Groovy programming language, which can be independently scaled, and used by each service, and its individual paths.

- Kotlin - Enabling the deployment of scripts written in the Kotlin programming language, which can be independently scaled, and used by each service, and its individual paths.

- PHP - Enabling the deployment of scripts written in the PHP programming language, which can be independently scaled, and used by each service, and its individual paths.

- Swift - Enabling the deployment of scripts written in the Swift programming language, which can be independently scaled, and used by each service, and its individual paths.

- IAM - Providing an identity and access management layer that is in sync with security for other backend systems, and across all exposed services.

### Availability
Dialing in the performance and availability of each serverless script or function allowing them to behave differently depending on the type of service it is driving.

- Fault Tolerance - Automatically balancing scripts and functions across many locations, providing failover and redundancy by default.

- Scaling - Automatically scaling each script and function independently, allowing for usage spikes to occur without any disruption or performance loss.

- Orchestration - Providing tools for orchestrating and working with serverless scripts and functions in sequence, batches, groups, and other more organized, concerted efforts.

- Scheduling - Allowing for scripts to be executed based upon a schedule, operating individual scripts at scale across a multitude of functions.

- Event-Driven - Operating scripts and functions in response to events that occur via backend systems, logs, database, and other common services.

- Websub - Enabling the orchestration of serverless scripts using Websub, a publish subscribe standard for enabling a real-time, event-driven, topical layer on top of services.

### Frameworks
Some of the open source frameworks available for deploying of serverless solutions, for a variety of use cases.

- Serverless Framework - Build applications comprised of microservices that run in response to events, autoscale for you, and only charge you when they run. This lowers the total cost of maintaining your apps, enabling you to build more logic, faster. - https://github.com/serverless

- OpenWhisk - Apache OpenWhisk (Incubating) is a serverless, open source cloud platform that executes functions in response to events at any scale. With Apache OpenWhisk you can easily create actions, test, connect to other actions or debug them. - https://openwhisk.apache.org/

## Orchestration
Defining what the build, syndication, and orchestration of service deployments and integrations look like, and are executed, realizing a more organized and effective continuous integration and deployment workflow.

- Version Control System - Establish which version control systems are available, allowing support for Github, Gitlab, Bitbucket, or other supported solution.

- Pipeline - Allowing for the modeling and defining the API deployment or integration context, establishing something that is repeatable, and reliable.

- IAM - Providing a comprehensive identity and access management layer for ensuring there is proper access to every element present in the pipeline and model definition.

- Environments - Establishing a common approach to defining relative environments involved in the deployment, testing, and building of each service.

- Steps - Precise modeling of each step in the deployment of each service, providing everything that is needed from start to finish.

- Tests - Building in tests for the entire servicestack into the orchestration environment, ensuring consistent and reliable deployment of services.

- Artifacts - Organized management and accounting of all artifacts involved in the build process, using them as definitions in the overall API lifecycle.

- Playback - Enabling the playback, review, and audit of each step involved with a build model and pipeline, allowing them to be cracked open and understood.

- Deployment - Allowing for deployment to any environment that is on-premise, in the cloud, via containers, and any other deployment target that has been already defined.

- Integrations - Establishing ready to go integrations for common deployment and integration targets, allowing for each setup, and management of the most common integration services.

- Plugins - Providing a define suite of plugins that should be used as part of the service delivery lifecycle, adding to the overall pipeline and model flow, and extend the features of the CI/CD solution.

- Command Line Interface - Define programmatic control over the orchestration lifecycle using a command line interface (CLI) solution, allowing for easy command line execution and engagement with the build workflow.

- API - Ensuring that the orchestration layer possess an API, and can leverage external 3rd party APIs as part of the build workflow, making sure that we can seamlessly execute every step of the process.

- Notifications - Providing a notification layer around all the events that can occur throughout the modeling, and pipeline build process, keeping everyone involved up date regarding each build.

- Messaging - Opening up channels for messaging to occur around models, pipelines, and the builds that make up the continuous integration and deployment cycles.

# Dependencies
Identifying all backend service, code and infrastructure dependencies present for each service.

- Identifying - Process for identifying dependencies between services, and as part of the overall model, pipeline, and build process, while establishing channels of communication as well.

- Defining - Establishing the ability to define service dependencies in a machine readable format that can be included as part of the wider life cycle artifacts.

- Visualizing - Enabling the ability to visualize dependencies between services, making every service, framework, system, and other scope of dependency easy to see.

- Drill Down - Allow for the ability to drill down on dependencies and understand and explore how connected services across all lines of business.

- Scope - Allow for the definition of different levels of dependencies depending on where they are in the service stack, and properly defining the scope of the dependency.

# Virtualization
Details how how services and their underlying data are mocked, virtualized, sandboxed, and made available for non-production usage.

## Core Virtualization
Delivering the core features of virtualization and making sure there are relevant and useful representations of services available to work with when developing, staging, and testing of services.

- Mock - Creation of mock API interfaces that matches a specific API definition.

- Sandbox - Generation of a sandbox environment that matches a specific API definition.

- Simulator - Creation of simulation environments from existing definitions.

- Record - Recording the setup of a virtualization environment for use at later date.

- Playback - Setup of a virtualized environment captured from recording of earlier instance.

- Verification - Verification that a virtualization environment exists and matches existing definition.

- Port Forwarding - Forward of specific ports to a specific virtualized API instance.

- SSL - Use of SSL when communicating with virtualized API instances.

## Data Virtualization
Not just virtualizing APIs and other aspects of the services, but also virtualizing the data that is made available via services, allowing for meaningful data for development and testing.

- Templates - Being able to create templates of data to be used when virtualized APIs are setup.

- Dummy Data - Dummy data sets that can be imported individually or as collections into virtualized APIs.

- Excel Data - Import of data from Microsoft Excel spreadsheets or Google sheets into virtualized APIs.

## Import / Export
Allowing for the importing and exporting of API definitions to be used to generate virtualized instances of services that can be used in testing and development.

- Import OpenAPI Spec - Allow for the creation of virtualized APIs using existing OpenAPI Spec definitions.

- Import API Blueprint - Allow for the creation of virtualized APIs using existing API Blueprint definitions.

- Import WADL - Allow for the creation of virtualized APIs using existing WADL definitions.

- Import Postman - Allow for the creation of virtualized APIs using existing Postman definitions.

## Collaboration
Enabling the ability to collaborate around the deployment, availability, and testing of virtualized infrastructure in support of services.

- Reporting - Providing reporting tools on virtualized instances, providing developers and consumers with snapshots of activity.

- Analytics - Provide real-time, and other analytics that give details of what is happening with virtualized APIs as they operate.

- Teams - Provide team tooling, allowing multiple individuals to work together when monitoring API virtualization.		

# Authentication
What is involved with authentication across all services, including key-based approaches, basic authentication, JWT, and OAuth solutions.

## Overview
Relevant overview information about authentication across services, providing what is needed to get started understanding how authentication will work across service integrations.

- Inline Token Generator - Allowing developers to request token inline with documentation.

- Authentication Overview - An overview of how authentication is handled for a platform, and which formats are supported, setting expectations for consumers.

- Authentication Tester - Providing a testing tool for authentication, that allows developers to test key and Basic Auth to oAuth, to help them understand how authentication works and if they are using proper credentials.

- OAuth Scopes - Providing a dedicated page or section to listing out the different OAuth scopes used by a platform. Providing a transparent window into all the scopes available, and some of the logic into why they exist.

- Test Token Generator - Providing the ability to generate test tokens for use in authenticating with the API.

## Approaches
Details about the supported approaches to authentication in place, or supported by different services, leverage the most common patterns, and building on authentication and access management standards.

- Key Access - Providing simple tokens, often called API key as a common way to access to APIs, issuing one to each developer and per application they register.

- Basic (RFC 7617) - The Basic authentication scheme is based on the model that the client needs to authenticate itself with a user-id and a password for each protection space ("realm"). The realm value is a free-form string that can only be compared for equality with other realms on that server. - http://webconcepts.info/concepts/http-authentication-scheme/

- Bearer (RFC 6750) - All challenges defined by this specification MUST use the auth-scheme value "Bearer". This scheme MUST be followed by one or more auth-param values. - http://webconcepts.info/concepts/http-authentication-scheme/

- Digest (RFC 7616) - The Digest scheme is based on a simple challenge-response paradigm. The Digest scheme challenges using a nonce value and might indicate that username hashing is supported. A valid response contains an unkeyed digest of the username, the password, the given nonce value, the HTTP method, and the requested URI. - http://webconcepts.info/concepts/http-authentication-scheme/

- HOBA (RFC 7486) - An HTTP server that supports HOBA authentication includes the "HOBA" auth-scheme value in a WWW-Authenticate header field when it wants the client to authenticate with HOBA. - http://webconcepts.info/concepts/http-authentication-scheme/

- Mutual (RFC 8120) - The scheme provides true mutual authentication between an HTTP client and an HTTP server, using just a simple password as a credential. - http://webconcepts.info/concepts/http-authentication-scheme/

- Negotiate (RFC 4559) - Use of Kerberos is wrapped in an HTTP auth-scheme of "Negotiate". - http://webconcepts.info/concepts/http-authentication-scheme/

- OAuth (RFC 5849) - Protocol parameters can be transmitted using the HTTP "Authorization" header field as defined by RFC 2617 with the auth-scheme name set to "OAuth" (case insensitive). Servers MAY indicate their support for the "OAuth" auth-scheme by returning the HTTP "WWW-Authenticate" response header field upon client requests for protected resources. - http://webconcepts.info/concepts/http-authentication-scheme/

- SCRAM-SHA-1 (RFC 7804) - HTTP SCRAM is an HTTP Authentication mechanism whose client response and server challenge messages are text-based messages containing one or more attribute-value pairs separated by commas. SCRAM-SHA-1 is registered for database compatibility with implementations of RFC 5802 that want to also expose HTTP access to a related service, but it is not recommended for new deployments. - http://webconcepts.info/concepts/http-authentication-scheme/

- SCRAM-SHA-256 (RFC 7804) - HTTP SCRAM is an HTTP Authentication mechanism whose client response and server challenge messages are text-based messages containing one or more attribute-value pairs separated by commas. For interoperability, all HTTP clients and servers supporting SCRAM MUST implement the SCRAM-SHA-256 authentication mechanism. - http://webconcepts.info/concepts/http-authentication-scheme/

- vapid (Internet Draft ietf-webpush-vapid) - This authentication scheme carries a signed JWT, plus the key that signed that JWT. This authentication scheme is for origin-server authentication only. Therefore, this authentication scheme MUST NOT be used with the Proxy-Authenticate or Proxy-Authorization header fields. - http://webconcepts.info/concepts/http-authentication-scheme/

- JSON Web Token - JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

- OpenID - Providing simple identity layer on top of the OAuth 2.0 protocol, which allows computing clients to verify the identity of an end-user based on the authentication performed by an authorization server, as well as to obtain basic profile information about the end-user in an interoperable and REST-like manner.

- HMAC - Leveraging cryptography, an HMAC (sometimes disabbreviated as either keyed-hash message authentication code or hash-based message authentication code) is a specific type of message authentication code (MAC) involving a cryptographic hash function and a secret cryptographic key to gain access to each service.

# OAuth Specifications

- OAuth 2.0 Dynamic Client Registration Management Protocol (RFC 7592) - This specification defines methods for management of OAuth 2.0 dynamic client registrations for use cases in which the properties of a registered client may need to be changed during the lifetime of the client. Not all authorization servers supporting dynamic client registration will support these management methods. - http://webconcepts.info/specs/IETF/RFC/7592
- OAuth 2.0 Dynamic Client Registration Protocol (RFC 7591) - This specification defines mechanisms for dynamically registering OAuth 2.0 clients with authorization servers. Registration requests send a set of desired client metadata values to the authorization server. The resulting registration responses return a client identifier to use at the authorization server and the client metadata values registered for the client. The client can then use this registration information to communicate with the authorization server using the OAuth 2.0 protocol. This specification also defines a set of common client metadata fields and values for clients to use during registration. - http://webconcepts.info/specs/IETF/RFC/7591
- OAuth 2.0 Token Introspection (RFC 7662) - This specification defines a method for a protected resource to query an OAuth 2.0 authorization server to determine the active state of an OAuth 2.0 token and to determine meta-information about this token. OAuth 2.0 deployments can use this method to convey information about the authorization context of the token from the authorization server to the protected resource. - http://webconcepts.info/specs/IETF/RFC/7662
- OAuth 2.0 Token Revocation (RFC 7009) - This document proposes an additional endpoint for OAuth authorization servers, which allows clients to notify the authorization server that a previously obtained refresh or access token is no longer needed. This allows the authorization server to clean up security credentials. A revocation request will invalidate the actual token and, if applicable, other tokens based on the same authorization grant. - http://webconcepts.info/specs/IETF/RFC/7009

## JSON Web Token Specifications

- JSON Web Token (JWT) (RFC 7519) - JSON Web Token (JWT) is a compact, URL-safe means of representing claims to be transferred between two parties. The claims in a JWT are encoded as a JSON object that is used as the payload of a JSON Web Signature (JWS) structure or as the plaintext of a JSON Web Encryption (JWE) structure, enabling the claims to be digitally signed or integrity protected with a Message Authentication Code (MAC) and/or encrypted. - http://webconcepts.info/specs/IETF/RFC/7519
- JSON Web Token (JWT) Profile for OAuth 2.0 Client Authentication and Authorization Grants (RFC 7523) - This specification defines the use of a JSON Web Token (JWT) Bearer Token as a means for requesting an OAuth 2.0 access token as well as for client authentication. - http://webconcepts.info/specs/IETF/RFC/7523

## Additional Considerations
Some of the other considerations involved with authentication around services being offered via the platform.

- Application Only - Provides authenticated requests on behalf of the application only, and not targeting any particular user account.

- PIN Based Authorization - For applications which cannot access or embed a web browser, such as command-line applications, embedded systems, game consoles, and certain types of mobile apps.

- Two Factor Authentication - Allowing API consumers to turn on and employ two factor authentication, requiring an additional component to making changes to account security, either by SMS or authenticator app.         

# Portal
The strategy for how all services are required to be published to one or many public, private, and partner developer portals.

- Dedicated Location - Providing a dedicated location for all targeted API consumers to find the portal, and find all relevant resources.

- Dedicated Subdomain - Establishing a single subdomain for accessing the API portal, usually at http://developer.example.com, making it simple, intuitive, and consistent with the rest of the industry.

- Publicly Available - Will the API portal be publicly available? Available for anyone to access the information available within the portal, even if the API requires signing up for and requesting access to actually use.

- Privately Available - Will the API portal be only available within the corporate firewall, or may locked down for viewing by just a handful of partners.

- Continuously Deployed - Consider making the portal a statically generated website that can be continuously updated as part of a CD pipeline.

- Continuously Integrated - Think about the implications of using machine readable definitions, and hosting the portal using a version control system that will allow elements of the portal to be used in other systems.

- Community Contributions - Open up the possibility of allowing the community to make suggestions, or possibly submit pull requests to contribute to the portal helping drive an API platform.

# Documentation
The requirements for what documentation is expected as part of each service presence, defining what the services delivers.

## Overview
Providing relevant overviews of the documentation available for a platform, providing a summary of what is available across all services.

- Overview - Simple title, and single paragraph describing what an API platform delivers.

- Authentication - Provide a summary, with link to more API authentication information.

- Single Page - Providing a single page for accessing API documentation without clicking too much.

- Endpoint List - Display a list of all available API endpoints in a single list for easy review of what is available within a platform.

- Resource List - A single bulleted list of all the available resources for an API platform.

- What's New - A simple, up to date list of what has changed recently across all documentation.

- RSS / Atom - An RSS or Atom feed for all changes made to documentation.

## API Documentation
The details of an API's surface area, with all the details needed to put to services work, and be able to full integrate with the platform.

- Static - Providing static API documentation that details the surface area of the API, including requests, response, and schema details.

- Interactive - Publishing interactive API documentation using one of the common API definition driven documentation solutions, providing details of the requests, responses, and schema of an ApI.

- Status Codes - Provide a list of all the status codes available either for each individual APIs, or also across all API paths available via a platform.

- Errors - Provide details about errors returned across APIs, beyond the HTTP status code, with details codes, messages, and other elements.

- Postman Collection - Providing a single, or multiple Postman Collections that allow for an API to be executed in a single click.

- OpenAPI Definition - Providing a link to the OpenAPI definition that is behind the documentation, allowing it to be used for other purposes.

## Resources
The extra resources that are made available for developers to put to use in their integration journey, providing a wealth of resources to be applied across the API lifecycle.

- Case Studies - Offering a wealth of case studies of actual implementations that have occurred with an API , showing potential consumers what is possible.

- How-to Guides - Providing how-to guides that walk consumers through common aspects of API integration, giving them self-service resources they can use.

- White Papers - Offer white papers that educate consumers around topics that are relevant to the platform, consumers, and the industry that is being operated in.

- Webinars - Provide online webinars on a regular basis that API consumers can attend to learn about various aspects of platform operations.

- Events - Publish a page with information about any events the an API program will be attending, or maybe links to video and slide decks from past conferences.

- Slideshare - Publish a list of slide decks available on a Slideshare account, providing developers with access to past talks the API program has done.

- Codecademy - Creating courses on Codecademy, then publishing them within an API developer area, providing lessons for developers on how an API operates.

- Tour - Providing a guided tour of how a platform and API operates, allowing new developers to walk through all aspects of operations in an interactive or video format.

- Glossary - A glossary of terms that applies to an industry, platform, and the business or technical aspects of operations, providing API consumers who may not be familiar with sector or platform specific terms, with a dictionary they can use during integration.

- Videos - Provides video resources, helping people understand the API platform, how it can be put to use, and any other supporting areas of API operations.

# Management
Information about how services are composed, limited, measured, reported upon, and managed consistently across all services, providing a consistent definition to how services get managed.

## Access Control
Considering how APIs are being accessed at the service layer by authenticated users, while be organized in different ways, depending on the user, situation, and services in play.

- Groups - Defining, profiling, and planning for which groups will be accessing API resources, and organizing which services they will have access to.

- Keys - Outlining what the process will look like for issuing, managing, and revoking keys that give developers access to all services.

- Limits - Documenting what rate limitations will be in place for different groups when it comes to working with all services.

- Services - Possessing a complete list of services, their variations, and what the limitations and groups involved with their operations.

## Change
Making change happen at the API management layer, by building in awareness and intelligence into API operations at request time.

- Connectors - Defining the possible backend connectors available for binding the API management layer to backend systems and services using a variety of methods.

- Discovery - Providing options for discovery existing services that are available on the backend, allowing the management layer to pick up, and be the bridge for existing services.

- Mapping - Options for mapping each service to an existing backend service, binding some or all of the paths, schema, and other elements offered by an existing services.

- Transformations - Defining what transformations are possible, and will occur as a backend service is begin served up via an API through the API management layer.

- Filtering - Outlining what filters are available or being applied at the management layer, preventing certain features, data, and other elements from passing through the management layer.

- Validation - Details about what type of validation should occur at the management layer, ensuring that the path, request, or response elements of a service meet the required definition and schema.

- Circuit Breakers - Allowing for a circuit breaker model to exist between a service, and it's backend dependencies, triggering when a backend service becomes unreliable or unavailable.

## Extending
Exploring the ways in which API platforms are extending the features available at the API management layer, further customizing how APIs operate and are consumed.

- Plugins - What opportunities are there for extending the API management layer, adding functionality, and connecting to external services.?

- Connectors - What backend connectors are available for working with common backend systems like databases, file systems, LDAP, etc. Making it easier to deploy an API as well as manage.

- Scripting - Identify the opportunities for writing scripts and executing as part of the API management layer, allowing for custom code to be injected into the API request and response structure.

## On-boarding
What is involved with getting up and running with a service, setting the table for being able to properly manage API consumption and usage.

- Getting Started - Laying out simple, clear steps for developers on how to register, authenticate, access documentation and code samples, and get support and any other details that are essential to integration.

- Self-Service Registration - Providing a self-service registration for a developer portal, allowing developers to signup and get access to an API, 24 hours a day, 7 days a week.

- Best Practices - Publishing of a plain english introduction to the best practices around integrating with an API, providing introductory lesson for developers of how to properly integrate with an API.

- FAQ - Providing developers a list of the common questions asked of an API platform, with simple answers to each question, allowing them to understand the common problems faced during onboarding.

- Service Accord - Service level agreements (SLA) provide a legal framework managing the relationships between API consumers, and service accords provide a plain english explanation of what they expect from a provider, without the legaleze, in a format they can understand without calling the lawyers.

- Sign Up Email - Providing a simple, informative, personal email immediately upon signup, letting developers know what they need to onboard.

- Google Authentication - Allowing developers to create their API account using their Google account, and allowing the to login in the future using their Google oAuth.

- Github Authentication - Allowing developers to create their API account using their Github account, and allowing the to login in the future using their Github oAuth.

- Facebook Authentication - Allowing developers to create their API account using their Facebook account, and allowing the to login in the future using their Facebook credentials.

- LinkedIn Authentication - Allowing developers to create their API account using their LinkedIn account, and allowing the to login in the future using their LinkedIn credentials.

## Developer Account
What resources are available to a developer to help them manage their engagement with a platform, reflecting the overall management services that are available.

- Developer Dashboard - Provide developers a single dashboard for getting at all their tools, metrics and information they need to successfully manage their usage.

- Account Settings - Provide developers access to their basic account detail and settings, giving them quick access to their account configuration and allow for easy updates.

- Reset Password - Provide the necessary tools for developers to gain access to their account if they lose their password.

- Application Manager - Providing an interface that allows developers to manage one or many applications that will be integrating with an API.

- Usage Logs & Analytics - Allowing developers to be able to see where they stand with usage, logging and other aspects of operations, by providing them reports and analytics of their history.

- Billing History - Provide clear and easy access to what a developer has been billed, allowing them to access and download their billing history around API usage.

- Message Center - Providing developers with a messaging system within their developer accounts, and communicate with API providers, and receive system updates.

- Github Authentication - Allow developers to create and login to their API developer account using their own Github account credentials.

- Delete Account - Giving developers the ability to delete their account from within their account portal.

- Service Tier Management - Allow developers to change the service tier they operate with in via their developer dashboard, without having to request changes from platform support.

## Management API
Ensuring the the management layer has an API for developers to seamlessly integrate their solutions with the management layer of the services they are depending on.

- User Management - A user management API, enabling the ability to create, read, update, and delete information associated with a specific user.

- Account Management - An account management API, enabling users to create, read, update, and delete information associated with their account.

- Application Management - An application management API, allowing users to manage their registered applications, and get information about their consumption.

- Service Management - A service management API, providing users to see what services are available, and their access and usage levels for any given service. 	 

# Logging
What is being logged as part of service operations, and what is required to participate in overall logging strategy?

- Formats - Defining the support for many different logging formats, and mapping out all of the formats that are in use as default, or available with extra effort.

- Creation - Identifying EVERYWHERE logs are created and stored, ensuring that there is no single log file left untouched, and not aggregated and evaluated as part of the entire lifecycle.

- Ingestion - Quantifying how log files are ingested, and aggregated across a comprehensive, service wide logging strategy.

- Storage - Standardizing how logs are stored by default, as well as being aggregated, and made available for current or archival access.

- Retention - Defining how long logs are being stored across all systems relevant to a services operation, ensuring that each log entry has a time to live (TTL).

- IAM - Plan the identity and access and management management layer required for all aspects of logging, ensuring access across systems, as well as separate, secure storage of aggregate logs.

- Archive - Providing an archival process and storage for all logs that meets IAM and retention policies, allowing for clear definition of what should be archived.

- Events - Define the types of events that occur across logging activity allowing for granular definition of common or obscure events that occur around service operations.

- Alerts - Allow for notifications and alerts to be triggered for all activity and events that will be occurring via the platform, and allow relevant users to subscribe to the events that matter.

- Pub/Sub - Providing a publish / subscribe platform using Websub that identifying logging topics, and establishes channels that relevant users, systems, and applications can subscribe to the channels they need.

- Streaming - Offering a streaming option for subscribing to logging activities, events, and channels, providing real time one-way streaming APIs across logging efforts.

- Search - Allowing for each search across all aggregated log files, looking by keyword, tags, source, application, and other relevant data points that will matter to operations.

- Command Line Interface - Enable a command line interface at the aggregate log level, allowing for easy programmatic integration, orchestration, and integrated into the larger continuous build process.

- API - Making aggregate log files a first class citizen when it comes to API access, allowing robust access via simple web APIs, that provide secure access to all log files.

- Metrics - Establishing and documenting all metrics that are applied across log files, understand the data points that will matter the post when it comes to visualizations, analysis, and reporting.

- Tags - Embrace a tagging strategy that will allow for logs to be labeled, organized, and defined depending on what topics, and value they deliver to operations, security, and compliance.

- Visualizations - Integrating the aggregate logging APIs with the wider visualization strategy enabling the ability to see across all log activity, and events that occur in real time.

- Compliance - Defining the wider compliance strategy to ensure all logging efforts are meeting any compliance requirements, and that all relevant data is being stored or destroyed.

- Encryption - Applying encryption to all aggregate logging while being stored, and in transit, ensuring that no data is leaked at any point in the lifecycle.

- Troubleshooting - Providing solutions that assist with immediate troubleshooting across services, based upon errors, spikes, and other signals that indicate there might be a problem.

- Datensparsamkeit (Data Minimization) - It's an attitude to how we capture and store data, saying that we should only handle data that we really need.

# Support
Relevant support channels, points of contact, and best practices for receiving support as an API consumer.	 	

## Overview
Providing the default elements of providing support across the services that are available via the platform.

- Support Overview Page - Providing a single overview page where users can find a listing of available support resources, with an easy to find link to this page.

- Contact Form - A contact form available in the central API portal, that developers can use to ask questions.

## Self-Service Support
Enabling developers and consumers to be able to get support on their own, by providing help resources that do not require a person directly engage synchronously with users, allowing support to occur 24/7, and often assisted by the community.

- Forum - A modern, up to date, active, and well monitored forum, providing self-service access to information about an APIs operation.

- Forum RSS - Going beyond just a forum, and providing an RSS feed for all forum activity.

- Stack Overflow - Using the public QA site Stack Overflow as part of support operations for an API.

- Knowledgebase - Providing a single repository of content, organized by title, and tag, allowing you to search for keywords and phrases, as well as browse for answers.

## Direct Support
Also providing direct support opportunities so that all developers and consumers will be able to get direct support across all services, and actually engage with a human being to get the help they needed.

- Social - Providing direct support using existing social channels used by the platform, or parent organization.

- Email - Providing a simple email address that API consumers can use when looking to get answers to their questions.

- Phone - Providing a phone number that developers can call when they need support.

- Ticket System - Provide a central ticketing system for all support requests, possibly using popular support software like Zendesk.

- Office Hours - Dedicated a specific time each week or monthly where support staff will be available via live chat to answer questions.

- Calendar - A single calendar of all events related to API operations, providing a place where developers can find all related goings on.

- Paid Support - Providing paid support tiers for developers to use, allowing them to pay by the minute, hour, or project, and get the intimate, direct support they desire.

# Communications
Information about the communication strategy around each service, and how blogs, social, and other channels should be leveraged.

- Blog - Providing a blog dedicated to API platform operations, with stories about the providers, consumers, and other related stories.

- Blog RSS Feed - Make sure there is an RSS feed for any blog that is published as part of API operations.

- Twitter - Provide an active Twitter account for support, as well as evangelism efforts around an APIs operations.

- Email Newsletter - Provide an email for not just support, but also general platform communications.

- LinkedIn - Provide an active LinkedIn account for support, as well as evangelism efforts around an APIs operations.

- Facebook - Provide an active Facebook account for support, as well as evangelism efforts around an APIs operations.

- Google+ - Provide an active Google+ account for support, as well as evangelism efforts around an APIs operations.

- Email Newsletter - An email newsletter dedicated to cover news across platform operations, providing weekly summary of activity in the inbox.

- Instagram - Using Instagram as a way to communicate with platform users, and let users know there is someone home.

- Vimeo - Using Vimeo as a communication channel for educating users about an API platform.

- Youtube - Using Youtube as a regular content and communication channel to help users learn about platform operations.

- Chat - Providing a live chant mechanism in the developer portal, allowing developers to connect directly with API support and evangelists.

- Slack - Using Slack to create private channels just for communicating with internal, partner, or public API consumers.

# Road Map
Details on a services road map, and what the future will hold, providing individual service, as well as larger organizational details on what is next.	 	 

- Road Map - A detailed list of what additions and changes are being planned as part of API operations, giving consumers a place where they can go learn about what is next in an APIs evolution.

- Idea Submission - Allow for the submission of ideas, using the Github issue management, or other system, giving API consumers the ability to potentially contribute to the API road map.       

# Issues
Expectations, communications, and transparency around what the current bugs, issues, and other active problems exist on a platform.

- Issues - Showcasing what the open issues are, letting people know they are outstanding, saving the need to report.

- Status RSS - Providing an RSS feed for a status dashboard, allowing users to receive updates on any website, and via any RSS client.

- Status Dashboard - A single location, at dedicated subdomain, providing status update(s) for all API resources, giving developers a place to go when looking to see if platform is available.

- Status History - Providing a history of status, usually by day, and showing results month by month, or week by week, as long as status has been tracked for an API.

# Change Log
Translating the road map, and issues into a log of activity that has occurred for each service, providing a history of the service.

- Change Log - A detailed list of changes have been made to an API platform, giving consumers a single place they can go to learn about what changes have been made.

# Monitoring
What is required when it comes to monitoring the availability and activity of each individual service.

## Authentication
Providing a standardized approach to authentication across monitoring services, allowing monitoring services to have the access they need to properly monitor what is happening.

- Basic Auth - Using Basic Auth, a username and password for authentication.

- OAuth - Using OAuth for platform authentication.

- API Keys - Using API keys for authentication.

## Core Details
The core aspects of operating a monitoring campaign across all services, ensuring that they are granularly monitored and ensured they are meeting SLAs.

- Service Availability - Making sure a service is available.

- Latency Measurement - Measuring the latency associated with a specific request.

- Response Header Validation - Being able to validate for a specific header for a request.

- Response Body Validation - Being able to validate the content of the body for a request.

- Request Editor - Being able to edit the request being made as part of API monitoring process.

- Request Retry - Being able to retry a specific request that has been made at previous time frame.

- Request Sharing - Allow the sharing of a specific request designated for monitoring.

- Request Playback - Enable the playback of a specific request that has been made at previous time frame.

- Request Scheduling - Allow the scheduling of when to run specific task at specific time(s).

- Request Compare - Being able to compare to requests against each other.

- Request Scripting - The ability to script against a specific request.

- Request Automation - The ability to automate the running of multiple requests.

- Request Commenting - Allowing the ability to comment on a specific request.

## Import
Enabling the ability to import and export common API definitions and use them to define the monitoring across all services.

- Postman - Allow for importing using Postman Collections.

- OpenAPI Spec - Allow for importing using OpenAPI Spec.

- HAR - Allow for importing using HAR.

## Management Monitoring
Solutions for monitoring more than just the surface area of an API, and be able to also monitor the management and business aspects of services, ensuring everything you need to get up and running are available.

- Documentation Monitoring - Keeping track of changes to an APIs documentation

- Pricing Monitoring - Notifications when an API platform pricing changes

- Terms of Service Monitoring - Updates when a company changes the terms of service

## Notification
Enabling the ability to send notifications in response to monitoring activity and events as they occur using common channels that key stakeholders will be using.

- SMS - Allow notifications to be received by SMS.

- Email - Allow notifications to be received by email.

- Phone - Allow notifications to be received by Phone.

- Webhook - Allow notifications to be received by webhook.

## Reporting
Providing what is needed to properly report upon monitoring that is occurring across services, allowing for reporting to all stakeholders regarding how well services are being delivered.

- Dashboard - Providing a dashboard to review monitors.

- Embeddable - Providing embeddable tools for API monitoring.

## Targeted Monitoring
Allowing for the targeting of services from a variety of regions, demonstrating what service availability will look like across targeted regions, and around the globe.

- Provider Based Monitoring - Being able to monitor an LAPI from a particular provider.

- Region Based Monitoring - Begin able to monitor from a specific geographical region.

- Public Monitoring - Monitoring of public APIs, and providing the information for others to use.

## Utility
Some of the other utility considerations for working with the monitoring of services, and ensuring a certain quality of service at scale across all services.

- Collections - Being able to organize requests into collections.

- Virtualize - The ability to virtualize any single or group of requests.

- Localhost - Allow for executing monitoring requests using localhost.

- Teams - Enable the ability for teams to work together and share monitoring.

- API - Providing an API for API monitoring tools.

# Testing
The tactical, as well as strategic testing that is involved with each service, ensuring it is meeting service level agreements.

## Authentication
Providing a standardized approach to authentication across testing services, allowing testing processes to have the access they need to properly monitor what is happening.

- Basic Auth - Using Basic Auth, a username and password for authentication.

- OAuth - Using OAuth for platform authentication.

- API Keys - Using API keys for authentication.

## Core Details
The core aspects of operating a testing campaign across all services, ensuring that they are granularly testing and ensured they are meeting SLAs, with clear and consistent assertions that meet business goals.

- Load Testing - Offer loading testing services for HTTP endpoints.

- Response Header Inspector - Ability to inspect a response header.

- Response Body Inspector - Ability to inspect a response body.

- Request Retry - Ability to retry a specific request.

- Request Sharing - Allow for the sharing of requests.

- Request Playback - Enable the playback of a single request.

- Request Scheduling - Allow for the scheduling of requests at a specific time.

- Request Compare - Allow for the comparing of two requests.

- Request Scripting - Provide the ability to script against requests.

- Request Automation - Allow for the automation of multiple requests.

- Request Commenting - Enabling users to comment on a specific request.

- Simulator - Provide tools for simulating requests.

- Templates - Offer templates of common or specialized requests.

- Data Scenarios - Provide specific data scenarios that can be executed.

## Import
Enabling the ability to import and export common API definitions and use them to define the testing across all services.

- Postman - Allow for importing using Postman Collections.

- OpenAPI Spec - Allow for importing using OpenAPI Spec.

- HAR - Allow for importing using HAR.

## Notification
Enabling the ability to send notifications in response to testing activity and events as they occur using common channels that key stakeholders will be using.

- SMS - Allow notifications to be received by SMS.

- Email - Allow notifications to be received by email.

- Phone - Allow notifications to be received by Phone.

- Webhook - Allow notifications to be received by webhook.

## Reporting
Providing what is needed to properly report upon testing that is occurring across services, allowing for reporting to all stakeholders regarding how well services are being delivered.

- Dashboard - Providing a dashboard to review monitors.

- Embeddable - Providing embeddable tools for API monitoring.

## Targeted Testing
Allowing for the targeting of services from a variety of regions, demonstrating what service availability will look like across targeted regions, and around the globe.

- Provider Based Testing - Being able to monitor an LAPI from a particular provider.

- Region Based Testing - Begin able to monitor from a specific geographical region.

## Utility
Some of the other utility considerations for working with the testing of services, and ensuring a certain quality of service at scale across all services.

- Collections - Being able to organize requests into collections.

- Command Line Interface - Provide a command line interface for working with tests.

- Teams - Enable the ability for teams to work together and share monitoring.

- API - Providing an API for API monitoring tools.

# Performance
How is the performance of each service measured and report upon, providing a benchmark for the quality of service.

## Authentication
Providing a standardized approach to authentication across performance Testing services, allowing performance testing processes to have the access they need to properly monitor what is happening.

- Basic-Auth - Using Basic Auth for authentication.

- API Keys - Using API keys for authentication.

- OAuth - Using OAuth for authentication.

## Core Performance
The core aspects of operating a performance testing campaign across all services, ensuring that they are granularly testing and ensured they are meeting SLAs, with clear and consistent assertions that meet business goals.

- CPU Usage - Allow for the monitoring of CPU usage.

- Memory Usage - Allow for the monitoring of memory usage.

- Disk I/O - Allow for the monitoring of disk I/O.

- Network I/O - Allow for the monitoring of network I/O.

- Request Editor - Being able to edit the request being made.

- Request Retry - Allow the retry of any performance test.

- Request Sharing - Enable the sharing of performance tests.

- Request Playback - Enable the playback of any performance test.

- Request Scheduling - Enable the scheduling of performance tests.

- Request Compare - Allow for the comparison of performance tests.

- Request Scripting - Allow for the scripting againsts tests.

- Request Automation - Allow for the automation of performance tests.

- Request Commenting - Enable testers to comment on tests.

- Latency Testing - Provide latency testing tools.

- Simulator - Provide a performance test simulator.

## Import
Enabling the ability to import and export common API definitions and use them to define the performance testing across all services.

- Postman - Allow for tests to be imported using Postman.

- OpenAPI Spec - Allow for tests to be imported using OpenAPI Spec.

- HAR - Allow for tests to be imported using HAR files.

- JUnit XML - Allow for tests to be imported using JUnit XML.

## Targeted Performance
Allowing for the targeting of services from a variety of regions, demonstrating what service availability will look like across targeted regions, and around the globe.

- Region Based Testing - Allow for performance tests from specific geographic regions.

- Provider Based Testing - Allow for performance tests from specific providers.

## Utility
Some of the other utility considerations for working with the performance testing of services, and ensuring a certain quality of service at scale across all services.

- Collections - Allow performance tests to be organized in collections.

- Command Line Interface - Provide a command line interface for performance tests.

- Virtualization - Allow performance tests to be conducted against virtualized instances.

- Teams - Enable team environments for performance testing.

- API - Provide an API for integrating with all testing.

# Observability
What does observability of the service look like, providing transparency and accountability using all of its existing outputs?

## Communication
Ensuring there are appropriate communication channels open that demonstrate the desire to make operations behind services more observable and accessible to acceptable levels, sharing regular information about what is happening.

- Blog - A blog is one of the strongest signals regarding what is happening on a platform, and the motivation behind what the intent of the operators are.

- Twitter - An active Twitter account, that is dedicated to platform operations, provides a look into the real time exhaust from the regular things that are happening on a platform.

- Github - The Github account for a platform, and its operators provides a unique look into what is happening from an engineering standpoint, showing signals around what is happening.

## Monitoring
Details surround the monitoring, testing, and other elements in place to ensure that platform operators are aware of the overall platform health, and security, which demonstrates a maturity level when it comes to platform observability.

 - Testing - If a platform is actively testing, publishing and sharing these tests across teams and with the public, it demonstrates a certain level of maturity.

 - Monitoring - Actively monitoring and publishing the uptime and availability status demonstrates the maturity of platform and makes it more observable.

 - Performance - Regular performance monitoring and testing, as well as actively sharing and publishing the results with stakeholders demonstrates the observability around operations.

## Updates
Tuning into what updates are provide around platform operations, providing a look into what is being planned, what currently is happening, as well as what has occurred historically across all services.

- Road Map - A road map demonstrates that there is a plan in place, and that a service is moving forward as part of a wider strategy.

- Issues - Being open and transparent about the issues that are happening via a platform demonstrates a certain level of awareness, as well as honesty.

- Change Log - A complete and accurate lot of what has change on a platform allows for consumers to stay in tune with what has changed.

# Encryption
Details regarding what is expected regarding encryption on disk, as well as in transport for each service.

- Certificates - What certificate(s) are in place for protecting a particular service to encrypt at all levels of operations.

- Transport - Details of how everything is being encrypted in transport, protect data, content, and other details as it moves around on the web.

- Storage - The information around how everything that is being stored on disk is being encrypted by default as part of the storage across API usage.

- Database - Background on how all databases involved are being encrypted, and what the process looks like for ensuring all data is being encrypted by default.

# Security
Detailed strategy and processes regarding how each service is secured on a regular basis as part of operations.

## Overview
General details regarding the security position and practices that occur across a platform, and ensure the security of all services being made available via a platform.

- Security Practices Page - Publishing a single page that covers what the security approaches are for a platform, providing as much detail as possible about what practices are employed, what the schedule looks like, and what results of security history is.

- Security Contact - Who to contact in the event of a security incident that concerns the platform. Providing a phone number, email, or form that can be submitted.

- Denial of Service (DDOS) - DNS tools for identifying and defending against a denial of service (DOS) attack.

## Authentication Considerations
Looking at the security concerns focused in on platform authentication, and staying in sync with how authentication and authorization layers are performing as expected and not opening up the platform to malicious activity.

- Session Management - API should pass session-based authentication, either by session token via a POST or by API key as a POST body argument or as a cookie, avoiding usernames, passwords, session tokens, and API keys in the URL

- Session State - Many web services are written to be as stateless as possible, usually ending up with a state blob being sent as part of the transaction.

- Anti-Farming - APIs are regularly farmed for the data they contain, and while there's no technical method of preventing this use, having a clear business model, and API management strategy works to minimize.

- Protect HTTP Methods - Making sure the incoming HTTP method is valid for the session token/API key and associated resource collection, action, and record.

- Methods Whitelist - Properly restrict the allowable verbs such that only the allowed verbs would work, while all others would return a proper response code (for example, a 403 Forbidden).

- Cross-Site Request Forgery - Make sure any PUT, POST, and DELETE request is protected from Cross Site Request Forgery, typically done using a token-based approach.

- Insecure Direct Object References - It may seem obvious, but if you had a bank account REST web service, you'd have to make sure there is adequate checking of primary and foreign keys.

## By Force
Looking at the most common brute force approaches to breaching platform security, and ensuring they cannot be exploited to gain access to systems that are powering services.

- Brute Force Attack - A brute force attack can manifest itself in many different ways, but primarily consists in an attacker configuring predetermined values, making requests to a server using those values, and then analyzing the response.

- Cash Overflow - An attack specifically aimed at exceeding hosting costs, either essentially bankrupting the service owner or exceeding the cost limits, leading the cloud service provider to disable the application.

- Cryptanalysis - Cryptanalysis is a process of finding weaknesses in cryptographic algorithms and using these weaknesses to decipher the ciphertext without knowing the secret key (instance deduction).
Denial of Service - The Denial of Service (DoS) attack is focused on making a resource (site, application, server) unavailable for the purpose it was designed.

## Abuse of Functionality
Studying how normal functionality available via the existing services might be abused and used to gain access to data, content, algorithms, and backend systems working in the cracks to open up security holes.

- Buffer Overflow Attack - Avoid overwriting of memory fragments of the process, values of the IP (Instruction Pointer), BP (Base Pointer) and other registers which can cause exceptions, segmentation faults, and other errors to occur.

- Buffer Overflow via Environment Variables - Avoid this pattern that involves causes a buffer overflow through manipulation of environment variables, which once the attacker finds that they can modify an environment variable, they may try to overflow associated buffers.

- Overflow Binary Resource File - Coming from input data, and an Overflow Binary Resource File, where attacker modifies/prepares the binary file in such a way that the application, after reading this file, becomes prone to a classic Buffer overflow attack.

## Data Structure Attacks
Focusing in on possible data structure attacks that can occur probing and opening up holes in common backend data sources, and approaches to making data resources available.

- Cross-Site Request Forgery (CSRF) - An attack that forces an end user to execute unwanted actions on a web application in which they're currently authenticated, targeting state-changing requests, not theft of data, since the attacker has no way to see the response to the forged request.

- Logic/time Bomb - A logic bomb is a piece of malicious code that executes when specific trigger conditions are met, such as a date or time, or possible a specific database event.

- Trojan Horse - A Trojan Horse is a program that uses malicious code masqueraded as a trusted application, which is vehicle in which malicious code can be injected on benign applications, masqueraded in email links, or JavaScript.

- Account Lockout Attack - Where attackers attempts to lock out user accounts by purposely failing the authentication process as many times as needed to trigger the native account lockout functionality.

- Cross-Site Request Forgery (CSRF) - An attack that forces an end user to execute unwanted actions on a web application in which they're currently authenticated, targeting state-changing requests, not theft of data, since the attacker has no way to see the response to the forged request.

- Execution After Redirect (EAR) - Execution After Redirect (EAR) is an attack where an attacker ignores redirects and retrieves sensitive content intended for authenticated users. A successful EAR exploit can lead to complete compromise of the application. - https://www.owasp.org/index.php/Execution_After_Redirect_(EAR)

- Session Fixation - An attack that permits an attacker to hijack a valid user session, and explore a limitation in the way the web application manages the session ID, more specifically the vulnerable web application.

- Session Hijacking Attack - An attack that consists of the exploitation of the web session control mechanism, which is normally managed for a session token, exploiting http communication which uses many different TCP connections.

- Session Prediction - An attack that focuses on predicting session ID values that permit an attacker to bypass the authentication schema of an application, by analyzing and understanding the session ID generation process, an attacker can predict a valid session ID value and get access to the application.

## Embedded Malicious Code
Evaluating how malicious code might be injected into API requests looking to open up holes within services, and get behind validators, filters, and other approaches to limiting the damage that can occur by malicious activity.

- Code Injection - Attack types which consist of injecting code that is then interpreted/executed by the application, exploiting poor handling of untrusted data, and usually made possible due to a lack of proper input/output data validation.

- Command Injection - An attack in which executes arbitrary commands to the host operating system via a vulnerable application, made possible when an application passes unsafe user supplied data (forms, cookies, HTTP headers etc.).

- Comment Injection Attack - Comments injected into an application through input can be used to compromise a system. As data is parsed, an injected/malformed comment may cause the process to take unexpected actions that result in an attack.

- Content Security Policy - Open up the possibility to instruct the client browser from which location and/or which type of resources are allowed to be loaded, providing a directive that loads a behavior for a target resource type.

- Content Spoofing - An attack made possible by an injection vulnerability, where an API does not properly handle user supplied data, and an attacker can supply content, typically via a parameter value, that is reflected back to the user.

- CORS RequestPreflighScrutiny - Opening up the possibility to expose resources to all or restricted domain, made by AJAX request for resource on other domain than is source domain.

- Cross-site Scripting (XSS) - A type of injection, in which malicious scripts are injected into
otherwise benign and trusted web sites, occurring when an attacker send malicious code, generally in the form of a browser side script, to a different end user.

- Custom Special Character Injection - Not properly filtering or quoting special characters or reserved words that are used in a custom or proprietary language or representation, allowing attackers to modify the syntax, content, or commands before they are processed.

- Format String Attack - Occurring when the submitted data of an input string is evaluated as a command, allowing the execution of code, to read the stack, or cause a segmentation fault, causing behaviors that could compromise the system.

- Full Path Disclosure - Vulnerabilities enabling the attacker to see the path to the webroot/file, potentially opening up full access to the underlying system.

- Parameter Delimiter - An attack based on the manipulation of parameter delimiters used by web application input vectors in order to cause unexpected behaviors like access control and authorization bypass and information disclosure.

- Resource Injection - This attack consists of changing resource identifiers used by an application in order to perform a malicious task, allowing data to be manipulated to execute or access different resources.

- Server-Side Includes (SSI) Injection - An attack that allows the exploitation of a web application by injecting scripts in HTML pages or executing arbitrary codes remotely, exploiting through the manipulation of SSI in use and force its use through user input fields.

- SQL Injection - The insertion of a SQL query via the input data allowing the reading sensitive data from the database, modify database data, execute administrative tasks, and in some cases issue commands to the operating system.

- Web Parameter Tampering - An attacked based on the manipulation of parameters exchanged between client and server in order to modify application data, such as user credentials and permissions, price and quantity of products, etc.

- XPATH Injection - An attack occurring when a web site uses user-supplied information to construct an XPath query for XML data, sending malformed information to an API opening up how the XML data is structured, or access data.

## Input Validation
Scrutinizing how information is inputted through existing parameters, and body requests being made of services, and looking for better ways to validate what is imputed and being injected as part of request

- Validate Content-Types - The server should never assume the Content-Type; it should always check that the Content-Type header and the content are the same type.

- Assist the User - Assisting in the input of high quality data into APIs, by validating what is submitted, and rejecting anything that does not pass validation.

- Secure Parsing - Use a secure parser for parsing the incoming messages. If you are using XML, make sure to use a parser that is not vulnerable to XXE and similar attacks.

- Strong Typing - It's difficult to perform most attacks if the only allowed values are true or false, or a number, or one of a small number of acceptable values. Strongly type incoming data as quickly as possible.

- Validate Response Types - Do NOT simply copy the Accept header to the Content-type header of the response, and reject the request if the Accept header does not specifically contain one of the allowable types.

- JSON Validation - Making sure all JSON is valid helps make sure that APIs are operating as expectation and making sure vulnerabilities are not being passed in with API requests and responses.

- XML Validation - XML-based services must ensure that they are protected against common XML based attacks by using secure XML-parsing.

- Framework-Provided Validation - Many frameworks allow for validation constraints to be enforced automatically by the framework at request or response time, providing automatic validation before the data is delivered to the application.

## Output Validation
Looking at how API requests are validated for accuracy, and do not possess any secrets, or other information that might be used to compromise the services, and systems that are behind them.

- Send Security Headers - The server should always send the Content-Type header with the correct Content-Type, and preferably the Content-Type header should include a charset.

- JSON Encoding - Use a proper JSON serializer to encode user-supplied data properly to prevent the execution of user-supplied input on the browser.

- XML Encoding - Do not assemble XML string concatenation, rather us a XML serializer, ensure that the XML content sent to the browser is parseable and does not contain XML injection.

- Link Integrity - Checks the reputation of web links in real time, providing an invisibly secure experience by blocking malicious and unwanted links from being present or loading in content.

## Transport Level Security
Diving deeper into transport level security and understand the security concerns as services are being delivered, and thinking about how information could be exploited, rerouted, and illegally obtained.

- Data in Transit - Unless the public information is completely read-only, the use of TLS should be mandated, particularly where credentials, updates, deletions, and any value transactions are performed.
Path Traversal Attack

- HTTP Request Smuggling - The HTTP Request Smuggling attack explores an incomplete parsing of the submitted data done by an intermediary HTTP system working as a proxy.

- HTTP Response Splitting - Occurs when data enters a through an untrusted source, most frequently an HTTP request, included in an HTTP response header sent to a web user without being validated for malicious characters.

- Traffic Flood - A type of DoS attack that explores the way that the TCP connection is managed, with the generation of a lot of well-crafted TCP requisitions, with the objective to stop the Web Server or cause a performance decrease.

## Protocol Manipulation
Understanding the common ways in which protocols can be manipulated to open up security holes and allow for bad actors to obtain access to data, content, algorithms and other resources behind services.

- Comment Injection Attack - Comments injected into an application through input can be used to compromise a system, where data is parsed, an injected/malformed comment may cause the process to take unexpected actions that result in an attack.

- Custom Special Character Injection - Not properly filtering or quoting special characters or reserved words that are used in a custom or proprietary language or representation, allowing attackers to modify the syntax, content, or commands before they are processed.

- Double Encoding - Encoding user request parameters twice in hexadecimal format in order to bypass security controls or cause unexpected behavior from the application.

- Forced Browsing - An attack that enumerates and opens up access to resources that are not referenced by the API, allowing the discovery unlinked contents in the domain directory, such as temp directories and files, and configuration files.

- Path Traversal - A Path Traversal attack aims to access files and directories that are stored outside the web root folder, by browsing the application, the attacker looks for absolute links to files stored on the web server.

- Relative Path Traversal - This attack is a variant of Path Traversal and can be exploited when the application accepts the use of relative traversal sequences such as ../.

- Repudiation Attack - A repudiation attack happens when an application or system does not adopt controls to properly track and log users' actions, thus permitting malicious manipulation or forging the identification of new actions.

- Setting Manipulation - The modification of settings in order to cause misleading data or advantages on the attacker's behalf, manipulating values in the system and manage specific user resources of the application or affect its functionalities.

- Unicode Encoding - Opening up of flaws in the decoding mechanism implemented by decoding Unicode data format, allowing for encoding of certain characters in the URL to bypass filters, thus accessing restricted resources.

## Resource Depletion
Evaluating how resources can be depleted, making sure security efforts aren't overlooking smaller, low-level, more precise attacks that might easily go unnoticed because of their scope.

- Cash Overflow - An attack specifically aimed at exceeding hosting costs, either essentially bankrupting the service owner or exceeding the cost limits, leading the cloud service provider to disable the application.

- Cross-Site Request Forgery (CSRF) - An attack that forces an end user to execute unwanted actions on a web application in which they're currently authenticated, targeting state-changing requests, not theft of data, since the attacker has no way to see the response to the forged request.

- Man-in-the-Middle Attack - The interception of communication between two systems, where once the TCP connection is intercepted, the attacker acts as a proxy, being able to read, insert and modify the data in the intercepted communication.

## Threats
Identifying the ways in which additional threat data and intelligence can be obtained and aggregated alongside platform information, providing more data points for defending a platform and its services.

- Threat Analysis - Providing systems that will automate the analysis of threats to DNS.

- Threat Intelligence - Give access to the actual intelligence behind threats to DNS.
Whitelist / Blacklist - Being able to establish whitelists and blacklists of domains, IP addresses, and other criteria for DNS level defense.

## General Considerations
Some of the other general considerations when it comes to security services, and ensuring that platform security is properly defended, and bad actors are kept outside the API perimeter.

- Certification - Providing a system for validating and certifying an APIs security, scanning the surface area and providing guarantees that the endpoint(s) are secure.
- Security Visualization - Allowing API owners with reports and charting, allowing them to visualize the surface area and security of an API. Providing a single way to see all the potential attacks, vulnerabilities, and what is being done about security overall.

- Compliance & Auditing Reporting - Providing a specific interface for auditors and compliance officers to see what security has been applied to any interface. The reporting should provide details that are in alignment with whatever standard is being applied to the industry, as well as standard security approaches.

- Bug Bounty Program - Provide a platform for running a bug bounty program, that allows API providers to crowdsource the discovery, and review of an API, providing a potentially friendly way to handle security before bad actors can step in and find vulnerabilities.

- Endpoint Tagging - Allow for the tagging and organizing of APIs into specific groups for scanning, monitoring, and reviewing of APIs. Giving providers an easy way to organize so that they can be secured, and understood.

- Intrusion Correlation - Providing the ability to connect the dots between various security attacks and intrusions, providing insight into patterns used by attackers, locations of attacks, and other details that might help security.

- Risk Scoring - Offer a single scoring approach to be able to score attacks, based upon existing understanding of the space, but also historical data, providing a clear way to rank, and understand how vulnerabilities, and attacks could affect operations.

# Terms of Service
Considerations, and legal requirements applied to each service as part of the overall, or individual terms of services.

## Overview
The overview of the terms of service, providing a single place where stakeholders can find all legal documents governing the services available via the platform.

- Terms of Service Page - Providing a single page dedicated to providing a listing of elements that impact terms of service for developers and end-users.

## Key Considerations
Some of the key considerations when it comes to the terms of service that are governing how the services can and cannot be put to use within applications.

- Sites Covered - What sites are covered by the terms of use. Even if there is a single, provide a basic reference to the domain. If there are multiple domains, make sure and list them. Also consider subdomains that might be a consideration.

- Opting Out - What are the possibilities for opting out of services? Are there data sharing, licensing, or communication areas that can be opted out, or NOT opted out of.

- Pay For Changes - Can API consumers pay to get any aspects of terms of services adjusted?

## Data & Information
Looking at how the terms of service covers aspects of accessing and ownership of data, governing how platform information can be put to use within applications and other systems.

- How We Use Your Information - Be clear about how information is used. Is it only used as part of operations. Provide straightforward explanations of how information is put to work to power the platform.

- Personal Information - What personal information is collected, stored, shared, and put to use? What are the security procedures, and other considerations for dealing with privacy of users personal information.

- Non-Personal Information - What are the considerations for all other content and data areas. This not personally identifiable information, but everything else.

- Aggregate Information - What information is aggregated, and what are the considerations when it comes to the platform terms of service.

- Access To Information - What levels of access are there. Is everything available via APIs or downloads, or are there restrictions around what you can get access to.

- Accuracy of Information - What are the expectations for accuracy of information available via the platform. What is the bar, and how is this level determined and enforced.

## Information Storage
Providing guidance on how information that is obtained through services can be stored, including logging of API requests and responses, and the resulting data, content, and algorithmic output.

- Caching - Information regarding how data can be cached as part of usage within the web and mobile applications where the data and content is being made available.

- Log Files - Providing some details on how log files are used in platform operations, what is logged, and what isn't, and how things are collected, retained and shared.

## Tracking Used
Legal details about what tracking is used, providing observability into what data points are tracked for users, and governing how developers can be tracking users activity.

- Geo Guidelines - Providing an overview of considerations when it comes to location, and geo tracking via the platform.

- Cookies - What are the cookie policies? How are cookies crafted, stored, and deprecated. Cover the cookie policies for a platform, and any connection to the API.

## Sharing Approaches
Details regarding how data and content is being shared by the platform, as well how developers are expected to share or not share valuable resources being made available via services.

- Web Beacons - Are web beacons in use? Are they return as part of API operations, and possibly required in all web and mobile deployments

- Partner Resources - Are there any members-only and partner specific opportunities, and how do these different levels of access impact terms of service.

- Information Sharing - How is information shared with partners, government, and any potentially external partners. Does this occur via the API, and how does this affect terms of service.

## Concerns For Minors
The legal details regarding how platform operations can be used to serve minor children, providing a set of guidance regarding how this will impact API operations.

- Children's Privacy Overview - Are there any special considerations for children's privacy. Will minors potentially be using the system, and what areas should be considered?

- Children's Online Privacy Protection Act (COPPA) - Congress enacted the Children’s Online Privacy Protection Act (COPPA) in 1998. COPPA required the Federal Trade Commission to issue and enforce regulations concerning children’s online privacy.

## Linking To Other Sites
Legal guidance regarding how external domains are linked as part of platform operations, and guidance for how developers should be linking within their applications.

- Links to Non-Operators Web Sites - What are the levels of responsibility and liability when it comes to external links made available through platform operations.

## Services
The legal side of the terms of service that impacts specific services and their availability, providing what can be legally expected when it comes to putting services to work.

- Service Level Agreement - Provide a service level agreements (SLA) describing what service(s) are offered by an API provider, with details about the quality of service, and ​warranties, disaster recovery, and steps for termination of agreement.

- Deprecation Policy - Provide a API deprecation policy setting expectations with API consumers about when and how API resources will be deprecated and shut down.

## Monetization
The terms of service guiding how money can be made by developers who are putting services to use, setting the bar for how revenue is generated around platform resources.

Monetization Guidelines - Providing legal guidelines for how developers can monetize around resources that are available via an API.

## Corporate
The legal details regarding the corporate entities involved with platform operations, and responsible for the services being made available.

- Trademarks - Providing a reference to​ corporate trademarks that are part of API operations, and developers may have to consider.

## Regulation
Any legal disclaimers regarding regulatory and compliance aspects of operating the platform, providing the required disclosures in service of government oversight.

- Compliance - A page providing compliance related information, covering how a company, platform, and APIs complies with government and industry regulations.

# Privacy
Details regarding the privacy of platform owners, developers, and end users as it pertains to service usage.

## Data & Information
Understanding how privacy needs to be respected as data and information flow through, and is gathered as part of each service, covering the legal aspects of privacy is respected.

- Use of Personally Identifiable Information - Linking to the same area in terms of service, how is privacy considered when personally identifiable information is put to use. Lay out what is considered in this area.

- User Submissions - What is the general view of user submissions, and user generated content and data. Is it core to platform operations, and what is the general tone of users and API consumers access and ownership of this exhaust.

- User Discussion Lists and Forums - What privacy considerations have been made around discussion lists and forums operated by the platform? What data is stored? How is the privacy of users addressed?
Legal Department

- License - What licensing considerations are there that could potentially impact the privacy of platform owners, consumers, and end-users.

- Intellectual Property Rights - Where does intellectual property rights come into play, that could potentially impact the privacy of platform owners, consumers, and end-users.

- Liability - What is the liability assumed by the platform, or possibly consumers, and end-users when it comes to platform operations, in the area of privacy.

- Warranty Disclaimer - A disclaimer is a defensive measure, used generally with the purpose of protection from unwanted claims or liability. A platform may disclaim responsibility for loss or damage to a customer's Personal Property, or a disclaimer clause in a contract might set forth certain promises and deny all other promises or responsibilities.

## Platform Changes
Talking through the legal side of how changes will be made, and privacy will be considered as the platform changes and versions are released throughout the road map.

- Termination - What privacy considerations are taken when accounts are terminated. Can users, and API consumers terminate their relationship and assume that privacy is respected.
Changes - How may changes to the platform, APIs, and how data is collected and stored that may impact privacy.

## Site Linkage
Talking about how links are handle, and privacy is considered as part of the linkage that will occur throughout data and content being made available via the platform.

- Links to Other Materials - What are the privacy considerations when external sites and materials are linked to.

- Short Code Usage - Details about proxying with short codes, and how this information is tracked, and shared across service operations.

## Technical Details
Speaking to the technical details, limitations, and implications on privacy, and how those are addressed, communicated, and shared.

- Technical Requirements and Limitations - What are the technical requirements and limitations that impact the privacy of platform owners, consumers, and end-users.

## Usage of Service
Thinking about the tradeoffs between the terms of service and privacy, linking sensible usage of the platform, respecting privacy, and being able to use the service or not.

- Permitted and Prohibited Uses - What are the permitted uses of data and content made available via the APIs, and what are some of the common prohibited uses that impact the privacy of users and platform owners.

# Service Level Agreements
Details regarding what service levels are required to be met when it comes to partner and public engagements.

- Commitment - Details about a platforms commitment and philosophy around providing a SLA, and what it means to the level of service.

- Downtime - Details that describe what downtime means, and how it is measured and quantified as part of making sure services meet a certain level of availability.

- Downtime Period - Information regarding how downtime duration and length are measure, quantified, and reported upon as part of availability.

- Monthly Uptime Percentage - Information regarding how the monthly uptime percentage is calculated and reported upon regularly as part of SLA reporting.

- Scheduled Downtime - Details regarding how scheduled downtime is factored in as part of ensuring an SLA is being met, and how preparations and communication occurs.

- Domain - Details regarding how service level agreements are broken down by domain, separating availability and concerns by domain.

- Service - Information about how different services are broken down as part of the service, and the SLA is being applied in different ways.

- Service Credit - When an SLA is not met, how are accounts being credit due to service outages, and downtime, hold the platform accountable for reliability.

- Exclusions - Outlining any exclusions in place regarding the applying of SLA across the platform, and what won't be considered an outage.

- Support - Details regarding how the service level agreement is communicated to new users, as well as with existing users, as changes are made, or incidents occur.

# Licensing
Information about backend server code, API surface area, data, and client licensing in play.

## API
What does the licensing look like for the surface area of the API, not the underlying code or client tool, but the naming and ordering of the interface involved with integrating with any service.

- Attribution (CC BY) - This license lets others distribute, remix, tweak, and build upon your work, even commercially, as long as they credit you for the original creation. This is the most accommodating of licenses offered. - http://creativecommons.org/licenses/by/4.0/

- Attribution-ShareAlike (CC BY-SA) - This license lets others remix, tweak, and build upon your work even for commercial purposes, as long as they credit you and license their new creations under the identical terms. This license is often compared to copyleft free and open source software licenses. All new works based on yours will carry the same license, so any derivatives will also allow commercial use.

- Public Domain (CC0) - Use this universal tool if you are a holder of copyright or database rights, and you wish to waive all your interests in your work worldwide. - https://creativecommons.org/about/cc0

## Client Code
What does the licensing look like when it comes to the client side code that is provided on top of APIs, and shared with consumers for integrating with services.

- Apache - The Apache License is a free software license written by the Apache Software Foundation (ASF). The Apache License requires preservation of the copyright notice and disclaimer. Like other free software licenses, the license allows the user of the software the freedom to use the software for any purpose, to distribute it, to modify it, and to distribute modified versions of the software, under the terms of the license, without concern for royalties. - http://www.apache.org/licenses/LICENSE-2.0

- GPL - The GNU General Public License (GNU GPL or GPL) is the most widely used[6] free software license, which guarantees end users (individuals, organizations, companies) the freedoms to run, study, share (copy), and modify the software. Software that allows these rights is called free software and, if the software is copylefted, requires those rights to be retained. - http://www.gnu.org/licenses/gpl-3.0.en.html

- MIT - The MIT License is a free software license originating at the Massachusetts Institute of Technology (MIT). It is a permissive free software license, meaning that it permits reuse within proprietary software provided all copies of the licensed software include a copy of the MIT License terms and the copyright notice. - https://opensource.org/licenses/MIT
Content

- Attribution (CC BY) - This license lets others distribute, remix, tweak, and build upon your work, even commercially, as long as they credit you for the original creation. This is the most accommodating of licenses offered. - http://creativecommons.org/licenses/by/4.0/

- Attribution-ShareAlike (CC BY-SA) - This license lets others remix, tweak, and build upon your work even for commercial purposes, as long as they credit you and license their new creations under the identical terms. This license is often compared to copyleft free and open source software licenses. All new works based on yours will carry the same license, so any derivatives will also allow commercial use. - http://creativecommons.org/licenses/by-sa/4.0

- Public Domain (CC0) - Use this universal tool if you are a holder of copyright or database rights, and you wish to waive all your interests in your work worldwide. - https://creativecommons.org/about/cc0

## Data
Looking at licensing at the data layer, and understanding how data is licensed and made available via APIs, and the services they are powering.

- Public Domain Dedication and License (PDDL) - The PDDL places the data(base) in the public domain (waiving all rights).

- Attribution License (ODC-By) - You are free to share, create, and adapt, as long as you attribute the data source.

- Open Database License (ODC-ODbL) - You are free to share, create, and adapt, as long as you attribute the data source, share-aloe, and keep open.

## Server Code
Considering how server-side code is licensed, and made available beyond just driving the API, and looking at how it can make APIs deployable and federated at scale.

- Apache - The Apache License is a free software license written by the Apache Software Foundation (ASF). The Apache License requires preservation of the copyright notice and disclaimer. Like other free software licenses, the license allows the user of the software the freedom to use the software for any purpose, to distribute it, to modify it, and to distribute modified versions of the software, under the terms of the license, without concern for royalties. - http://www.apache.org/licenses/LICENSE-2.0

- GPL - The GNU General Public License (GNU GPL or GPL) is the most widely used[6] free software license, which guarantees end users (individuals, organizations, companies) the freedoms to run, study, share (copy), and modify the software. Software that allows these rights is called free software and, if the software is copylefted, requires those rights to be retained. - http://www.gnu.org/licenses/gpl-3.0.en.html

- MIT - The MIT License is a free software license originating at the Massachusetts Institute of Technology (MIT). It is a permissive free software license, meaning that it permits reuse within proprietary software provided all copies of the licensed software include a copy of the MIT License terms and the copyright notice. - https://opensource.org/licenses/MIT

# Branding
What branding requirements are in place for the platforms and its partners when it comes to the service, and what is expected of consumers when it comes to supporting the branding of the platform.

## Assets
Providing a list of assets and related resources that can be used to supporting branding guidelines, and wider corporate branding efforts.

- Image Assets - What image assets are available to support and encourage branding efforts by API consumers? Could be logos, all the way to banners--anything image related that supports branding.
- Icon Assets - What image icon assets are available to support and encourage branding efforts by API consumers? Could be logos, all the way to banners--anything image related that supports branding.
- Other Assets - What other assets are available at your company that you use to help guide internal branding strategies, that maybe you could repurpose, and share with the developer community, helping them be more successful in representing your brand.

## Guides
What branding guides are available to provide guidance for platform consumers when it comes to protecting the brand of the platform and its partners.

- Branding Examples - What are some existing examples of how brand can be used. Are there samples, or actual case studies of existing integrators that can show how branding is done properly, or maybe done improperly.

- Full Style Guide - Is a full style guide available, using in PDF or HTML format that API consumers can use to understand all branding and style guidelines?
Overview

- Give Credit - Explaining to API consumers that they should give credit where appropriate, and use common sense when it comes to integrations and giving proper credit to value generated via the API.

- Bring Value - Explaining to API consumers that they should bring value to the platform, and not extract more value than they create. Demonstrating that this balance is needed, to make the API integration relationship work.

- Use of Brand Name - How should API consumers understand when it comes to using brand names in their tools, services, and any materials they produce to support their work.

- Use of Brand Logo - How should API consumers understand when it comes to using logos in their tools, services, and any materials they produce to support their work.

- Use of Product Titles - How should API consumers understand when it comes to using product titles in their tools, services, and any materials they produce to support their work.

- Naming Your Application - What are the considerations when an API consumers is naming their application that is build on top of an API? Are there any reserved words, or things consumers should be considering?

## Requirements
Providing clear requirements regarding what is required of API consumers when it comes to displaying logos, providing links, and following other branding and image guidelines.

- Content Display Requirements - What are the considerations for how content can be displayed. Any restrictions or considerations for displaying within web and mobile applications.

- Data Display Requirements - What are the considerations for how data can be displayed. Any restrictions or considerations for displaying within web and mobile applications.

- Linking Requirements - What are your linking requirements? Along with images and other assets, what URLs should be attributed to as part of the process. Make the instructions clear and simple, with all URLs easily available, throughout all assets, and branding related tooling.

# Regulations
Information regarding regulations in place that effect service operations, and are required as part of its usage.

- Laws - What laws are in place that impact how APIs should operate, and needed to be paid attention to as part of the lifecycle to ensure everything is compliant.

- Definitions - Are there schema or API definitions in place that need to be used as part of the development process, which are part of regulatory compliance.

- Reviews - Are there regular reviews that need to occur to ensure that a service is in compliance with regulatory guidance, that might impact the lifecycle of a service.

- Regions - What regions are available and required to use as part of regulatory constraints, or part of customer requirements that are driven by regulations.

# Discovery
How are services catalogued and made discoverable, making them accessible to other systems, developers, as well as to internal, partner, or public groups.

## API Definition Formats
Providing machine readable API definitions that support the discovery of APIs, as well as the supporting API operations around them.

- APIs.json - Use the APIs.json JSON specification for describing collections of APIs, allowing them to be indexed for inclusion in public and private search engines.
- OpenAPI - Providing a complete, machine readable definition using the JSON or YAML format from the OpenAPI Initiative.

## API Directories
Making sure APIs are available in the common public API directors available, allowing public APIs to be discovered by new users searching these directories.

- ProgrammableWeb - The original API directory created by John Musser in 2005, to provide a single, searchable directory of common public APIs.

- RapidAPI - A public API directory, formerly known as Mashape, but has been rebranded as RapidAPI, providing a directory of popular API programs.

- APIs.guru - A public API directory running on Github, with a public catalog for searching and browsing, as well as a way for API providers to submit a pull request with their complete OpenAPI, for inclusion in the directory.

## API Search Engines
Considering the newer API search engines that allow for easy submission of new APIs using a machine readable APIs.json format.

- APIs.io - APIs.io is an open source search, driven using the APIs.json discovery format, allowing API providers to manage the discovery index of their own APIs, while allowing consumers to search, discover, and build collections of APIs they use.

## Business Directories
Rather than focusing just on the API, but consider listing the business behind the API in common business directories, and tagging as having an API focus.

- Crunchbase - A directory of companies that is curated by Techcrunch, and allows an approach to listing companies who have APIs.

- AngelList - Like Crunchbase, AngelList is a directory of companies, but also provides a way to showcase companies who have APIs.

## How Are APIs Found?
Thinking about how APIs are found within an organization or industry, and helping make sure that APIs can be organized and found by internal, partner, and public consumers.

- API Directory - API directories allow for the submissions and curation of APIs, then enable users to search and browse by keywords and tags, in many areas.

- API Hub - API directories usually span many categories, where hubs often focus on specific area like telco, or healthcare, providing a single hub for discovering APIs.

- IDE Extension - integrated development environment (IDE) extensions or add-ons that allow developers to quickly discovery and understand API endpoints.

- API Explorer - Sometimes also called consoles are designed to provide an interactive interface for developers to discover, explore, make calls and see responses in an interactive way.

# Client
Information about clients being used to interface with and work with the service, allowing it to be put to use without code.

## Authentication
Ensuring that clients have the ability to support and connect using common authentication schemes, making sure they can work with the most available APIs out there.

- Basic Auth - Basic Auth is supported by an HTTP client for authentication as part of ay request being made.

- API Keys - API keys is supported by an HTTP client for authentication as part of ay request being made.

- Digest Auth - Digest Auth is supported by an HTTP client for authentication as part of ay request being made.

- OAuth 1.0 - OAuth 1.0a is supported by an HTTP client for authentication as part of ay request being made.

- OAuth 2.0 - OAuth 2.0 is supported by an HTTP client for authentication as part of ay request being made.

## Environment
Brining common definitions of the environments that will be needed to work with many different APIs, allowing for a common way to authentication, and pass key values to each API being integrated with.

- Separate Environments - The HTTP client allows for establishing of separate environments to make requests to APIs in different modes.

- Saved Variables - Allow for naming and saving of variables that can be used across API requests, in separate environments.

## Import / Export
Enabling the import and export of common API definitions into an API client and allowing for API definitions to be used across the API lifecycle, and when leveraging a client to work with APIs.

- Import OpenAPI Spec - Allow for the importing of API requests using the OpenAPI Spec.

- Import API Blueprint - Allow for the importing of API requests using the API Blueprint API definition format.

- Import Postman - Allow for the importing of API requests using the Postman API definition format.

- Export Postman - Allow for the exporting of API requests using the Postman API definition format.

- Export OpenAPI Spec - Allow for the exporting of API requests using the OpenAPI Spec.

- Export API Blueprint - Allow for the exporting of API requests using the API Blueprint API definition format.

## Organization
Enabling the organization of definitions, collections, templates and other artifacts that can be used to integrate and put services to use at the client level.

- Collections - Allow for requests to be saved, and stored into collections that can be named,
organized and managed in meaningful groups.

- Templates - Provide starter templates of common public APIs, allowing HTTP client to be immediately put to use from common definitions.

- Clone Requests - Enable the HTTP client to clone existing requests, and generate new collections or requests from existing definitions.

- Record - Allow for any saved request to be recorded, for playback later.

- Replay - Allow for the replay of any saved requests that has been run and recorded.

- Keyboard Shortcuts - Provide keyboard shortcuts, that make working with HTTP client requests easier.

- History - Provide a historical listing of API requests that have been made, allowing the history to be searched, reviewed, and managed.

- Teams - Provide team environments, allowing users to collaborate, share and work across API requests, and collections.

## Request Editor
Allowing for the easy editing and working with client request made, providing an environment where integration can safely occur without actually writing code, and help consumers develop a better sense of the requests they are making.

- Request URL Editor - Having full control to edit any part of the URL for any request being made through the client.

- Request Headers Editor - Being able to add, edit, and remove any headers that will be sent with any request being made through the client.

- Cookies Manager - Being able create, edit, and remove cookies that control any session of a request being made through the client.

- Request Method Manager - Allowing for the use of all HTTP verbs, identify each method that is being made as part of a request through the client.

- Request Body Editor - The ability to add, edit, or remove the entire body of a request being made through the client.

## Response Viewer
Providing the ability to easily work with API responses, and enable the consumer to make sense of the moving parts of each request, and easily see and understand what has been returned without writing code.

- Save Requests - Allow individual requests to be saved, and run again in the future with the saved configuration.

- XML Viewer - Provide a viewer for seeing the XML returned, and be able to copy, paste, save, and other features.

- JSON Viewer - Provide a viewer for seeing the JSON returned, and be able to copy, paste, save, and other features.

- RAW Viewer - Provide a viewer for seeing the raw response returned, and be able to copy, paste, save, and other features.

- Search - Allow the searching of results, by keyword and key phase, returning the point in results that match search.

## Tooling
Providing additional client tooling that helps consumers make sense of the integration with services and be able to enhance the API integration cycles.

- Command Line - Provide a command line interface for developers to use along with an HTTP client.

- Codegen - Enable the generation of client code samples from API definitions within the HTTP client.

- Proxy - Provide a proxy that can be used when making requests via the HTTP client.
Extensions - Allowing the extension of an HTTP client using a standardize plugin interface.

# Command Line Interface
The command line interface (CLI) tooling being used to developer or consume a service, and integration within larger pipelines, models, and lifecycle implementations.

- Options - Providing a list of the available command line interface options that can be applied to commands and put services to work on the platform.

- Commands - Providing a list of the available commands that can be applied to commands and put services to work on the platform.

- Parameters - Providing a list of the available command line interface parameters that can be applied to commands and put services to work on the platform.

- IAM - Defining the identity and access layer via the CLI, including the login and authorization to the interface, as well as with existing services and backend systems.

- Web Browser Access - Provide command line interface access in the browser, offering a shell that can be accessed anywhere and put services to work via the web CLI.

- Virtual Instances - Offer the ability to scale up, and increase the scope of virtual instance that is powering any single command line service connection and command being executed.

- Persistent Storage - Providing persistent storage that is accessible via the command line interface, allowing for storing of commands, and results of executed commands.

# SDKs
What software development kits (SDK) are generated, or developed and maintained as part of a service’s operation? Providing the code samples, libraries, and development kits that are needed to put services to use.

## Overview
Giving an overview of what is available when it comes to supporting client side code for all services, providing a single location for all consumers to get the code resources they need for successful integrations.

- Overview - Providing a single page with overview of samples, libraries, or SDKs.
Beta - Provide a beta program as part of language, mobile, or platform SDKs.

- Crash Reporting - Provide tooling and services to assist with crash reporting within language, mobile, or platform SDKs.

## Language SDKs
What programming languages are available when it comes to software development kits (SDK), providing a suite of client code for developers to find the kit that speaks to them, and the environment they are used to working in.

- PHP - An SDK available in the PHP programming language, with consideration specifically tailored for the language.

- Python - An SDK available in the Python programming language, with consideration specifically tailored for the language.

- Ruby - An SDK available in the Ruby programming language, with consideration specifically tailored for the language.

- Node.js - An SDK available in the Node.js programming language, with consideration specifically tailored for the language.

- C Sharp - An SDK available in the C Sharp / C# programming language, with consideration specifically tailored for the language.

- Java - An SDK available in the Java programming language, with consideration specifically tailored for the language.

- Go - An SDK available in the Go programming language, with consideration specifically tailored for the language.

- Scala - An SDK available in the Scala programming language, with consideration specifically tailored for the language.

## Mobile Solutions
What SDKs are available that enable mobile application development, providing the code needed to quickly deliver mobile applications on top of available services.

- Mobile Overview - An overview page, dedicated to mobile application development, giving equal time to each platform, including iOS, Android, and Windows.

- iOS SDK - Providing mobile-focused SDKs for developers to build IOS mobile applications on top of an API.

Android SDK - Providing mobile focused SDKs for developers to build Android mobile applications on top of an API.

- HTML5 - Providing mobile focused SDKs for developers to build HTML5 mobile applications on top of an API.

## Browser Development Kits
What assistance is available for helping API consumers integrate services into the browser, making APIs easily integrated into the leading browsers using their extension and add-on capabilities.

- Chrome Extension - Providing ready to go Google Chrome browser integration, allowing developers, and sometimes even non-developers to immediately put an API to use in their browser, with a Google Chrome extension.

- Firefox Add-On - Providing ready to go Mozilla Firefox browser integration, allowing developers, and sometimes even non-developers to immediately put an API to use in their browser, with a Mozilla Firefox add-on.

## Platform Development Kits
What other 3rd party platforms are invested in when it comes to provide read to go code for integration, significantly speeding up the time it takes for an API consumer to deploy an application via popular platforms.

- Wordpress - Providing ready to go WordPress integration, allowing developers, and sometimes even non-developers to immediately put an API to use through their WordPress site(s).

- Heroku - Providing ready to go Heroku integration, allowing developers, and sometimes even non-developers to immediately put an API to use through their Heroku platform account.

- Drupal - Providing ready to go Drupal integration, allowing developers, and sometimes even non-developers to immediately put an API to use through their Drupal site(s).

- SalesForce - Providing ready to go SalesForce integration, allowing developers, and sometimes even non-developers to immediately put an API to use through their SalesForce account.

- Joomla - Providing ready to go Joomla integration, allowing developers, and sometimes even non-developers to immediately put an API to use through their Joomla account.

- Google App Engine - Providing ready to go Google App Engine integration, allowing developers, and sometimes even non-developers to immediately put an API to use through the Google Cloud platform.
Single Page Applications (SPA)

- Angular.js - Providing developers with AngularJS framework integration, allowing them to build single page applications using API resources.

- React.js - Providing developers with React.js framework integration, allowing them to build single page applications using API resources.

## Monetization Development Kit (MDK)
Beyond just the technical, what code is available to help API consumers monetize their applications, and generate revenue as part of their integration, helping create sustainable applications?

- Advertising Development Kit (ADK) - Providing a toolkit for integrating advertising opportunities directly into language, mobile, and platform development kits.

## Import / Export
What options are available for generating SDKs or other types of code from the machine readable definitions that are present for each service, helping API consumers tackle much of the busy work of client integrations.

- Import OpenAPI Spec - Allow for importing of API definitions using OpenAPI specification format, for generation of SDKs.

- Import Postman - Allow for importing of API definitions using Postman format, for generation of SDKs.

## Discovery
Identifying resources and challenges with helping developers find the SDKs, and other code libraries they are needed. Providing a common approach to indexing, cataloging, reviewing, and making API resources available.

- List SDK - Are SDKs listed in an easy to find location, where developers can browse them easily? A simple list goes a long way in making them found.

- Search SDK - Is there the ability to search for SDKs, using a single index dedicated to them, or possibly using Github's already available search mechanisms.

- Browse SDK - Is there a browsable directory of SDKs, that developers can use to find the SDK that they need? Potentially giving more information than just a listing.

- Rating - Are SDKs rated, allowing for various quality considerations around their value and usage in other API integrations, allowing developers to find the best SDKs possible.

# Plugin
What platform plugins are developed and maintained as part of a services operations, allowing it to work with other platforms and services.

- SDK - The details of how plugins should be designed, developed, deployment and managed, with exit code, documentation other resources to deliver platform plugins.

- Builder - The details about a service or tool that helps people craft new plugins that can be used via an API platform, eliminating the need to write code.

- Directory - The location where all plugins are published for private or public consumption, allowing platform users to find new plugins, and turn on as part of their platform usage.

- Management - The place where platform users can go to manage the platforms they have activated, allowing them to configure the details of how it works, as well as remove plugins no longer wanted.

# IDE
Are there integrated development environment (IDE) integrations, libraries, plugins, or availability considerations for each service?

## Workbench
Providing a common workbench within an IDE that helps developers build their projects, bring in the services they need, and effectively work on the integrations that matter to them and their teams.

 - Workspace - Workspace definition tooling and services, allowing APIs to be an integrated part of the IDE workspaces, either by default or custom addition.

 - Project - Allowing developers to break up API development into specific projects, providing well defined, project focused organization for API integration.

 - Environment - Is there the option for establishing separate environments within an IDE. Are developers able to segment and group their API integrations into multiple environments.

 - Autocomplete - One of the hallmark features of an IDE, is autocomplete for specific languages and frameworks. In this scenario autocomplete is focused on dictionaries created by API definitions, meant for specific integrations.

## Backend
Providing backend services for development environments allowing for the scaling up of jobs, workers, and other elements involved with compiling, working with, and executing the services available via a platform.

 - Worker - Are there options for creating specific works, that allow specific API integrations to be established, and run in isolation as specific workers or jobs.

 - Container - Are there options to be able to containerize individual API integrations, isolating them into specific virtualized instances.

## Configuration
Providing a rich environment for allowing each developer to customize and configure their development environment making it work with their way of doing things, while also following a common set of patterns used across teams.

- Editor(s) - Are there options for multiple editors, depending on media or file type, or possible set per project and environment levels, within the IDE.

 - Themes - Are there theme options, allowing the environment, workspace, and projects to be custom defined by stored themes.

## Extending
Allowing developers to extend and evolve their development environments through plugins, scripts, and other modules that are designed to augment and extend what is happening at integration and application development time.

 - Github - Using Github as a source for code, templates, definitions, and other essential building blocks of the API development process, in a modern IDE.

 - Plugins - Does the IDE environment allow for plugins, and extending the environment? Plugins allow for the introduction of 3rd party tools and services into the IDE workspace.

 - Customize - Are there options for customizing the IDE, from look and feel, to the functionality.

## Awareness
Providing as much awareness within the development environment regarding other resources, analysis, and information that might help them make better decisions at development time.

 - Resources - What API focused resources are available within an IDE environment. How do developers find documentation, and other resources that support them in their integrations.

 - Analytics - What analytics are available to support API integrations, during development? Is the ability to track and measure API related integrations during design and development time.

# Browsers
Are there any browser plugins, add-ons, bookmarklets and integrations used as part of each service’s operation, providing browser specific client solutions, that are ready to go--no coding necessary.

- Bookmarklets - Establishing copy and pastable, or drag and droppable browser bookmarklets that can be used to make specific API calls, and put a single service to use.

- Builder - Are there any tools for building browser add-ons, plugins, bookmarklets, or assist in configuring a browser to execute something on behalf of a particular service?

- APIs - Are there specific browser APIs that work with a specific service, or in conjunction with a service when an API consumer is putting to use within a specific browser.

# Embeddable
Information about any embeddable badges, buttons, widgets, and other JavaScript enabled solutions built on top of a service?

## Overview
Providing a snapshot of what is available when it comes to embeddable solutions build on top of services, offering a one-stop location for information and embeddable solutions.

- Language Support - Providing support for multiple languages across embeddable elements.

- CSS Control - Providing support over CSS elements for embeddable elements.

- Analytics - Providing analytics as part of the embeddable tooling operations.

## Embeddable Tools
Publishing a list of all the embeddable tools available for deployment on top of existing services by developers or non-developers looking to embed features available in service on other web and mobile locations.

- Widgets - Widgets are highly functional, API is driven​ JavaScript tools that provide portable applications that can be embedded on any website or application.

- Buttons - Buttons are shareable snippets of code that often share, syndicate or trigger a variety of events that use APIs as their source.

- Badges - Badges are common for displaying content and resources delivered via an API and allow these assets to be embedded on any website or application.

- Bookmarklet - A bookmarklet that can be added to the toolbar of a browser, and quickly push data to an API.

- Login Button - Providing a single click button for logging into system.

- Intents - providing the ability to easily make a single, or orchestrate several API calls -- fulfilling a single intent.

## Embed Engines
Documenting any engines and builder solutions available that allow users to build their own embeddable solutions, with a handful of customizable elements, and features for them to change and make work for different applications.

- Widget Builder - A widget builder provides a form that API consumers can use to configure a predefined widget that is integrated with an API, allowing them to customize and tailor the widget experience.

- JavaScript API - A complete JavaScript API that developers can use to build and manage their own JavaScript integrations with an APIs resources, beyond existing widgets.

## Embed Formats
What open formats are supported to ensure that embeddable tools build on top of services or interoperable, and employ common patterns when it comes to extending the features of a service.

- Open Graph Protocol - The Open Graph protocol enables any web page to become a rich object in a social graph, by embedding of simple tags in the pages header that describe objects.

- oEmbed - Format for allowing an embedded representation of a URL on third party sites to display embedded content (such as photos or videos) when a user posts a link to that resource.

# Bots
What type of automation and bot implementations are in development or being supported as part of a service’s operation?

- Services - Are there specific services that are designed to support bot and other approaches to automation.

- Resources - Profiling the resources available regarding building and operating bots on a platform, involving any particular service.

- Development Kits - The available development kits focused on assisting API consumers in building bots that use a platform services and resources.

- Builders - Details regarding the tooling and services available for helping service consumers build, deploy, and manage bots via a platform.

- Accounts - Information and directories regarding the registering and sharing of bot accounts that are operating on a platform using existing services.

- Applications - Information and directories regarding the registering and sharing of bot applications that are operating on a platform using existing services.

- Ethics - Detailing what ethical bot behavior looks like on a platform, providing a base for API consumers to think about when building bots that use a service.

- Rules - Establishing a set of rules that bot developers should be following as they look to automate, and build accounts and applications that are using services.

# Visualization
Are there specific visualizations that exist to help present the resources available within any service?

- Services - Providing details regarding any services that can be used to help visualize the data, content, and algorithmic output from any platform services.

- Tooling - Providing details regarding any open source tooling that can be used to help visualize the data, content, and algorithmic output from any platform services.

- Embeddable - Details regarding how to put embeddable visualizations to use that are connected to, generated by, or in sync with platform services.

# Analysis
How are logs, APIs, and other aspects of a service being used as part of wider analysis, and analytics strategy?

- Metrics - Details regarding which metrics are used as part of analysis features involving platform services, and how results are obtained by having clear metrics in place.

- Services - Providing details regarding any services that can be used to help analyze the data, content, and algorithmic output from any platform services.

- Tooling - Providing details regarding any open source tooling that can be used to help analyze the data, content, and algorithmic output from any platform services.

- Platform - What is available to analyze platform usage to the platform itself, allowing teams to measure what is happening, and understand operations at all levels.

- Developer - What is available for developers to analyse their own consumption, usage, and behavior, including informing them of what is measured about them at the platform level.

- Historical - Are there services available that provide historical analysis opportunities, allowing consumers to look back over history, as well as get the most recent information.

- Predictive - What approaches are in place to help predict the future when it comes to analysis, allowing for consumers to user services that work with historical, current, as well as potential future outcomes.

- Machine Learning - Details regarding how machine learning is applied at the analysis layer, adding the ability to establish models based upon platform operations, and make decisions as part of wider artificial intelligence strategy.

# Aggregation
Are there any aggregation solutions in place that involve the service, and depend on its availability?

- Services - Providing details regarding any services that can be used to help aggregate the data, content, and algorithmic output from any platform services.

- Tooling - Providing details regarding any open source tooling that can be used to help aggregate the data, content, and algorithmic output from any platform services.

- Industry - Are there opportunities to access aggregate data within the industry, comparing data across providers, and even with competitors whenever possible.

- Definitions - When it comes to aggregation are there overarching API definitions and schema that help normalize the aggregate information, including mappings to each individual sets of definitions?

- Authentication - Are there aggregate authentication concerns, practices, services, and tooling in place to make sure many different APIs can be managed effectively?

- Reliability - What is in place to help ensure reliability across many disparate API providers, ensuring a certain quality of service when one breaks or goes away?

- Consistency - How is consistency across many different APIs surface area and schema addressed, providing a single philosophy for handling the changes that will exist?

# Integration
What 3rd party integrations are available for working with a service in existing integration platforms like IFTTT, and Zapier.

- Authentication - Providing the mechanisms for the most common approaches to API authentication, including basic auth, digest auth, session based, oAuth.

- Triggers - Provide the framework to use verbs and nouns, with help text, and webhook infrastructure to trigger anything users will desire.

- Actions - Provide the framework to use verbs and nouns, with help text, and webhook infrastructure to accomplish an action users will desire.

- Searches -Allowing for simple questions to be asked, and provide a framework to allow APIs to be employed in answering any question asked.

- Webhooks - Putting the automation in API integration, allowing for webhooks that can be triggered,

- Notification - Using notifications throughout the process to keep the platform, developers, and end-users informed about anything that is relevant.

- Scripting - Allowing for code integration for calculating, converting, and manipulating data as part of any step of the process.

- Multi-step - Going beyond just just triggers and actions, and allowing for multi-step workflows that put multiple APIs to use.

- Activation - Allowing developers and end-users of the integration, and automation to decide whether the process is invite only, private, or publicly available.

- Pages - Providing a single, or multiple pages and directory of integrations available as part of a service operations, either direct integrations or enabled by a 3rd party platform.

- Command Line Interface - Delivering a Command Line Interface (CLI) that developers can use when integrating, as well as building into continuous integration pipelines.

- Rules - Establishing a set of rules of what is acceptable when it comes to integrating 3rd party services with a platform, establishing a reasonable expectation around integration.

# Network
Information about networks that are setup, used, and allocated for each service governing how it can be accessed and consumed.

- Virtual Private Cloud - Establishing isolated cloud resources with your own private virtual network for the delivery of services to a specific audience or set of applications.

- Addressing - What IP addresses and other DNS related information is available regarding the network layer of operating any particular service, or across many services.

- Ports - What ports are in use as part of operating services, including any standard and non-standard uses, covering all stages, and environments used as part of the platform.

- Connection Changes - Providing information on how connections have changed, or can be changed as part of API access across all services.

- Policies - What network policies are in place, and should be considered as part of service operations, making sure behavior is known and sanctioned as part of access of to resources.

- Bandwidth - What bandwidth restrictions, costs, and other allowances are in place which should be considered, measured, and understood as part of operating services?

- Security - What are the network level security concerns and process in place for addressing the overall security of the network(s) used as part of operating services.

- API - What APIs are available for working with the network level, ensuring that all levels of the API stack are programmatically accessible.

# Regions
Which regions does a service operate within, making it available in specific regions, and jurisdictions–also which regions is it not allowed to operate within.

- Region Lists - Providing lists of regions that are available to operate within across many different providers, allowing API developers to understand where they can publish.

- Region Maps - Publishing a single, or multiple maps that show all the regions that are available as part of platform operations, providing a visual representation of options.

- Used Regions - A real time, working list of regions that are in use as part of platform operations, showing where services are deployed permanently or temporarily.

- Monitoring - Details on how regions can be used to monitor different services, sharing healthy practices for how regions can be used for platform availability.

- Redundancy - Information regarding how services can failover, balanced, and made available across multiple regions, sharing healthy practices for how this is done across teams.

- Regulatory - How are regions employed as part of regulatory practices, ensuring that data, content, and algorithms are applied appropriately within specific areas of operation.

# Webhooks
Are there webhooks employed to respond to events that occur via the service, pushing data, and notification externally to consumers?

## Core
Focusing in on the core aspects of webhooks and how they operate, providing details on the essential features users will need when putting webhooks to work in their applications.

- URL - Tooling for managing the URL of a Webhook.

- Payload - Editing what goes into the payload of the Webhook.

- Event - Selecting which events triggers a Webhook.

- Content Type - Selecting the content type for a Webhooks being submitted.

## Inbound
Usually webhooks are outward bound, but occasionally they have inbound characteristics that should be documented and made available to potential consumers.

- Webhooks Targets - Providing targets where Webhooks can post information, with targets then providing other services once received.

## Outbound
Defining the outbound features of webhook functionality, documenting how they are put to use for pushing of data, content, and other resources externally in response to events.

- Multiple Destinations - Sending of received Webhooks to multiple destinations once received, providing routing opportunities for Webhooks.

- Scheduling - Running code that can be used as webhook target, also as schedule jobs allowing them to trigger on schedule instead of just events.

## Operations
Looking at the operational side of managing webhooks, and providing any information and features to help webhook consumers understand what is happening when they put them to work.

- Analytics - Providing analytics on webhooks activity, triggers, usage, and other aspects of operations.

- Emails - Trigger the sending of emails when webhooks are triggered, received, or other aspects of operations.

- Logging - The logging of all activity generated via webhook activity.

- Alerts - Triggering of alerts based upon events, schedule, and other webhook operations.

- Simulator - Being able to simulate the occurrence of a webhook without the actual event being triggered.

## Utilities
Detailing some of the other more utility aspects of webhook operations, making sure as many details about how they are are covered for consumers to learn from and take advantage of.

- Transformations - Allow for transformations of received webhooks before they are sent elsewhere.

- Scripting - Providing scripting tools for creating of webhook targets, transformation, and other webhook functions.

- Retry - Allowing for the retry of any webhook, based upon specific events or schedule.

# Migration
What solutions are available for migrating an API between regions, cloud environments, and on-premise?

- Discovery - Provide the ability to discovery and map out existing services, systems, and applications, and make them available for migration.

- Server Migration - Provide the ability to migrate virtual machines between service providers, and on-premise systems.

- Container Migration - Provide the ability to migrate containers between service providers, and on-premise systems.

- Database Migration - Provide the ability to migrate databases between service providers, and on-premise legacy systems.

- Data Migration - Provide the ability to migrate database between service providers, and on-premise legacy systems.

- Storage Migration - Provide the ability to migrate stored objects and documents between service providers, and on-premise legacy systems.

- Acceleration - Identifying solutions and processes for accelerating the server, container, database, data, or storage migration.

- Managed - Provide certified partners and vendors who can assist with a managed migration, helping make sure it happens without any problems.

- Resources - Identifying what sources are available to learn from and better plan and prepare for the migration of legacy systems to their new locations.

# Backup
What types of backups are in place to bring redundancy to the database, server, storage, and other essential aspects of a service’s operations?

- Virtual Machine - Providing services and tooling for backing up virtual machines and containers, allowing for easy storage and restore of all compute resources.

- Database - Providing services and tooling for backing up database, allowing for easy storage and restore of all database resources.

- File Storage - Providing services and tooling for backing up file storage, allowing for easy storage and restore of all storage resources.

- Restore - Allowing any machine, database, and file to be restored based upon a variety of criteria, and across all regions, and all available  deployment options.

- Retention - Determine the constraints, and process for determining and managing retention of backups across all services, properly defining how long anything should be kept.

- On-Premise - Allowing for on-premise backups to occur, ensuring that backups of all resources are available in at least one or two additional locations.

- Hybrid - Allowing for hybrid on-premise and cloud backups to occur, ensuring that backups of all resources are available in at least one or two additional locations.

- Cloud - Allowing for cloud backups to occur, ensuring that backups of all resources are available wherever in the cloud that makes the most sense for stability and access.

- Archiving - Supporting the ability to archive backups of machines, database, and storage to alternate archives that be stored outside the mainstream backup process.

- Compliance - Providing the ability to verify and report upon backup and restore process to ensure they are in alignment with regulatory compliance and governance restrictions.

- Status - Allowing for the status of backups across all services to be reported upon, and responded to across the platform, allowing for complete backup coverage.

- Service Level Agreement - connecting the backup and restore process to the wider service level agreement (SLA), and helping measure, deliver, and report upon the entire backup process.

# Real Time
Are there Server-Sent Events (SSE), Websocket, Kafka, and other real time aspects of a service’s delivery, allowing for the delivery of content, data, and other resources in real time, using dedicated connections and streams.

## Architecture
Looking at the architecture involved with delivering real time services, and making sure that API consumers have what they need to adequately put real time solutions to work for them properly.

- Proxy - A proxy server is a server (a computer system or an application) that acts as an intermediary for requests from clients seeking resources from other servers.

- Compute - Providing cloud compute infrastructure to accompany and support real time technology.

- Containers - Providing container virtualization infrastructure to accompany and support real time technology.

- Database - Providing database infrastructure to accompany and support real time technology.

- Storage - Providing cloud storage infrastructure to accompany and support real time technology.

- Content Delivery Network (CDN) - Providing content delivery network (CDN) infrastructure to accompany and support real time technology.

- Caching - Providing caching infrastructure to accompany and support real time technology.

- Compression - Providing request and response compression infrastructure to accompany and support real time technology.

- Open Source - Providing open source tooling to accompany and support real time technology.

- DNS - Providing DNS infrastructure to accompany and support real time technology.

## Authentication
Covering the ways in which real time services are authenticated and authorized when it comes to making data and content available in streams and dedicated connections.

- Java Authentication and Authorization Service (JaaS) - Java Authentication and Authorization Service, or JAAS, pronounced Jazz, is the Java implementation of the standard Pluggable Authentication Module (PAM) information security framework. JAAS was introduced as an extension library to the Java Platform, Standard Edition 1.3 and was integrated in version 1.4.

- ACL-Based Authorization - An access control list (ACL), with respect to a computer file system, is a list of permissions attached to an object. An ACL specifies which users or system processes are granted access to objects, as well as what operations are allowed on given objects.[1] Each entry in a typical ACL specifies a subject and an operation. For instance, if a file object has an ACL that contains (Alice: read, write; Bob: read), this would give Alice permission to read and write the file and Bob to only read it.

## Features
Covering the common features involved with consuming real time feeds and streams, helping consumers understand why they might want to putting these types of APIs to work in their applications, over more request and response based solutions.

- Presence - Presence provides information on when a user has joined or left a channel, who, and how many, users are subscribed to a particular channel, which channel(s) an individual user is subscribed to associated state information for these users, which may include latitude / longitude, typing status, and more.

- Push Notifications - Push notifications let your application notify a user of new messages or events even when the user is not actively using your application. On Android devices, when a device receives a push notification, your application's icon and a message appear in the status bar.

- Messaging - Approaches to enabling messaging for users from custom formats, to SMTP, XMPP chat, and any other way of sending messages back and forth between clients.

- Chat - Providing a always on experience when messaging, establishing presence awareness of each user that is part of a conversation.

- Groups - Allow users and applications to be put into lists, allowing real time features to participants of these groups.

- Search - Providing search features, allowing the real time search of users, messages, and other data or content.

- Scheduling - Offering the ability to schedule messages, jobs, and other events, and allow triggering of them on defined schedules.

- Multi-Lingual - Providing default multi-lingual support, either natively or through real time translation.

- Offline - Provide graceful degradation of services when their is no network connection, allowing for seamless on and offline transitions.

## Geo
Understanding the geographic limitations or features associated with the delivery of real time APIs, allowing for more precise filtering and subscription to streams and channels that might be more relevant.

- Geofencing - A geofence is a virtual barrier. Programs that incorporate geo-fencing allow an administrator to set up triggers so when a device enters (or exits) the boundaries defined by the administrator, a text message or email alert is sent.

- GeoLocation - Geolocation is the identification of the real-world geographic location of an object, such as a radar source, mobile phone or Internet-connected computer terminal. Geolocation may refer to the practice of assessing the location, or to the actual assessed location.

- Beacon - A beacon is an intentionally conspicuous device designed to attract attention to a specific location. Beacons can also be combined with semaphoric or other indicators to provide important information, such as the status of an airport, by the color and rotational pattern of its airport beacon, or of pending weather as indicated on a weather beacon mounted at the top of a tall building or similar site. When used in such fashion, beacons can be considered a form of optical telegraphy.

## Management
Providing information regarding the management tooling involved with and provided to help manage the consumption of real time streams, channels, and feeds, enhancing the ways in which consumers can engage.

- Analytics - Providing analytics on all activity via account(s), allowing users to review their usage in a visual way.

- Deep Linking - Deep linking is the use of a hyperlink that links to a specific, generally searchable or indexed, piece of web content on a website.

- Logging - Allow the logging of all activity that occurs, and access by end users and developers.

- Rate Limiting - Provide tools for controlling the rate limits of activities on a platform, via a number of different mechanisms.

- Debugging - Offering debugging tools to assist developers when they are building applications using real time technology.

- Statistics - Providing statistical information about how API resources are being consumed in a client.

## SDK
What real time SDKs are available for working with real time streams, and handling more dedicated API connections within a variety of web, mobile, or even device based applications.

- Android - Providing an Android SDK for mobile developers to put to use.

- IOS - Providing an IOS SDK for mobile developers to put to use.

- JavaScript - Providing a JavaScript SDK for mobile developers to put to use.

## Protocols
What are the protocols being used to deliver real time APIs, and being used by existing sources, or are being considered as part of the road map in response to consumer needs. Adding to the API toolbox, and extending being basic web API consumption.

- Simple (or Streaming) Text Oriented Messaging Protocol (STOMP) - STOMP is the Simple (or Streaming) Text Oriented Messaging Protocol. STOMP provides an interoperable wire format so that STOMP clients can communicate with any STOMP message broker to provide easy and widespread messaging interoperability among many languages, platforms and brokers.

- Advanced Message Queuing Protocol (AMQP) - The Advanced Message Queuing Protocol (AMQP) is an open standard for passing business messages between applications or organizations. It connects systems, feeds business processes with the information they need and reliably transmits onward the instructions that achieve their goals.

- MQTT - MQTT is a machine-to-machine (M2M)/Internet of Things connectivity protocol. It was designed as an extremely lightweight publish/subscribe messaging transport. It is useful for connections with remote locations where a small code footprint is required and/or network bandwidth is at a premium.

- RSS - RSS (Rich Site Summary; originally RDF Site Summary; often called Really Simple Syndication) uses a family of standard web feed formats to publish frequently updated information: blog entries, news headlines, audio, video. An RSS document (called feed, web feed, or channel) includes full or summarized text, and metadata, like publishing date and author's name.

- Atom - The name Atom applies to a pair of related Web standards. The Atom Syndication Format is an XML language used for web feeds, while the Atom Publishing Protocol (AtomPub or APP) is a simple HTTP-based protocol for creating and updating web resources.

- JSON - JSON (JavaScript Object Notation) is a lightweight data-interchange format. It is easy for humans to read and write. It is easy for machines to parse and generate.

- OpenWire - OpenWire is our cross language Wire Protocol to allow native access to ActiveMQ from a number of different languages and platforms. The Java OpenWire transport is the default transport in ActiveMQ 4.x or later.

- Webhooks - A webhook in web development is a method of augmenting or altering the behavior of a web page, or web application, with custom callbacks. These callbacks may be maintained, modified, and managed by third-party users and developers who may not necessarily be affiliated with the originating website or application.

- Websockets - WebSocket is a protocol providing full-duplex communication channels over a single TCP connection. The WebSocket protocol was standardized by the IETF as RFC 6455 in 2011, and the WebSocket API in Web IDL is being standardized by the W3C.

- Extensible Messaging and Presence Protocol (XMPP) - XMPP is the Extensible Messaging and Presence Protocol, a set of open technologies for instant messaging, presence, multi-party chat, voice and video calls, collaboration, lightweight middleware, content syndication, and generalized routing of XML data.

- SockJS - SockJS is a browser JavaScript library that provides a WebSocket-like object. SockJS gives you a coherent, cross-browser, Javascript API which creates a low latency, full duplex, cross-domain communication channel between the browser and the web server.

- Websub - Websub is an open protocol for distributed publish/subscribe communication on the Internet. Initially designed to extend the Atom (and RSS) protocols for data feeds, the protocol can be applied to any data type (e.g. HTML, text, pictures, audio, video) as long as it is accessible via HTTP. Its main purpose is to provide real-time notifications of changes, which improves upon the typical situation where a client periodically polls the feed server at some arbitrary interval. In this way, PubSubHubbub provides pushed HTTP notifications without requiring clients to spend resources on polling for changes.

- Protocol Buffers - Protocol buffers are Google's language-neutral, platform-neutral, extensible mechanism for serializing structured data – think XML, but smaller, faster, and simpler. You define how you want your data to be structured once, then you can use special generated source code to easily write and read your structured data to and from a variety of data streams and using a variety of languages.

- Real Time Streaming Protocol (RTSP) - The Real Time Streaming Protocol (RTSP) is a network control protocol designed for use in entertainment and communications systems to control streaming media servers. The protocol is used for establishing and controlling media sessions between end points. Clients of media servers issue VCR-style commands, such as play and pause, to facilitate real-time control of playback of media files from the server.

- Hypertext Transfer Protocol (HTTP) - The Hypertext Transfer Protocol (HTTP) is an application protocol for distributed, collaborative, hypermedia information systems.[1] HTTP is the foundation of data communication for the World Wide Web.

- Transmission Control Protocol (TCP) - The Transmission Control Protocol (TCP) is a core protocol of the Internet protocol suite. It originated in the initial network implementation in which it complemented the Internet Protocol (IP). Therefore, the entire suite is commonly referred to as TCP/IP. TCP provides reliable, ordered, and error-checked delivery of a stream of octets between applications running on hosts communicating over an IP network.

- User Datagram Protocol (UDP) - The User Datagram Protocol (UDP) is one of the core members of the Internet protocol suite. The protocol was designed by David P. Reed in 1980 and formally defined in RFC 768. UDP uses a simple connectionless transmission model with a minimum of protocol mechanism. It has no handshaking dialogues, and thus exposes the user's program to any unreliability of the underlying network protocol. There is no guarantee of delivery, ordering, or duplicate protection. UDP provides checksums for data integrity, and port numbers for addressing different functions at the source and destination of the datagram.

- FTP - The File Transfer Protocol (FTP) is a standard network protocol used to transfer computer files between a client and server on a computer network. FTP is built on a client-server model architecture and uses separate control and data connections between the client and the server.[1] FTP users may authenticate themselves with a clear-text sign-in protocol, normally in the form of a username and password, but can connect anonymously if the server is configured to allow it.

- Simple Mail Transfer Protocol (SMTP) - Simple Mail Transfer Protocol (SMTP) is an Internet standard for electronic mail (email) transmission. First defined by RFC 821 in 1982, it was last updated in 2008 with the Extended SMTP additions by RFC 5321—which is the protocol in widespread use today. SMTP by default uses TCP port 25.

- Server-Sent Events - Server-sent events (SSE) is a technology where a browser receives automatic updates from a server via HTTP connection. The Server-Sent Events EventSource API is standardized as part of HTML5 by the W3C.

- HTTP Live Streaming (HLS) - HTTP Live Streaming (also known as HLS) is an HTTP-based media streaming communications protocol implemented by Apple Inc. as part of its QuickTime, Safari, OS X, and iOS software.

- HTTP Long Polling - HTTP long polling, where the client polls the server requesting new information. The server holds the request open until new data is available. Once available, the server responds and sends the new information. When the client receives the new information, it immediately sends another request, and the operation is repeated. This effectively emulates a server push feature.

## Security
Taking a look at the security layer involved with delivering real time streams of data and content, making sure things are properly secured when it comes to high volume consumption.

- Transport Layer Security (TLS) & Secure Sockets Layer (SSL) - Transport Layer Security (TLS) and its predecessor, Secure Sockets Layer (SSL), both of which are frequently referred to as 'SSL', are cryptographic protocols designed to provide communications security over a computer network.

- Security Rules Language - Firebase provides a flexible, expression-based rules language with JavaScript-like syntax to easily define how your data should be structured and when your data can be read from and written to. Combined with our login service which allows for easy authentication, you can define who has access to what data and keep all of your user's personal information secure. The Security and Firebase Rules live on the Firebase servers and are automatically enforced at all times.

# Voice
Are there any voice or speech enablement, integrating services with Alex, Siri, Google Home, or other conversational interface? Looking at how services can be tailored and evolved to better meet this specific type of client usage, which might be significantly different than other web or mobile client scenarios.

## General
What are common building blocks of providing voice-enablement solutions on top of existing services, keeping consumers aware of what is available, and how they can effectively build their conversational interfaces?

- Services - What services are in operation to serve voice enablement, providing a more conversational friendly set of resources to enable this particular clients?

- Resources - Listing of resources available to support voice-enablement, and help API consumers better use voice as part of their efforts.

- Showcase - Is there a place where voice-enablement gets showcased, on the blog, via dedicated application directory, or other location highlighting what is possible?

- Multi-Lingual - What are the multilingual strategies for voice-enablement, even if they are just part of the road map, and something that will eventually happen.

- Playground - What sandbox, virtualization, and playgrounds are available for developers to play with what is possible when it comes to voice-enablement using services.

## Platforms
Discussing what platforms are available when it comes to voice-enablement, and showcasing the support available for each of the major voice platforms, encouraging consumers to help deliver within platform objectives.

- Alexa - What tooling, SDKs, links, and resources are available to help API consumers understand how they can build Alexa voice-enabled applications?

- Siri - What tooling, SDKs, links, and resources are available to help API consumers understand how they can build Siri voice-enabled applications?

- Google - What tooling, SDKs, links, and resources are available to help API consumers understand how they can build Google voice-enabled applications?

- Others - Are there other voice-enabled services and platforms being employed as part of platform operations, allowing services to be used to drive voice applications

# Spreadsheets
What types of spreadsheet integrations, connectors, and publishing solutions are available for a service?

- Microsoft Excel - What types of Microsoft Excel integrations, plugins, and usage is available as part of platform operations, allowing API integration or consumption via spreadsheets.

- Google Sheets - What types of Google Sheets integrations, plugins, and usage is available as part of platform operations, allowing API integration or consumption via sheets.

- Importing - Are there solutions for allowing the importing of spreadsheets or CSV using platform services, allowing spreadsheets to become data sources.

- Exporting - Are there solutions for allowing the exporting of spreadsheets or CSV using platform services, enabling data portability using a common set of services.

- Integrations - What other types of spreadsheet platform enablement is available, allowing services to drive external, spreadsheet-driven functionality and features.

# Investment
Where do the funds for operating a service come from within a company, from external organizations, or VC funds?

- Individual - What individual investments have been made when it comes to platform operations, or are available to make future investments in new services, or applications delivered as part of the platform.

- Corporate - What corporate investments have been made when it comes to platform operations, or are available to make future investments in new services, or applications delivered as part of the platform.

- Venture - What venture capital investments have been made when it comes to platform operations, or are available to make future investments in new services, or applications delivered as part of the platform.

- Grants - Are there grant opportunities involved with the platform operations, or available to consumers who are looking to invest in the platform, or develop applications on top of their services.

# Monetization
What does it cost to operate a service, breaking down the one time and recurring costs involved with delivering the service.

## Acquisition
What is involved with actually bring a service to life, and obtain all the data, content, and other things that will be needed for development, and we will ultimately want to be included as a cost center when it comes to overall budget and planning?

- Entry - Costs, resources, and investment involved with entry of data into a system.

- Validation - All acquisition of data will require some sort of validation to ensure the quality of information.

- ETL - The extracting, transforming and loading of data into the system.

- Discover - What did I spent to find this. I may have had to buy someone dinner or beer to find, as well as time on the Internet searching, and connecting the dots.

- Negotiate - What time to I have in actually getting access to something. Most of the time its on the Internet, and other times it requires travel, and meeting with folks.

- Licensing - There is a chance I would license a database from a company or institution, so I want to have this option in here. Even if this is open source, I want the license referenced as part of acquisition.

- Purchase - Also the chance I may buy a database from someone outright, or pay them to put the database together, resulting in one-time fee, which I'm going to call purchase.

## Development
What does it cost to develop a service, and understand development costs at scale across services? Keeping track of everything it takes to stand up a service and get it ready for production.

- Investment - Who put up the money to support the development of this API resource? Was it internal, or did we have to take external investment.

- Grant - Was the development of this API rolled up in a grant, or specifically a grant for its development. Covering costs involved.

- Normalization - What does it take me to cleanup, and normalize a dataset, or across content. This is usually he busy janitorial work necessary.

- Design - What does it take me to generate a Swagger and API Blueprint, something that isn't just auto-generated, but also has the required hand polish it will require.

- Database - How much work am I putting into setting up the database. A lot of this I can automate, but there is always a setup cost involved.

- Server - Defining the amount of work I put into setting up, and configuring the server to run a new API, including where it goes in my overall operations plan.

- Coding - How much work to I put into actually coding an API. I use the Slim PHP framework, and using automation scripts I can generate 75% of it usually, but there is always finish work.

- DNS - What was the overhead in me defining, and configuring the DNS for any API, setting up endpoint domain, as well as potentially a portal to house operations.

## Direct Value
Taking a look at the direct value that will be generated by a service, helping quantify the impact it will have on revenue, and meeting the organizational objectives behind doing a service in the first place.

- API Value - Each API will have its own credit rate set, where some will be one credit, while others may be 100 credits to make a single call, it can be defined by API or a specific endpoint.

- Limits - The daily allowed credit limit will be determined by the access level tier is registered at, starting with daily free public access to retail, trusted, and potentially custom tiers.

- Usage - How many credits does any one user use during a day, week, or month, across all APIs. When each API is used, it will apply the defined credit value for the single API call.

- Incentive - How can the platform give credits as an incentive for use, or even pay credits for writing to certain APIs, and enriching the system, or driving traffic.

- Purchase - What does it cost to buy a credit, something that could fluctuate from day to day, week to week, or month to month.

- Buyout - Allow API consumers to get paid for the credits on their account, preferably all users are encouraged to spend credits, but buyout is an option.

- Discounts - Can we give discounts when you buy credits through specific channels, promotions, or other type of planned deal.

- Volume - Are there volume discounts for buying of credits, allowing consumers to purchase credits in bulk, when they need to and apply when they desire.

- Applying - Can you wait to apply credits you have accumulated? Given the option with each billing cycle to apply, or you may want to wait and use at future date.

- Value - What is the value of an API resource? Often you will be just making this up, but at the least you should be able to articulate in some way.

- Revenue - What revenue opportunities for the ecosystem around an API and its operation, sharing in the money made from platform operations.

- Timeframes - What timeframes can be leverage to generate direct value? Timeframes should be used in conjunction with plans to dial in the value generated.

- Metrics - What are the metrics, no matter what you choose to track by, what is the metric and its value? The most common metrics is the hit, but could be any other quantifiable metric you can consider.

- Geo - How can geographic location be leverage as part of determining value generation? Different data centers, or networks, or possibly as part of support. How can geographic constraints be applied to maximize value generated.

- Resources - The best part of API design, is you can dial in your value generate to the smallest unit of compute, the single API resource. How are APIs value generation considered at the individual level like this?

- Extensions - Are there extensions available that will impact the developers, or end-users experience. Can extensions be used for a default experience, or added on to incrementally increase value generated.

- Usage - How is usage wielded as part of value generation? Is value about the increased usage of a resource, or possible value generated by a minimum usage of a resource? Usage is an important dimension of determining how value is generated as part of API operations.

- Fees - How are fees leveraged as part of value generation, where like usage, fees driving that value generation, or possibly the lack of fees is where the value lies. Where, within the ecosystem do discussing fees make sense?

- Donations - Does API operations depend on donations, either one time, or possibly soliciting ongoing donations to make sure an API operations. An actual API may be present to allow for donations to occur in-line.

- Grants - Is the value generated around API operations because of a single, or possibly multiple grants? How are grant programs leveraged to develop the API itself, or possibly drive the evolution of resources made available via APIs.

- Percentages - Is value generation measured in percentages? Such as revenue share, or percentage of any resource usage for free. There are a number of ways to think about percentages, and how they apply to defining value generation.

- Users - How is value generated on a per user level? More users is valuable, or possible fewer users. Teams, groups, and many other ways to determine how users impact positively or negatively the value generated from platform usage.

- Relationships - How can relationships between users, or companies be applied to value generated? Will access to more relationships positively or negatively impact how value is generated for platform, and consumers?

- Support - Is access to support something that impacts the value being generated? Does access to support resources introduce the optimal levels of value consumers are looking for? How is support wielded within overall platform monetization.

- Applications - Is value generated looked at on a per application basis? Does having multiple applications impact the value generate? Coming up with interesting ways to understand how applications impact platform value for everyone.

- Integrations - What external integrations are available? How can these be leveraged to enhance the value for consumers? Are some integrations part of base operations, where others are accessible at higher levels, or on a one off basis.

- Investment - Similar to donations, what investment possibilities are part of platform operations? How can access to invest be a value option for consumers, and be used to create more value for platform operators?

## Indirect Value
Stepping back and looking at the indirect benefits of a service, and other ways in which it will generate value for an organization beyond the direct revenue effects, and other benefits it brings to the table.

- Marketing Vehicle - Having an API is cool these days, and some APIs are worth just having for the PR value, and extending the overall brand of the platform.

- Traffic Generation - The API exists solely for distributing links to web and mobile applications, driving traffic to specific properties - is this tracked as part of other analytics?

- Brand Awareness - Applying a brand strategy, and using the API to incentivize publishers to extend the reach of the brand and ultimately the platform - can we quantify this?

- Data & Content Acquisition - Using the API, and the applications built on top as part of a larger data and content acquisition strategy--can we quantify this?

- SaaS - Value generated is focused on SaaS services, and API value generation is about augmenting these services, secondary to the core SaaS business model.

- PaaS - Value generated is focused on PaaS services, and API value generation is about augmenting these services, secondary to the core PaaS business model.

- Devices - An API exists purely in support of a device, such as Fitbit, or with a 3D Robotics Drone. All value generated by the API is about enhancing, and building on the overall device experience.

- Products - An API exists in support of a specific product. Just like devices, but products could be physical devices that are not connected to the database.

- Services - As with products, an API may exist to augment an existing in-person, or possibly a digital service being offered by a company. The API value is centered around this service, and not the actual API.

- Syndication - An API exists to help syndicate data or content on the web. All value generated by the API is in service of the syndication process.

- Analytics - How can analytics be leveraged as part of API value generation? Are analytics part of the base of operations, or are they an added value incentive for consumers, and platform operators.

- Reporting - How is reporting via an API platform part over the overall value being generated? Reporting can be something that benefits internal or external operators, and bring more value to the table.

- Talent - How is talent, from an HR perspective considered as part of the value being generated by an API? Does the API exists as a sort of honeypot to attract talent for hire, project work, or possibly acquisitions and investments.

- Security - How is security used as a lens for measuring, quantifying, and delivering value via the platform. Does the existence of security only available at higher levels or on-demand usage? Security will continue to play an ever increasing role in API monetization.

## Extensions
How are extensions, add-ons, and introducing ways to extend services being monetized allowing for new revenue streams beyond the core features of service being delivered via a platform.

- Add-Ons - Are add-ons used to monetize the platforms? Are they a unit of value that can be used as part of base operations, or on-demand, or as part of any other dimension of API plans?

- Reciprocity - How can API interoperability, automation, and reciprocity with other platforms be used as part of the overall API monetization strategy? Common approaches to reciprocity can be leveraged as part of API monetization and planning.

- Single Sign On (SSO) - How can Single Sign On be leveraged as part of API monetization? Are there some opportunities that can be available for free, or are there other higher levels of access where SSO is an option? Consider how this level of authentication can impact monetization?

## Operation
Providing a detailed plan for what it will take to operate a service, keep it up and running, and fully make available to consumers throughout its lifecycle, and future versions. Establishing monthly and quarterly views of what it takes to operate.

- Definition - How much resources am I applying to creating and maintaining APIs.json, Swagger, and API Blueprint definitions for my APIs.

- Compute - What percentage of my AWS compute is dedicated to an API. Flat percentage of the server its one until usage history exists.

- Storage - How much on disk storage am I using to operate an API? Could fluctuate from month to month, and exponentially increase for some.

- Bandwidth - How much bandwidth in / out is an API using to get the job done.

- Management - What percentage of API management resources is dedicated to the API. A flat percentage of API management overhead until usage history exists.

- Code - What does it cost me to maintain my code samples, libraries, and SDKs for each individual API, or possibly across multiple APIs and endpoints.

- Evangelism - How much energy do I put into evangelizing any single API? Did I write a blog post, or am I'm buying Twitter or Google Ads? How is the word getting out?

- Monitoring - What percentage of the API monitoring, testing, and performance service budget is dedicated to this API. How large is surface area for monitoring?

- Security - What does it cost for me to secure a single API, as part of the larger overall operations? Does internal resource spend time, or is this a 3rd party service.

- Virtualization - What am I spending on virtualization for an API, as part of QA process, for retail sandbox and simulation environments, or for specific partner needs.

## Partner Revenue Generation
What opportunities are there to generate revenue with partners, either bringing in revenue, or possibly sharing with partners in a joint effort? Making services a team sport, and more than just what can be done with internal resources.

- Link Affiliate - What revenue is generated and paid out via links that are made available via the API, with potentially externally affiliate links embedded.

- Revenue Share - What portion API revenue is paid out to potential re-sellers who drive API usage. Revenue is percentage of overall credit purchases / usage.

- Credits to Bill - All revenue is paid in credits on account, and user can decide to get buy out of credits at any time, or possibly use in other aspects of system operation.

- Reseller - Is there a reseller program available for any levels of API platform operations? Are API consumers incentivized to sell products or services, in which they are compensated for? How can platform value being broken up using reseller approaches?

## Reporting
How is revenue being measured and reported upon? How is the value of what services deliver being measured and understood? Provide information on what type of reporting is in place to understand whether or not services are achieving their objectives when it comes to monetization goals.

- Timeframe - How much revenue is being brought in on a daily, weekly, monthly, quarterly, or annual basis for an API and all of its endpoints.

- Users - How much revenue is being brought in on a monthly basis for a specific user, for an API and all of its endpoints.

- Applications - How much revenue is being brought in on a monthly basis for a specific application, for an API and all of its endpoints.

- Plans - Which plans generate most usage and revenue? I should be applying just as easily to aspects of platform / internal usage as well. Better understanding value generated across all plan levels.

- Affiliate Revenue - What was generated from affiliate links made available via APIs, minus what percentage was paid out to API consumers.

- Advertising Revenue - What advertising revenue was derived from web or mobile application traffic resulting from the API, minus whatever was paid out as rev share to API consumers.

- Country - How are things broken down by country? Country defined API operations will continue to be an important way to look at API operations, and value generated.

- Region - Keeping in alignment with traditional sales regions, and looking at value generated within specific regions.

# Plans
Outline of plans involved with defining, measuring, reporting, and quantifying value generated around a service’s operation.

## Overview
Documenting the high level needs to help articulate the plan in place for operating each service, as well as coherently across many different services, providing a single place to tune into the pricing and plans for a platform.

- Dedicated Plans / Pricing Page - Providing a single landing page, available at a simple URL, with all the information about plans available as part of platform operations. There may be more than one plan overview page available, for example one for SaaS side of offering, one for developers, and another possibly for enterprise or partner consumers.

- Definitions - Providing machine readable definitions of the plans, as well as their pricing and details contained within each plan, making API plans more machine readable and executable at discovery and integration-time.

## Elements
What are the individual elements of a plan that dictate the value to consumers, and will be quantified and measured as part of wider monetization and revenue strategy, allowing operators to understand the value being generated, or not.

- Private - Is this plan a private one, available only to a limited audience? While the landing page, or overall portal might be publicly available, the API access itself requires approval, or existing account access before you can get more details. Private APIs are more common than public APIs, but you should think about the pros / cons of keeping things private.

- Public - Is this a publicly available API operation, something that may only apply to some plans? While not all aspects of API operations will be 100% publicly available, there are some elements that anyone from the public can gain access to, even if it is rate limited in some way.

- Free - Is this a free resource, or set of resources, something that may not apply to all plans. Free should be considered even if it is part of a trial, demo, or just a limited level of access by time other metric. Free should be a way to incentivize users to higher level of access, and not damage potential revenue.

- Trial - Is there a trial period that is limited by number of days, which may not apply to all plans. Not all audiences will respond to trial levels of access, but may work will with incentivizing higher levels of access, and API consumption. Refrain from requiring credit cards for trial levels of access, as it deters sign up from abuse by other providers.

- Demo - This resource or set of resources has a demonstration associated with it, which might apply to multiple plans. Consider the possibilities of offer live, or scheduled demos with overall platform operations, as well as individual planned levels of access.

- Access - Access should not be taken for granted, requiring you to request access, or elevated access levels. While different levels of API access are common, it is also common to use API access itself as an element of planned API operations.

- Setup - What are the costs associated with setting up and configuring an account for API access. Whatever time and resources are involved with setting up, or even perceived costs to end-users should be considered. Be careful making setup costs an obstacle for the on-boarding of consumers.

- On-Demand - The resource or set of resources can be deployed, and shut down on demand. Each resource can be evaluated for how long it should be available. With current approaches to virtualizations, it is easier to make API resources available on demand, similar to how Amazon has done with many of their cloud compute resources.

- Reserved - There are opportunities to reserve an instance of a resource or set of resources for specific time frames. If the resources are also available on-demand, a complimentary reserved option should also be considered as part of planning operations.

- Volume - Volume pricing levels are available, with plans based entirely on volume level access to resources. Some platforms operate entirely on volume levels of API access, and levels should be crafted with end consumers in mind, and how they will be consumed, and at what levels.

- Spot - There is an opportunity to big on resources in a localized or distributed marketplace driven environment. Maybe the demand for a resource changes from week, month, season or otherwise, and allowing for bidding can increase competition for a variety of API resources.

- Dedicated - Resources can be allocated in a dedicated state, remaining available with no downtime, or according to SLA. This element is complementary to on-demand, and reserved instances, where the resources can be purchased on a dedicated bases. For many API resources dedicated will be the default state, and not worth mentioning unless on-demand, and other elements are available.

- Infrequent - Resources are accessed infrequently, treating them as warehoused, or off to the side. Another side of the resource availability which focuses on these infrequent levels of access, and may allow a users access or plan shift from infrequent, to higher levels, if rate limits are exceeded.

- Archive - Resources are in an archived state and require very little access, and can be stored in different manner. Like infrequent, archive is mean for maybe one-time access, in future dates. Think of these levels as minimum rate limits, which base pricing not on volume, but only is cheap if minimum thresholds are met.

- Subscription - There is a regular, recurring element to accessing a resource, as part of a larger subscription part of, or separated from plans. In addition to the regular usage, a subscription plan usually continues, and has costs associated with it even if there are no calls against the API made.

- Personal - There is a personal element to a set of resources, meant for the casual user, and probably not developing an application or custom integration. These elements of API access usually involve some way for access APIs for non-developers through API reciprocity services like Zapier, or API aggregation providers like Cloud Elements, and not meant for developers.

- Commercial - There is a commercial licensing element to a set of resources, which require additional business or legal requirements. This element may not be cost associated, and just stipulate there are commercial opportunities around an API. These elements may require requesting access, or additional steps before they can become available.

- Non-Commercial - The platform allows for non-commercial access to resources, which usually means there is additional commercial requirements. Allowing non-profit organizations, researchers, and other potential API consumers the ability to validate their identity, and achieve reduced, or free levels of access can benefit the overall platform reach, and potential marketing engine.

- Educational - A platform provides considerations for K-12 or higher educational access to resources. Like non-profit levels of access, education can benefit the overall platform reach, and benefit other marketing efforts. Reaching educational users, can lead to future individual, business, or institutional users, and improve the overall platform image.

- Wholesale - There are wholesale options around deploying and accessing resources that are available via a platform. With cloud computing providers like AWS, Heroku, and Google, as well as virtualization technology like Docker, providing wholesale implementations of APIs are growing more possible, and are becoming more commonplace in API plans.

- Government - A set of API resources is available specifically for government access, meeting the specialized needs of local or federal government use. Complimentary to non-profit, and educational elements of access, government considerations are growing more common place for some API providers to offer.

- Internal - A set of resources are tailored specifically for internal consumption rather than for public or partner level access. Internal APIs, like public ones will usually have a portal available at an Internet URL, but will require additional access before you can see anything related to the API.

- Partner - There is a focus on partner access to resources, resulting in separate access layers, and features dedicated to partner level consumption. While anyone accessing APIs can be considered a partner, these levels of access usually require much more vetting, making sure business objectives are in alignment, and legal obligations are met. Keeping partner access layers as transparent as possible helps keep harmony with lower levels of public, or even internal API access.

- Reseller - There are reseller opportunities in place around resources available via the platform, that allow approved API consumers to access resources, as well as resell access to resources. Resellers are paid a fixed amount, or possibly percentages of sales of products and services, which could include accessing and usage of API resources.

- Venture - There are venture opportunities around a platform and the resources available, allow for investments to be made, or possibly received. API portals are often used as idea incubation area, but some API providers are going further and allowing for direct investment via the platform, opening up the opportunity financially supporting of various aspects of API operations, and products within its ecosystem

- Type - Are there custom types of plans available, with a grouping dimension that goes beyond just the available plans. Thinking of plan types as a sort of categorization, allowing plans to be grouped by other dimensions, for more easily sharing with different groups. Think about separate between SaaS, developer, or possibly enterprise levels of access, and how plans can be organized by type.

- Features - Additional features, usually key / value pairs that can be used to describe addition elements of API access and consumption. The purpose of this research is to identify some of the common elements of how API providers plan their operations, and there will be a long tale of features that I do not capture--these are features.

- Marketing - Is a big part of API operations about driving marketing efforts for other aspects of business operations. Direct API access is not always the primary motivation for having an API, especially a public API. There are a number of ways to increase attention to products, services, as well as the overall corporate engine using APIs. Acknowledging this across API planning is important to understanding the value generated by API consumption, beyond direct elements.

- Branding - Is there a strong brand aspect to API operations, with clear guidelines, resources, and a presence for the companies brand. It is common to require API consumers to provide brand attribution on their site, and sometimes on web or mobile applications, as part of the API consumption contract. Branding should be reflected as an element for all public APIs, with details about different requirements for different plan levels.

- SaaS - Is the API operations secondary to a strong SaaS focus for a platform. How does an API add value to a SaaS offering? Considering the relationship between an API, and how it can benefit end-users of the platform is important to establishing a stable plan that can benefit both sides of the operation in harmony.

- PaaS - Is the API operations secondary to a strong PaaS focus for a platform. How does an API add value to a PaaS offering? Considering the relationship between an API, and how it can benefit end-users of the platform is important to establishing a stable plan that can benefit both sides of the operation in harmony.

- Traffic - Is a primary focus of an API platform centered around driving traffic to a web or mobile presence. If there is a solid business model around users accessing content or data, driving traffic through an API, without charging API consumers can be a successful approach. How can API consumers be incentivized to drive more traffic to web and mobile properties, by extending the reach of the platform through APIs.

- Content - One of the primary objectives for API resources existing is in support of acquiring data and content that fuels platform operations. This is a very common element of successful API platforms that are operating today, such as Crunchbase or Angellist, or even Twitter and Tumblr. These are all examples of platforms where content acquisition is a core element of their API plans.

- Devices - Situations where APIs are available in support of devices. You can see examples of this with Fitbit or Nest, where they API is just value-add to the devices, allowing 3rd parties to develop applications, and put content or data to use that is generated around the API. This is the layer of the API space that is expanding to what is often called Internet of Things (IoT).

- Products - An API primarily exists to support the existence, or drive the sales of another product, or product line. I separate out devices from this grouping, because they require separate attention. This could describe entire supply chain integration using APIs, all the way to affiliate or reseller style systems like used by Amazon. There are a number of ways products can be sold, by putting APIs to work.

- Services - API resources exist to support other related services, and act as value-add to the primary business focus. This is somewhat duplicate to SaaS or PaaS elements, but more likely is about the delivery of classic services like Uber, TaskRabbit, and other sharing economy solutions are focused on today. How is an API driving the demand of other services, that may not be software based, and bridge into the physical world.

- Syndication - API resources exist to encourage syndication of data, content, and other digital resources. How are APIs supporting the syndication of data and content to other public or private locations, something that may overlap with embeddable aspects of API operations. APIs driven syndication can be seen in popular platforms like Twitter or Facebook.

- Analytics - A set of API resources exist to gather, refine, and organize data for the purpose of driving analytics. While these analytics might be also extended to API consumers, as well as end-users, one of the primary elements of API plans is to generate much needed data for use in analytics, increasing the value of a central, or even distribute resources.

- Reporting - A set of API resources exist to gather, refine, and organize data for the purpose of driving reporting efforts. Analytics is the intelligence, and reports is the distribution model. Using APIs to drive static, or even dynamic reports that can be published, printed, or delivered via dashboards.

- Talent - API resources are focused on driving talent acquisition, or even placement with ecosystem related companies or as part of wider services. This could be in support of an actual recruitment platform, or could just be one aspect of what an API platform does to support talent needed internally, by partners, or even end-users of recruitment related services.

- Security - Access to API resources provide a security benefit, or are in support of other related security products and services. There should always be a base level of security to just keep a platform stable, but sometimes additional, or tighter security elements can be factored into the plan for overall platform operations. Security is an ever-increasing aspect of overall platform health and stability.

- Terms of Service - API resources allow for the dynamic configuration of available terms of service that cover access and usage of resources. Terms of service will play a key role in defining every element of platforms, so it makes sense that it can be a variable used across API planning decisions, and even allow for it to be part of different levels of plans, allowing TOS to play variable roles, depending on which plan you exist in.

- Governance - API resources are focused on governance related tasks within a company or possibly a wider industry. For APIs that operate in more heavily regulated spaces, governance will be a pretty big element of planning around APIs. Governance can be applied across API operations, and subject to variability depending on plan levels and partner tiers of access.

- Donations - API resources allow for, or depend on donations as part of platform operations. Not all APIs will be operating for profit, and will require donations for all, or part of the operational budget. These donations might be large, or they might be smaller from individual API consumers, or possibly end-user groups that benefit from an APIs existence.

- Grants - API resources exist because of grant related resources, which pay for their design, deployment or operations. Similar to donations, grants could be more formal funding opportunities for certain APIs that provide a civic or public good. Part of the goal in identifying this as a building block, is bringing more focus to the need of some APIs in this area, and drive more grant funding their way.

- Advertising - API resources exist in support of advertising related elements of platform operations, driving advertising, or possibly alleviating the need for advertising to be present. The purpose of the APIs might be directly tied to advertising, or be more about helping drive traffic, or attention to resources that depend on advertising for their revenue. This element is focused on how advertising is coupled to API planning, no matter how tight it is.

- API - There are APIs available to access all or part of the plans, pricing, or limitations around an API platform operations. The API platforms I track on that have been around the longest, and are the most mature, have APIs for consumers to use, that gives access to plan information, rate limits, pricing, and other aspects of API operations. I include this as essential, because it will be something every API provider will need to complete in the future.

- Organization - There are organizational elements around API access and usage for API consumers to take advantage of. Are API plans organized by organization, or possibly specific access only for a specific group. How does user organizations, groups, and other ways to categorize API consumption applied at the API planning level?

- Customization - There are customization opportunities around API plans, pricing, and rate limits, giving more control to consumers to customize their experience. For many plans, things may be fixed, but as you go further up the chain, into enterprise and partner level tiers, there may be opportunities for customization of plan elements, where other users do not have the opportunity.

## Extensions
What extensions are available as part of each plan, allowing for clear extending of the platform within the constraints of each available plan or tier for consumers to choose from.

- Add-Ons - Factoring the availability of add-ons into specific API plans or overall API operations.

- Connectors - Factoring the availability of 3rd party or internal platform connections into specific API plans or overall API operations.

## Geo
What geographic variables are in play when it comes to choosing or working within a plan? How can services be delivered geographically or locally to better meet the needs of API consumers?

- Overview - Providing an overview of what geographic regions are covered or available as part of API consumption.

- Country - Providing API access or replication within specific countries.

- Region - Providing API access or replication within specific regions.

- On-Premise - Providing API deployment locally or within existing infrastructure, providing on-premise access levels.

- Co-Location - Allowing for access of API resources via collocated facilities.

## Limits
What are the limits and constraints in place for each plan and access tier, outlining exactly what is available, and where the limits of the plans become clear, incentivizing the shift to higher levels of access and consumption.

- Charts - Providing a chart with a listing of all endpoints and limits for each one.

- Overview - A single page which provides an overview of limits that are in place on API operations.

- Inline - Providing information about rate limits inline, either within documentation or available within API response details.

- Range - Considering a range of values when measuring API consumption, and evaluating plan level access.

- Resources - Limits are place upon specific endpoints or verbs, providing granular controls over API resources.

- Increased - Opportunities for increasing rate limits either by changing plans, or simply requesting limits to be raised.

- Unlimited - The ability to overcome limits, and achieve unlimited access to resources.

- Service Level Agreement (SLA) - A service level agreement (SLA) is applied as part of API operations as a whole, or as part of particular plans.

- API - There is an API specifically for accessing limitations around API resources for API consumers to use.

## Metrics
What data points are measure on a per second, per minute, daily, weekly, monthly or other basis to help quantity the consumption of users at all access levels, defining how value and success is measured, and billing or paying when it comes to incentivize service usage.

- Access - Where access to an API is on the table, and might not be publicly available, or part of all plans. Differing from API access as an element, this is about actually limiting entire APIs from various groups and plans, and allowing it to be metered as part of overall measurements.

- Calls - The most fundamental metric for APIs, the API call.

- Value - What is the value of an API or endpoint, is it simple 1, or maybe 10, allowing for multiple value settings.

- Transaction - Allow for the concept of transactions to exist which may span multiple API calls, moving a single concept forward.

- Count - Tracking by the count of something, could be API calls, files, or any other county of objects that are part of API operations.

- Instances - Allowing for instances of resources that are available via an API platform, and can be used in different ways within existing plans.

- Matches - Allowing for the measurement of API access in terms of when pre-defined matches are returned, rather than all of the results.

- Message - Charging per message rather than each API call that is required to prepare, send, or access messages.

- Volume - Volume is used as a basic measurement of how consumers can access API, providing a standard set of pricing, as well as volume pricing.

- Compute - Providing API resource access based upon various levels of compute power.

- Load Balancing - Measurement of resource usage, based upon the amount of load balancing that occurs.

- Operating System - Measurement of resources, based upon the operating system for compute resources.

- Storage - Measuring API resources based upon the size on the disk.

- Uploads - Restricting and measuring API access based upon the number of file uploads.

- Upload Size - Restricting and measuring API access based upon file upload size.

- Upload Speed - Restricting and measuring API access based upon file upload speed.

- Records - Measuring API access based upon the number of records accessed or returned.

- Containers - Measuring API access based upon the number of folders, buckets or virtual containers deployed.

- Transcripts - Measuring API access based upon the transcripts generated.

- Bandwidth - Measuring API access based upon the amount of bandwidth used.

- Connections - Measuring API access based upon the number of connections or threads made to resources.

- Simulations - Measuring API access based upon the number of simulations generated.

- Transfers - Measuring API access based upon the number of transfers that are executed.

- Transfer Limits - Using the ability to change transfer limits as a metric in API consumption.

- Sync - Measurement for API consumption based upon the number of syncs that are expected.

- Conversions - Measurement for API consumption based upon the number of conversions that are executed.

- Syndication - Measurement for API consumption based upon how much syndication occurs.

- Connectors - Measuring API access based upon the number of connectors that are employed, or part of
account access.

- Relationships - Measuring API access based upon the number of relationships between users and objects that are established or accessed.

- Migrations - Measurement of API accessed based upon the number of migrations that occur.

- Archives - Measurement of API accessed based upon the number of archives that are created.

- Rollback - Measurement of API accessed based upon the number of rollbacks that are executed.

- Tasks - Using the number of tasks that are started or completed as a measurement of API access.

- Events - Measuring of API consumption based upon the number of events that occur or are triggered.

- Trainings - Measurement based upon the number of trainings that occur around API access.

- Maintenance - Measuring maintenance events that occur, and affecting API consumption based upon.

- Latency - Measuring the latency that occurs as part of API access, and allowing it to impact API consumption plans.

- Performance - Using performance as a consideration when measuring API consumption.

- Users - Using the number of users as a metric when it comes to planning, and pricing adjustments.

- Media - Measuring specifically media related considerations as part of API consumption tracking.

- Scan - Measure the scanning of a physical or digital object involved in API operations.

- Support - Directly using support elements as a consideration in API resource planning and consumption.

- Fees - Fees that are used as part of API accounts, and consumption, and applied as part of API plans.

- Percentages - The application of various percentages as part of measuring API consumption, and plan operation.

- Consulting - Factoring in hourly consulting as part of API consumption, and plan operations.

- Priority - Providing the option of being prioritized in API requests and responses, and measured as part of overall planning.

- Groups - API access adjusted based upon grouping, or group level access which is aside from standard plans.

- Zone - Another form of grouping API access, into zones, allowing consumers to access and use resources by zone.

- Memory - Allowing for the measurement of resource access to be determined by the amount of memory available or consumed.

- Health - Factoring in health checks in API consumption, and charging specifically on health checks, or changing plans based upon health results.

- Encryption - Considering the existence of, or strength of encryption as part of the API consumption process.

- Characters - Counting of textual characters as part of the overall API consumption tracking process.

- Agent - Tracking on physical or virtual access to human agents as part of API consumption.

- Price Per - Considering a price per a specific amount of API calls or other metric being applied as part of API consumption.

## Timeframes
What timeframes are in use when it comes to measuring API consumption, and reporting upon plan and access tier usage by service consumers, defining the pay as you go framework in which services access is measured.

- Seconds - Managing, guiding, and restricting plan entries in seconds. This is a common timeframe for considering rate limits, and judging the overall volume requirements of different users. Availability in seconds is often directly linked to compute resources being applied as part of operations, and tie in with overall availability.

- Minutes - Managing, guiding, and restricting plan entries in minutes. Like seconds this is a common timeframe for considering rate limits, and judging the overall volume requirements of different users. Availability in seconds is often directly linked to compute resources being applied as part of operations, and tie in with overall availability.

- Hourly - Managing, guiding, and restricting plan entries in hours. While there may be rate limits at the hourly level, this timeframe is more applied to resources that are on-demand and ephemeral, and can be consumed as needed, in a utility style that is becoming common way to plan API access.

- Daily - Managing, guiding, and restricting plan entries in days. Like seconds and minutes this is a common timeframe for considering rate limits, and judging the overall volume requirements of different users. Availability in seconds is often directly linked to compute resources being applied as part of operations, and tie in with overall availability.

- Weekly - Managing, guiding, and restricting plan entries in weeks. This timeframe is more used to organizing billing and support cycles, organizing resource usage and services rendered within the weekly time period, and aligning billing, and other aspects to this timeframe.

- Monthly - Managing, guiding, and restricting plan entries in months. Like weekly, this timeframe is more used to organizing billing and support cycles, organizing resource usage and services rendered within the weekly time period, and aligning billing, and other aspects to this timeframe.

- Quarterly - Managing, guiding, and restricting plan entries in quarters. Like monthly, and weekly, this timeframe is more used to organizing billing and support cycles, organizing resource usage and services rendered within the weekly time period, and aligning billing, and other aspects to this timeframe.

- Annually - Managing, guiding, and restricting plan entries in years. Like quarterly, monthly, and weekly, this timeframe is more used to organizing billing and support cycles, organizing resource usage and services rendered within the weekly time period, and aligning billing, and other aspects to this timeframe.

## Resources
What other resources are available for use as variables within plans, to help refine and incentivize how service usage and consumption occurs beyond the usual data points?

- Endpoints - Providing access constraints based specifically on API endpoints allowing granular controls over each available resource.

- Verbs - Allowing access controls applied down to the HTTP verb level, providing granular controls for GET, POST, PUT, DELETE, and other dimensions of resources.

# Partners
An overview of partner program involved with a service’s operation, and how a wider partner strategy affects a service’s access and consumption. Establishing a trusted tier of access which high value partners can be organized and given special access to a variety of services, further meeting the platform's goals.

## Program Details
What are the details of the partner program, with all resources, landing pages, and breakdown of how the program will work for consumers, setting the stage for higher levels of access to services, and engagement with the platform.

- Landing Page - An official landing page for the partner program.

- Program Details - Short, concise information about the program.

- Program Requirements - Information about what the details of the program are.

- Program Levels - Details about what the different levels of the partner program are.

## Partner Program
What are the details of the program, and what is expected of partners to get up and running with the platforms partner program, and become eligible for higher levels of access to services.

- Application / Registration - The actual application for registering to become a partner.

- Private Portal - A private portal for partners to login to.

- Certification - Official certification showing that a partner is officially approved and vetted.

## Communication
What is the communication strategy associated with partner levels of access, providing higher levels of communication and engagement as part of involvement with the platform and its services.

- Blog - Have a blog that is dedicated to providing information for the partner program.

- Spotlight - Have a special section to spotlight on partners.

- Newsletter - Provide a dedicated partner newsletter.

## Content
What are the content opportunities that partners can take advantage of, helping stimulate and enforce the partner arrangement and increase the platform as well as partner exposure.

- Quotes - Allow partners to provide quotes that can be published to relevant properties.

- Testimonials - Have partners provide testimonials that get published to relevant sites.

- Use of Logo - Allow partners to use the platform logo, or special partner platform logo.

## Early Access
Are there early access opportunities to services, features, and other aspects of operating the platform that partners can be taking advantage of as they work more closely with the platform.

- Early Communication - Allow for partners to get early access to platform communications.

- Early Opportunities - Access to early platform opportunities meant just for partners.

- Alpha & Beta Access - Allow for beta access to new platform products.

## Financial
What are the financial incentivizes involved with the partner program, helping partners generate revenue, but also incentivize specific behavior and usage around a range of services.

- Revenue Sharing - Offer revenue sharing for partners.

- Reseller Discounts - Offer reseller discounts from referrals they make.

## Legal
What legal details are in place to help govern the partnership opportunities and tiers of access to services that are available, providing a single place where partners can find the legal documents they need.

- Agreement - The legaleze for the partner program agreement.

- Privacy Policy - What is the privacy policy for the partner program.

- Code of Conduct - A code of conduct targeting partners, explaining what is expected.

## Marketing Activities
Providing a list of the marketing activities available to partners who engage with the platform, offering them more exposure and attention to their applications and usage of platform services.

- Blog Posts - Provide blog posts for partners to take advantage of one time or recurring.

- Press Release - Provide press releases for new partners, and possibly recurring for other milestones.

- Facebook Post - Post updates to the platforms Facebook account.

- Twitter Post - Post updates to the platforms Twitter account.

- Google Plus - Post updates to the platforms Google Plus account.

## Partner Showcase
Adding in details regarding how partners are showcased, and how other consumers, press, and stakeholders can discover and learn from existing partner stories about how they put services to work.

- List of Partners - A list of partners, usually name and logo, maybe with some description.

- Partner Stories - Stories of the partners and how they use the platform.

- Partner Search - A keyword search for discovering partners.

## Support
Opening up wider support tiers to partners, allowing them to get access to more resources and direct access to support specialists who can help with better put services to work.

- Discounts - Provide discounts on direct support for partners.

- Office Hours - Provide virtual open office hours just for partners.

- Training - Offer direct training opportunities that is designed just for partners.

- Advisors - Provide special advisors that are there to support partners.

## API
Providing programmatic interfaces for partners to engage with their special access to services, and other resources, allowing for seamless integration and management of their partner relationship.

- Quota Increase - Increasing the rate limit for existing APIs.

- Additional APIs - Provide access to APIs that are only accessible to their partner tiers.

- Read / Write APIs - Access to not only read, but also write, update, and possibly delete access to APIs.

# Certification
Are there certification channels available for applications and developers, defining the knowledge required to competently operate and integrate a service.

- Landing Page - A page dedicated to the certification opportunities available via a platform, providing a single place to understand what is possible.

- Application - A program for certifying that applications meet a certain level of quality and integrity, and meet or exceed the platforms requirements for integration.

- Developer - A program for certifying that developers meet a certain level of quality and integrity, and meet or exceed the platforms requirements for integration.

- Training - Providing training course, materials, workshops, and other resources for helping ensure that developers and applications can understand what is required for certification.

- Badges - Offering badges that can be published, shared, syndicated, and displayed to represent that an application or developer has been certified.

# Evangelism
What does internal, public, and partner evangelism efforts and requirements look like for a service, and its overall presence?

## Goals
Establishing a core set of goals behind why we are doing APIs, understanding clearly why services are being deployed, and what constitutes success when it comes to delivering APIs at scale.

- Growth in New Users - Growing the number of new signups for an API platform, increasing the number of new consumers, and potentially establishing as an active user.

- Growth in Existing User API Usage - Growing the number of existing users who are actively using an API platform, increasing the number of APIs they use, and the number of calls they make.

- Brand Awareness - A consistent strategy and set of resources for extending the brand reach for any API platform, by providing a set of instructions and assets for consumers to use.

- More Applications - Increase the number of applications being developed on top of APIs.

- New System Integrations - Increase the number of integrations that occur with the API, into other systems.

- Other Goals - Any other goal that might be associated with evangelism activities.

## Landscape Analysis
Developing an understanding and awareness of the space we are operating in and mapping out the landscape of service providers who are doing the same thing we are doing within our company, institution, or wider industry.

- Competition Monitoring - Evaluation of the regular activity of competitors, cultivating an ever growing list of who they are and what they are up to.

- Industry Monitoring - Evaluation of relevant topics and trends of overall industry an API is operating within.

- Project & Developer Sites - Identifying of relevant project sites like Elance and ODesk, and targeting developers who may be suited for engagement.

- Keywords - Established a list of keywords to use when searching for topics at search engines, QA, forums, social bookmarking and social networks.

- City Targeting - Target specific markets in cities that make sense to an overall API evangelism strategy.

- Formal Studies - Conduct formal studies in the sector you are targeting, and potentially new business sectors--share internally or possibly with partners and the public

## Consumer Outreach
Defining what customer outreach looks like, and how it occurs in a consistent, strategy, and even tactical way, keeping the platform in sync with its consumers, and vice versa.

- Consumer / Developer Showcase - Providing a showcase of the spotlight is put on developers / consumers who are doing interesting things on the platform.

- Fresh Engagement - Emailing new developers who have registered weekly to see what their immediate needs are, while their registration is fresh in their minds.

- Active User Engagement - Where we reach out to existing, active users of your API and find out what they need, profiling them via Twitter, Facebook, LinkedIn and pulling any profile information to grade and categorize each developer.

- Historical Engagement - Emailing historical active and / or inactive developers to engage and understand what their needs are and would make them active or increase activity.

- Social Engagement - When emailing any developer, using business intelligence to establish any URL, Twitter, Facebook or LinkedIn profile they have and reach out via these networks.

## Partner Outreach
Overlapping with partner efforts, how does evangelism and outreach occur regularly to partners, and keep them engaged with what is happening via the platform, as well as with individual services that matter to them.

- New Partner Engagement - When a new partner is signed up, there is engagement of some sort, on-boarding them properly as a partner.

- Existing Partner Showcase - The showcasing of existing partners, to make sure the spotlight is on them in blog posts, PR, and social media.

## Blogging
What does storytelling look like, and what is the strategy for publishing and syndicating meaningful, helpful, and far reaching content as part of the wider evangelism effort.

- Projects - Establishing of editorial assembly line of technical projects that can feed blog stories, how-tos, samples and Github libraries.

- Stories - Writing, editing and posting of stories derived from projects, with SEO and API area support by design.

- Syndication - Syndication to Tumblr, Blogger and other relevant blogging sites available online.

## Developer Area
Making sure the developer portal(s), and other supporting destinations are visited, evaluated, and considered in an ongoing way to make sure they aren't falling behind when it comes to outreach and messaging.

- Getting Started - Evolution of getting started page when relevant based upon API and network changes, and relevant developer feedback.

- Documentation - Enhancement and addition to API documentation based upon project development and active developer engagement and feedback

- Code Samples - Establish new code samples that can be used within API documentation pages, maintain them as API evolves.

## Events
Where will we be found when it comes to a physical presence across target industries, and making sure there is a physical presence to the platform, team, highlight the valuable services being delivered.

- Hackathons - What hackathons are coming up in 30, 90, 120 days? Which would should be sponsored, attended, etc.

- Meetups - What are the best Meetups in target cities? Are there different formats that would best meet our goals? Are there any sponsorship or speaking opportunities?

- Conferences - What are the top conferences occurring that we can participate in or attend--pay attention to call for papers of relevant industry events.

- Lunches - What brown bag, and other formal or informal lunches are being held with internal, partner, or public stakeholders when it comes to platform operations.

## Forum Management
How is the forum being considered and included in the wider evangelism and outreach strategy, building on the conversations that are already occurring within the community.

- Forum Conversations - Responding to forum activity in a timely and engaging way, and conducting general janitorial work around the community.

- Forum Posting - Generating forum activity by anonymous posters or officially with common problems and questions faced throughout community as well as open landscape.

- Stories - Deriving of stories for blog derived from forum activity, and the actual needs of developers to be crafted and published as part of overall editorial strategy.

## GitHub Management
What activity is occurring via the social coding platform Github, pushing forward conversations around code, definitions, and other projects, focusing on platform projects, as well as those of partners, and other consumers.

- Github Repository - Managing of code sample Gists, official code libraries and any samples, starter kits or other code samples generated through projects.

- Github Relationship - Managing of followers, forks, downloads and other potential relationships via Github.

- Github Organization - Are there Github organizations in place in support of outreach? Is there a single one, or multiple ones for different projects, groups, etc?

## Internal
What does internal storytelling look like across and between teams, showcasing and sharing the efforts of teams who are building and operating services, and collectively moving forward the platform.

- Storytelling - Telling stories of an API isn’t just something you do externally, what stores need to be told internally to make sure an API initiative is successful.

- Participation - It is very healthy to include other people from across the company in API operations. How can we include people from other teams in API evangelism efforts.

- Reporting - Sometimes providing regular numbers and reports to key players internally can help keep operations running smooth. What reports can we produce?

## QA Management
What activity is occurring across existing QA sites on the web, and being used by consumers and other stakeholders as part of their regular activity, which might often include conversations relevant to the platform and services.

- QA Profile Maintenance - Ensure that profile on Quora and Stack Overflow are active.

- Stack Exchange - Regular trolling of Stack Exchange / Stack Overflow and responding to relevant [Client Name] or industry related questions.

- Quora - Regular trolling of Quora and responding to relevant [Client Name] or industry related questions.

- QA Seeding - Seeding of questions by anonymous 3rd party profiles for relevant topics.

## Reporting
How is evangelism measured and reported upon by the teams owning and delivering services? What is communicated internally, with partners, and shared externally with the public and service consumers?

- Activity By Group - Summary and highlights from weekly activity within the each area of API evangelism strategy.

- New Registrations - Historical and weekly accounting of new developer registrations across APIs.

- Volume of Calls - Historical and weekly accounting of API calls per API.

## Roadmap
How is the road map integrated into the evangelism and outreach efforts, using the future as a tool for capturing consumer, and would-be consumer's attention, and getting them more involved with the platform and it's services.

- Roadmap - Provide regular feedback on the API roadmap based upon developer outreach and feedback.

## Social Bookmarking
What does evangelism look like across social sharing and bookmarking locations, actively sharing platform and service URLs, but also actively sharing the links of other relevant information to consumers, partners and other stakeholders.

- Hacker News - Social bookmarking of all relevant API evangelism activities as well as relevant industry landscape topics to Hacker News, to keep a fair and balanced profile, as well as network and user engagement.

- StumbleUpon - Social bookmarking of all relevant API evangelism activities as well as relevant industry landscape topics to StumbleUpon, to keep a fair and balanced profile, as well as network and user engagement.

- Reddit - Social bookmarking of all relevant API evangelism activities as well as relevant industry landscape topics to Reddit, to keep a fair and balanced profile, as well as network and user engagement.

- Product Hunt - Listing of new API offerings via the Product Hunt social product and service platform, showcasing any new resources as they are made available.

## Social Management
Outlining how social media channels are being managed and curated as part of evangelism efforts, keeping them in sync with other campaigns, and using them as a regular way to engage with internal, partner, and 3rd party stakeholders.

- LinkedIn - Setup of new API specific LinkedIn profile page who will follow developers and other relevant users for engagement.  Posting of all API evangelism activities.

- Twitter - Setup of new API specific Twitter account, and the tweeting of all API evangelism activity, relevant industry landscape activity, discover new followers and engage with followers.

- Facebook - Setup of new API specific Facebook company, and the posting of all API evangelism activities and management of friends.

## Support
How are support efforts integrated with evangelism, ensuring that existing conversations are actively being used to generate new content, and amplify what is already occurring via the platform and services.

- Email Coordination - Regular coordination, relaying of support issues with central support process.

- Email Needs Tracking - Deriving of common support requests to drive API and API area roadmap.

# Showcase
How are developers and applications using a service showcased, and presented to the community, demonstrating the valuable around a service?

- Developer - Having a strategy for the publishing of a developer showcase directory, and a process focused on incentivizing developers to deliver valuable integrations, while providing them valuable attention and spotlight.

- Application - Having a strategy for the publishing of an application showcase directory, and a process focused on incentivizing developers to deliver valuable integrations, while providing them valuable attention and spotlight.

- Partner - Having a strategy for the publishing of a partners showcase directory, and a process for shining the spotlight on partners via regularly occurring cycles.

- Service - Regularly shining a light on specific platform, partner, or 3rd party service that will provide value to platform consumers, highlighting interesting use cases around services.

- Blog - Making sure to use the platform blog to showcase developers, applications, partners, and services on a regular basis, providing a regular stream of content that informs consumers.

- Social - Making sure to use social platforms to showcase developers, applications, partners, and services on a regular basis, providing a regular stream of signals that informs consumers.

# Deprecation
What are the plans for deprecating a service, involved the road map and communication around the individual and overall deprecation of service(s).

## Communication
How is deprecation communicated out across stakeholders, providing a structured approach to managing not just change, but the inevitable shuttering of services, making sure all consumers are tuned into what is happening on the horizon.

- Key Players - As soon as the first decision to deprecate is made, who are the key players, and stakeholder that need to be contacted, and made aware of the API deprecation.

- Public Players - Once key stakeholders are made aware, what is the plan to go public, and make the general community, and industry aware that the API deprecation is imminent.

- Schedule (Runway) - What does the entire runway look like, with as complete schedule from first decision, to final date -- including a communication schedule documented along the way.

- Historical - What historical communications will be made available from blog posts, to tweets, documentation, and other communication focused efforts.

- Be Real - Make sure that you are genuine in your plans, communication, and outreach.

- Be Friendly - Be as friendly as you can. It will be a hard time for everyone involved.

- Be Transparent - Try to be as transparent as you possibly can, throughout the process.

- Be Respectful - Showing respect for your consumers, and their challenges will go a long way.

- PR Campaign - Craft a public relations plan, and execute it well. Don't take shortcuts.

- Communicate Often - Make sure and email, post to blog, tweet, and communicate regularly about the deprecation.

## Licensing
Openly discussing and sharing the licensing involved with deprecated backend, frontend, as well as API definitions, allowing for consumers to potential take code and put to work after a service has been deprecated.

- Data License - How will data be licensed after things are shut down?

- Server Code - What server code will be made available as open source license?

- Client Code - What client code will be made available as open source license?

- API License - How will the API definition, and data schema be licensed for reuse?

## Management
What does the overall management of the depreciation process look like leading up to the actual shuttering of services, including the underlying tools used to make it happen, and keep consumers in tune.

- Github Repo - Will a dedicated Github repository be made available for the company, platform, API, or other aspects of opportunity, made available for capturing any remaining code, data, and content.

- Github Issues - Is there a Github issues established for handling all concerns, and conversations around the API deprecation.

- API Purgatory - Have you contacted Kin Lane, the API Evangelist, so he can take a snapshot of your API, for inclusion in the API Purgatory Museum.

- X-API-Warn - Using the X-API-Warn header for all requests made to any deprecated APIs.

## Runway
Providing clear details on what the deprecation runway will look like for a service, or any group o services, setting expectations accordingly, and making sure the time frames are clearly articulated.

- Initial Expectation Set - What expectations are, or have been set early on in the API design, and deployment parts of the life cycle when it comes to API deprecation.

- Legal Department - What legally has been provided in terms of service, privacy policy, and other parts of the legal department for a platform.

- First Decision - Establishing that an API or platform will need to be deprecated. Recording the date, time, and other key details on what this decision was reached.

- First Notice - What is the time to the first external notice, either privately to partners, or also publicly to the general community.

- Lock-down New Signups - When will new signups for the platform be locked down, stopping all new user and application registration.

- Lock-down New Writes - When will all POST, PUT, and other write capabilities be locked down, making it easier to stabilize, sync, and migrate for final shut down.

- Light Switch Flicking - Will there be light switch flicking, or dark-out testing, which send real world pain to API consumers, reminding them that a shutdown is imminent.

- Other Milestones - What other milestones are there that will be important to internal, partner, and public stakeholders?

- Final Date - What is the final date for shutdown, requiring all syncs, migrations, exports, and integration to completely cease.

## Support
Details of the deprecation support plan that is in place, providing assistance to partners and consumers as they work to migrate off of a service that is being deprecated.

- Contact Person - Who is the person (name, email, Twitter, and Github) who is the point of contact for the API deprecation process.

- Migration Partners - Are there any migration partners that can help out during any migrations, syncing, configuration, and setup of external solutions.

- Migration Locations - Are there any other existing platforms, including competitors, that you can point API consumers to, as an alternative to the API being deprecated.

## Services & Tooling
Providing information on any tooling or services that are available to ease migration, transition, and the pain often associated with services being shuttered, and going away.

- Data Migration - What data migration tools, services, and support will be made available to help customers get their data off of a platform, and somewhere where they can put to use.

- Settings Migration - Will there be the opportunity to export settings, and other configurations, so that they can be applied into other external systems, either automatically, or manually.

- Data Sync - Are there any real-time data sync opportunities, to help reduce the amount of work that is needed at the time of shutdown, slowly getting API consumers offloaded to their new solution.

- Data Portability - Beyond migration, and syncing, can API consumers get raw dumps of all of their usage data, as well as any other object, and entity they have stored via API operations.

## Types
Clearly articulating what type of deprecation is occurring, with a full awareness of the scope and how it will impact the platform, partners, and consumers along the way.

- Individual API Endpoints - Looking to have a plan for the deprecation of individual APIs, or sets of APIs.

- Individual API Tooling - An approach to how you deprecate one of the client solutions available on API platform.

- Entire Platform Shutdown - What is the plan for an entire platform shutdown, ceasing all API operations.

- Enter Platform Safe Mode - What is the plan for just putting the platform into safe mode, and still operating.

## Virtualization
Providing virtualized instances of services, as well as client tooling that can be deployed by consumers, allowing for them to continue operating long after a service has been deprecated--of course, with no support.

- AWS AMI - Will there be an Amazon AMI made available for any server or client implementations?

- Heroku Deploy - Will there be Heroku deployment made available for any server or client implementations?

- Docker Image - Will there be Docker images made available for any server or client implementations?

# Training
What training materials need to be developed, or already exist to support the service.

- Landing Page - Providing a landing page for aggregating and delivering all platform and service related training programs and materials for easy discovery and engagement.

- Content - Publishing formal training materials that help address the areas that platform partners and consumers will need to understand as they work to put resources to work in their applications.

- Blog - Regularly publishing, sharing, and sydnicating out training materials on the blog, and making it part of the regular communications, evangelism, and storytelling cycles.

- Social Media - Leveraging social media channels for syndicating training materials, but also using them as opportunities to engage with users.

- Videos - Developing, publishing, and syndicating video content intended to deliver training materials to API consumers, using the developer portal, and 3rd party channels.

- Services - What services are available for training, including APIs to deliver content, as well as in-person workshop and trainings that can occur as part of human engagements.

- Calendar - Providing a calendar of trainings that are occurring either online or offline, allowing consumers to plan for, and participate in formal training opportunities.

- Certification - Providing certification associated with the completion of training, which might include multiple tiers of accomplishments, and providing badges and other proof of completion.

# Governance
How are all steps measured, quantified, aggregated, reported upon, and audited as part of a larger quality of service effort for each service.

- Definitions - Plan for which definitions are required to provide what is needed to feed a wider service governance strategy.

- Design - Plan for the API design guidance that is needed to provide what is needed to feed a wider service governance strategy.

- Versioning - Plan for what versioning guidance that is needed to provide what is needed to feed a wider service governance strategy.

- DNS - Plan for the DNS guidance that is needed to provide what is needed to feed a wider service governance strategy.

- Deployment - Plan for the API deployment guidance that is needed to provide what is needed to feed a wider service governance strategy.

- Orchestration - Plan for the orchestration details are needed to provide what is needed to feed a wider service governance strategy.

- Dependencies - Plan for the dependency guidance that is needed to provide what is needed to feed a wider service governance strategy.

- Search - Plan for the search guidance that will be needed to drive a wider service governance strategy.

- Proxy - Plan for the proxy guidance that will be needed to drive a wider service governance strategy.

- Gateway - Plan for the gateway guidance that will be needed to drive a wider service governance strategy.

- Virtualization - Plan for the virtualization guidance that will be needed to drive a wider service governance strategy.

- Authentication - Plan for the authentication guidance that will be needed to drive a wider service governance strategy.

- Management - Plan for the management guidance that will be needed to drive a wider service governance strategy.

- Logging - Plan for the logging guidance that will be needed to drive a wider service governance strategy.

- Portal - Plan for the portal guidance that will be needed to drive a wider service governance strategy.

- Documentation - Plan for the documentation guidance that will be needed to drive a wider service governance strategy.

- Support - Plan for the support guidance that will be needed to drive a wider service governance strategy.

- Communications - Plan for the communications guidance that will be needed to drive a wider service governance strategy.

- Road Map - Plan for the road map guidance that will be needed to drive a wider service governance strategy.

- Issues - Plan for the issue guidance that will be needed to drive a wider service governance strategy.

- Change Log - Plan for the change log guidance that will be needed to drive a wider service governance strategy.

- Monitoring - Plan for the monitoring guidance that will be needed to drive a wider service governance strategy.

- Testing - Plan for the testing guidance that will be needed to drive a wider service governance strategy.

- Performance - Plan for the performance guidance that will be needed to drive a wider service governance strategy.

- Observability - Plan for the observability guidance that will be needed to drive a wider service governance strategy.

- Caching - Plan for the caching guidance that will be needed to drive a wider service governance strategy.

- Encryption - Plan for the encryption guidance that will be needed to drive a wider service governance strategy.

- Security - Plan for the security guidance that will be needed to drive a wider service governance strategy.

- Terms of Service - Plan for the TOS guidance that will be needed to drive a wider service governance strategy.

- Privacy - Plan for the privacy guidance that will be needed to drive a wider service governance strategy.

- Service Level Agreements - Plan for the SLA guidance that will be needed to drive a wider service governance strategy.

- Licensing - Plan for the licensing guidance that will be needed to drive a wider service governance strategy.

- Branding - Plan for the branding guidance that will be needed to drive a wider service governance strategy.

- Regulation - Plan for the regulation guidance that will be needed to drive a wider service governance strategy.

- Discovery - Plan for the discovery guidance that will be needed to drive a wider service governance strategy.

- Client - Plan for the client guidance that will be needed to drive a wider service governance strategy.

- Command Line Interface - Plan for the CLI guidance that will be needed to drive a wider service governance strategy.

- SDKs - Plan for the SDK guidance that will be needed to drive a wider service governance strategy.

- Plugin - Plan for the plugin guidance that will be needed to drive a wider service governance strategy.

- IDE - Plan for the IDE guidance that will be needed to drive a wider service governance strategy.

- Browsers - Plan for the browser guidance that will be needed to drive a wider service governance strategy.

- Embeddable - Plan for the embeddable guidance that will be needed to drive a wider service governance strategy.

- Bots - Plan for the bots and automation guidance that will be needed to drive a wider service governance strategy.

- Visualization - Plan for the visualization guidance that will be needed to drive a wider service governance strategy.

- Analysis - Plan for the analysis guidance that will be needed to drive a wider service governance strategy.

- Aggregation - Plan for the aggregation guidance that will be needed to drive a wider service governance strategy.

- Integration - Plan for the integration guidance that will be needed to drive a wider service governance strategy.

- Network - Plan for the network guidance that will be needed to drive a wider service governance strategy.

- Regions - Plan for the regional guidance that will be needed to drive a wider service governance strategy.

- Webhooks - Plan for the webhooks guidance that will be needed to drive a wider service governance strategy.

- Migration - Plan for the migration guidance that will be needed to drive a wider service governance strategy.

- Backup - Plan for the backup guidance that will be needed to drive a wider service governance strategy.

- Real Time - Plan for the real time guidance that will be needed to drive a wider service governance strategy.

- Voice - Plan for the voice enablement guidance that will be needed to drive a wider service governance strategy.

- Spreadsheets - Plan for the spreadsheet guidance that will be needed to drive a wider service governance strategy.

- Investment - Plan for the investment guidance that will be needed to drive a wider service governance strategy.

- Monetization - Plan for the monetization guidance that will be needed to drive a wider service governance strategy.

- Plans - Plan for the plan guidance that will be needed to drive a wider service governance strategy.

- Partners - Plan for the partner guidance that will be needed to drive a wider service governance strategy.

- Certification - Plan for the certification guidance that will be needed to drive a wider service governance strategy.

- Evangelism - Plan for the evangelism guidance that will be needed to drive a wider service governance strategy.

- Showcase - Plan for the showcase guidance that will be needed to drive a wider service governance strategy.

- Deprecation -Plan for the deprecation guidance that will be needed to drive a wider service governance strategy.

- Training - Plan for the training guidance that will be needed to drive a wider service governance strategy.
