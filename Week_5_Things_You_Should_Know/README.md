# UCSD Extension: Unit Testing: Supporting Modern Software Development Methods

## Videos: 

[Lecture 5: Things You Should Know](URL link here)

## Assignment/Classwork:

Quiz #5 (Blackboard)

Exercise #1:

Design Test Cases: State Testing

A StringUtils class contains a reverse() method, with a signature as presented below. List test
cases, which would verify that this method really reverses the input String!

Signature of reverse method:

```java
public String reverse(String s) { ... }
```

Exercise #2:

Design Test Cases: Interactions Testing

UserServiceImpl class contains the assignPassword() method, as presented on Listing 7.36. The
method uses two collaborators to successfully perform its task: userDAO and securityService.

assignPassword() Method
```java
private UserDAO userDAO;
private SecurityService securityService;
public void assignPassword(User user) throws Exception {
 String passwordMd5 = securityService.md5(user.getPassword());
 user.setPassword(passwordMd5);
 userDAO.updateUser(user);
}
```

Design the test cases for this method! Please note that this time you will have to think not only
about the input parameters (user), but also about the values returned (or exceptions thrown!) by
securityService and userDAO.

## Topics Covered: 

o	What values to check?

o	How to fail a test?

o	Matchers

o	Reading test data from files
