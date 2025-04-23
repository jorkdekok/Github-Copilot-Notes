# Unit tests
Create unit tests using xunit and moq.
 
If you create mock services or variables, put Mock at the end like so:
```csharp
private readonly Mock<IProjectsClient> _projectsClientMock = new();
var apiResponseMock = new Mock<IApiResponse>();
```
 
The name of your test should consist of three parts:
- The name of the method being tested.
- The scenario under which it's being tested.
- The expected behavior when the scenario is invoked.
Something like: 
```
<method name>_<scenario>_<expected behavior>
```
 
Also use .Verify to test how many times an injected service or client is called.

\_loggerMock should be verified like this:
```csharp
_loggerMock.Logger
	.Verify(x => x.Log(
		It.IsAny<LogLevel>(),
		It.IsAny<EventId>(),
		It.IsAny<It.IsAnyType>(),
		It.IsAny<Exception>(),
		It.IsAny<Func<It.IsAnyType, Exception?, string>>()),
	Times.Once);
```

 
Create tests so that all lines of code are covered.
If possible use [Theory] to test extensively and cover all lines of code. Also test the exceptions if any.

Also use the Builder pattern to create objects in the arrange section of the unit tests.

# Code style
Use the following code style:
- Use the Microsoft naming convention.
- Use record structs for DTOs.
