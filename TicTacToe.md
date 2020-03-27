### TicTacToe Java Assignment

##### Introduction
For this assignment, you will make a Swing application for the game Tic-Tac-Toe. Although you could make a Tic-Tac-Toe game with a
larger grid, we will be using a 3 x 3 Tic-Tac-Toe board for this assignment. 

Assignment Structure
1. 2-player TicTacToe game on a 3 x 3 grid
2. *Short Extension* 2-player TicTacToe game on a larger grid
2. *Hard Extension* 1-player TicTacToe game on a 3 x 3 grid
3. *Harder Extension* 1-player TicTacToe game on a larger square grid

##### Tips
1. You might want to have a 2D array of JButton objects to simplify your getWin() function. You should be able to write a couple of loops to help you check for the different "win conditions".
2. Have your JPanel class **implement** the **ActionListener** interface. Your JPanel class will now have *at least* one required method, **public void actionPerformed(ActionEvent e)**. All of your JButtons should now refer to this method whenever they are clicked. You can get the text of a button (as well as it's name) from the **ActionEvent e** parameter.
```java
public void actionPerformed(ActionEvent e){
  
  // Reference variable to the original button that was clicked. 
  // That means we can modify the JButton instance and our program will know what to do!
  JButton buttonClicked = (JButton) e.getSource();
  String buttonName = buttonClicked.getName();
  String buttonText = buttonClicked.getText();
  buttonClicked.setText("I have been clicked");

}
```
3. You might want to use the **GridLayout()** layout manager. Write the following code in your JPanel constructor to help accomplish this. When you add Swing components to your JPanel, they will add from left to right, top to bottom to fill up the 3 x 3 grid. See why a 2D array of JButton objects might help here?
```java
this.setLayout(new GridLayout(3,3));
```
4. There are a couple of useful JButton methods we haven't talked about yet.
```java
JButton testButton = new JButton("Test Button");
testButton.setName("1");
testButton.setText("Button Clicked);
String buttonName = testButton.getName();
String buttonText = testButton.getText();
```

##### Requirements
Your project should contain the following files (no more):
1. RunProgram.java
2. MainFrame.java
3. Board.java

Your Board class should contain the following class variables (CV), class methods (CM), and constructors (CC):
1. (CV) private JButton[][] grid;
2. (CV) private boolean xTurn;
3. (CC) public Board()
4. (CM) public String getWin()
5. (CM) public void ActionPerformed(ActionEvent e)


 
