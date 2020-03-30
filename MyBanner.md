### MyBanner Homework Assignment

##### Purpose
The purpose of the assignment is to get you all familiar with JFrames, JPanels, and JLabels. These Swing components will be used 
extensively throughout the rest of the semester!

##### Description
You should create a graphical window to display information about a dream vacation destination. Think of this like a mini-advertisement.
You may use different background colors, JPanels/JFrames, JLabels, and even Layout Managers if you would like! Refer to the posted 
videos for some ideas and maybe some inspiration.

Note: *your vacation destination does **not** need to be a summer destination. Get creative and think about a cool 
location you would like to advertise!*

##### Requirements
1. At least one [JFrame](https://docs.oracle.com/javase/7/docs/api/javax/swing/JFrame.html)
2. At least on [JPanel](https://docs.oracle.com/javase/7/docs/api/javax/swing/JPanel.html)
3. At least 2 different background colors (for any Swing component)
4. At least 3 JLabels or [JTextAreas](https://docs.oracle.com/javase/7/docs/api/javax/swing/JTextArea.html) at different locations in your program

##### Hints
1. JTextAreas can display more than one line at a time. Use the escape sequence ***\n*** to indicate the start of a new line you would 
like to show.
2. You can place a Swing component at an arbitrary location using the code below. This example is for a JLabel. This does **not** use a
Layout Manager...

```java
// In the constructor of the JFrame OR JPanel class
int xLoc = 100;
int yLoc = 100;
int width = 300;
int height = 100;

this.setLayout(null);
JLabel myLabel = new JLabel("Mr. v");
this.add(myLabel);
myLabel.setBounds(xLoc, yLoc, width, height);
```

3. You can give a JLabel a background color using the following code snippet...

```java
// In the constructor of the JFrame or JPanel class
JLabel myLabel = new JLabel("Mr. v");
myLabel.setOpaque(true);
myLabel.setBackground(Color.cyan);
```

4. When looking for a color, the following are the most popular/easiest to use...
```java
// In the constructor of the JFrame or JPanel class
JLabel myLabel = new JLabel("Mr. v");
myLabel.setOpaque(true);
myLabel.setBackground(Color.red);
myLabel.setBackground(Color.orange);
myLabel.setBackground(Color.yellow);
myLabel.setBackground(Color.green);
myLabel.setBackground(Color.blue);
myLabel.setBackground(Color.pink);
myLabel.setBackground(Color.black);
myLabel.setBackground(Color.gray);
myLabel.setBackground(Color.lightGray);
myLabel.setBackground(Color.white);
myLabel.setBackground(Color.magenta);
```
##### Extension Credit
1. Try adding an image into your project! The image should be .jpg or .png and should be saved in the same folder as your other Java
project files.
```java
// IMPORT AT TOP OF FILE
import javax.imageio.ImageIO;
import javax.swing.*;
import java.awt.*;
import java.awt.image.BufferedImage;
import java.io.File;
import java.io.IOException;

// ...

BufferedImage myImage = null;
try {
    myImage = ImageIO.read(new File("file-name"));
} catch (IOException e) {
    e.printStackTrace();
}
JLabel myLabel = new JLabel(new ImageIcon(myImage));
this.add(myLabel);

// ...
```

