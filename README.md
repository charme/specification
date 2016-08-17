[![Author](http://img.shields.io/badge/Project-@CharmeAPI-blue.svg?style=flat-square)](https://twitter.com/CharmeAPI)
[![Author](http://img.shields.io/badge/Author-@cziegenberg-blue.svg?style=flat-square)](https://twitter.com/cziegenberg)

# Charm API Specification (wip)

## Abstract
***Charme*** is the French word for charm, or "the ability to persuade, delight or arouse admiration", and this is the best description for the aim of this specification.

The Charme API Specification defines an overall data format for modern APIs which enables clients and servers to exchange their data in a standardized way. It's designed to be protocol independent and easy to implement. It's suitable for small APIs, but offers many optional features to also fulfill the requirements of more complex APIs.

It's inspired by [JSON API](http://jsonapi.org), but eliminates its known limitations and issues.

## Main Features
### Communication
- The specification is protocol independent. The first version will include support for HTTP and WebSockets.
- The communication between client and server can be synchronous or asynchronous.
- Multiple commands can be send in one request.
- Requests can be processed asynchronously, no matter if the communication is synchronous or asynchronous.

### Resources
- Although resources are part of the core specification, they are fully optional. The API can use the core functionality with self-defined operations and data formats.
- Resource revisions can be supported.
- Soft deletes for resources can be supported.
- Clients can be allowed to access and restore previous revisions or previously deleted resources, resulting in a full undo functionality.
- Resource data can optionally be localized.
- Resources can be searched, filtered, sorted...

### Security
- Defined versioning rules for the API and the specification - clients and servers can independently be updated to newer versions, without the risk of breaking anything.
- Full data consistency for resource modifications.

### Misc
- Optional support for [JSON-LD](http://json-ld.org).

### Planned
- Automatic discovery of the API for documentation and client generation.

## Current Status
- Separation of the specification draft into multiple independent parts.
- Creation of clients and servers for different protocols.
- Validation and completion of the specification.

## Be a part of it!
The project just started, and a first preview version of the spec will be published as soon as possible. Nevertheless you can tell us which limitations of other API specifications like JSON API are currently a problem for you - create an issue for, explain the problem and suggest a solution that would solve it for you.
