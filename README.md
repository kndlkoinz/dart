# dart

void main() {
  // Create an object based on the class
  User userOne = User('jk', 4);
  print(userOne.username);
 
  User userTwo = User('bo', 7);
  print(userTwo.age);
  
  SuperUser userThree = SuperUser('Dan', 48);
  print(userThree.age);
  userThree.publish();
  
}

// Just creates the class
class User {
  
  String username;
  int age;
  
  // constructor
  User(String username, int age){
    this.username = username;
    this.age = age;
  }
  
 void login() {
   print('user logged in');
  }
}

class SuperUser extends User {
  
  // constructor
  SuperUser(String username, int age): super(username, age);
  void publish() {
    print("Publish!");
  }
}

