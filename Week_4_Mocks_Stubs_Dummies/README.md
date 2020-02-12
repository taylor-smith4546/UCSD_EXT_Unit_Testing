# UCSD Extension: Unit Testing: Supporting Modern Software Development Methods

## Videos: 

[Lecture 4: Mocks, Stubs and Test Spies](URL link here)

## Assignment/Classwork:

Quiz #4 (Canvas)

Exercise #1:

User Service Tested

Write a happy-path test for the class presented below. Verify that the user gets his new password, and
that the updateUser() method of userDAO is called.

```java
public class UserServiceImpl {
 private UserDAO userDAO;
 private SecurityService securityService;
 public void assignPassword(User user) throws Exception {
 String passwordMd5 = securityService.md5(user.getPassword());
 user.setPassword(passwordMd5);
 userDAO.updateUser(user);
 }
 public UserServiceImpl(UserDAO dao, SecurityService security) {
 this.userDAO = dao;
 this.securityService = security;
 }
}
```

## Topics Covered: 

o	Introducing Mockito

o	Types of Test Double

o	Putting it all together


## Supplementary Items (Please Read!)

[Mockito main reference documentation](https://javadoc.io/doc/org.mockito/mockito-core/latest/org/mockito/Mockito.html)

[TestDouble - Martin Fowler](https://martinfowler.com/bliki/TestDouble.html)

[The Difference Between Mocks & Stubs - Martin Fowler](https://martinfowler.com/articles/mocksArentStubs.html)

[The hitchhiker guide to test doubles](https://dev.to/docplannertech/the-hitchhiker-guide-to-test-doubles-53m3)

[Stubbing and Mocking with Mockito and JUnit](hhttps://semaphoreci.com/community/tutorials/stubbing-and-mocking-with-mockito-2-and-junit)

