void main() {
  // Create an object based on the class
  User userOne = User();
  print(userOne.username);
  print(userOne.age);
  userOne.login();
  
}

// Just creates the class
class User {
  String username = 'jason';
  int age = 25;
  
  void login() {
    print('user logged in');
  }
}
