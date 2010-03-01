# Build Instructions #
To build the SWC for this library, run the build.xml found in the root of this project with its 
default settings.  Please note that the environment variable FLEX_HOME must be set for this build 
to function correctly.  Please also note that the FlashBuilder project is an application setup to
execute the FlexUnit tests using the UIListener rather than the built-in FlexUnit4 support;
the project cannot be used as a library project.

# Examples #
http://github.com/blegros/flexRpcStubs/tree/master/src/test/flex/mx/rpc/http/test/sample/ - for an 
example using HTTPServiceStub to create a unit test for a domain/model class which has an HTTPService 
dependency.

http://github.com/blegros/flexRpcStubs/tree/master/src/test/flex/mx/rpc/remoting/test/sample/ - for an
example using RemoteObjectStub to create a unit test for controller class which has a RemotObject 
dependency.

DISCLAIMER: Please note these example unit tests are meant to serve as examples only.  They are not 
intended to infer best practices or dictate preferred implementations.

# Change Log #
## 0.2 ## 
- Added support for Hamcrest matchers within parameters to HTTPServiceStub and RemoteObjectStub
- Added support for header matching on HTTPServiceStub
- Added more detailed samples for using HTTPServiceStub and RemoteObjectStub

## 0.1 ## 
- Initial import of project from http://brianlegros.com/blog

# Roadmap #
- Add a support for matching method on HTTPService
- Add a stub for the HTTPMultiService class
- Add a WebServiceStub
- Add better error handling
   