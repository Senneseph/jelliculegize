# TODO

This is OPERATION CODENAME PROJECT CYBERDECK

Terminology:

- Cyberdeck - this is a standard web browser + whatever hardware it's on
- Cyberdeck Launcher - this is a meta application that will help manage Cyberdeck Apps as well as the Cyberdeck itself.
- Cyberdeck App - a PWA that is installable via the Cyberdeck (browser), it is shorthand for Cyberdeck Application - the long form is associated with heavier-weight, server style applications.

These are the name of the software libraries that will enable this project. Essentially, we are using existing and prevalent web standards to create a standarized set of conventions to build, test, distribute, administer, and interact with technology.  We will have a UI with an API specification, which will talk to a normal application API, which again, will be OpenAPI and this application API goes both ways - input / output.

jcule is a specification and library for creating Cyberdeck Applications a user interface library for the web.  Specifically, PWAs + SPA.  It provides libraries necessary to create and build these apps.

jellicule is a specification and software library for a semantic library of User Interface components and how to translate them into an OpenAPI specification. it provides some simple javascript, html, and css conventions and libraries necessary to create a jcule app. building the jellicule project results in a UI builder for jellicule apps. You can practice creating a UI and mapping it to different OpenAPI specifications. You are essentially defining a view.

jcx is a tool that takes the jcule specification and the jellicule library and helps a user create, extend, or adapt an app. Unlike `npm` or `git`, it is not a command-line application. It requires only `docker-compose up -d` and the the user will have a development environment with their choice of command line or web interface. It will automatically go out and get the jcule, jellicule, jelliculegize, transcribulator libraries.

transcribulator: a tool to help transcribe, transcode, transliterate, transpile, etc foreign code into WASM, TypeScript, Rust, or JavaScript. We are targeting the browser, if it can run there, it is already OK, we just have to make it work.

jelliculegize helps adapt, configure, and import jcule apps and UIs.

jucle-open-adapt: part of jelliculegize, provides an quick way to build UIs for OpenAPI specifications.As an example: the Pet Store API has an OpenAPI specification for accessing its services and defines their aspects. But there is no UI. This is where jelliculegize can come in. The service's OpenAPI already exists and works, we just need to create our preferred way of interacting with it by defining UI elements and their rules. We will define the UI with an OpenAPI-compatible spec, using our jellicule semantic language library and entity database.

jcule-tsx: the jecule transcriber is part of jelliculegize. This is a standard app we will build which will take a normally command line software package and attempt to build a jcule UI for it. For example, we have FFMPEG with its command line options and outputs.  We document all of these as an OpenAPI specification and then we separately decide how we want to build a flexible UI for it.  It's essentially a WYSIWYG Drag n' Drop, editable UI. it takes a command line application that is pre-jcule and brings it into our ecosystem. Its main purpose is to take command line applications and semi-automatically create separate OpenAPI specifications for its UI, inputs, and outputs. Besides this, it will also attempt to take the source code of the application and convert it WASM, TypeScript, Rust, or JavaScript. jcule will specify its own, shared, and always pinned package notation for these transcribulated applications. language, environment, package system, application name, developer identity, etc should be considererd, but we don't want to overcomplicate it.  For now, the namespace will be identicaly to github because that is our package system.  So if there is an official `ffmpeg` source code on github, we would start with that repository's name.

We need to get started on planning and building the jelliculegize project.
