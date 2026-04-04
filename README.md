<link rel="shortcut icon" type="image/png" href="appleT2.png">

<h1 align="center">NicheFruit</h1>

<p align="center">
  <img src="appleT2.png" width="400" alt="NicheFruit Logo"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white"/>
  <img src="https://img.shields.io/badge/Focus-Backend%20&%20Frontend%20Development-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Status-Kinda%20Active-brightgreen?style=for-the-badge"/>
  <img src="https://img.shields.io/github/followers/NicheFruit?style=for-the-badge&logo=github"/>
</p>

---

## 🗞️ About Me

I enjoy experimenting with concepts that challenge normal logic while staying organized and thoughtful. I’m always curious about how systems work, whether in code, design, or storytelling, and I enjoy breaking problems into pieces to find clever solutions.

This curiosity inspires both my creative projects and my technical work, driving me to experiment, learn, and create things that are both functional and imaginative.
When I’m not programing or building projects, I enjoy exploring new ideas, testing unconventional approaches, and pushing boundaries to see what’s possible. I like projects that mix logic and creativity, and I find satisfaction in turning abstract concepts into something tangible and useful.

---

## 💻 Programming & Development

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,github,eclipse,robloxstudio"/>
</p>

- Primary Language: **Java** ☕  
- Interests: Shi, I'll do anything.  
- Focus: Mostly clean, scalable, object-oriented applications

🔗 GitHub: [https://github.com/NicheFruit](https://github.com/NicheFruit)

---

## Java Example

```java
package JPanelArrayTest;
import javax.swing.*;
import java.awt.*;

public class Main {

    public static void main(String[] args) {

        try {
            String answer = JOptionPane.showInputDialog(null, "Enter a #:", "Size Input", JOptionPane.INFORMATION_MESSAGE);

            int enteredNum = Integer.parseInt(answer);

            Main.setTiles(enteredNum, enteredNum);

        } catch(Exception e) {
            System.err.println("No variables were entered, or number was too large!.\nEntered 16x16 as a default numbers.");

            int enteredNum1 = 16;
            int enteredNum2 = 16;

            JOptionPane.showMessageDialog(null, "No variable were entered, or number was too large!\n16x16 were set default numbers.", "ERROR", JOptionPane.ERROR_MESSAGE);
            Main.setTiles(enteredNum1, enteredNum2);
        }
    }
    private static void setTiles(int x, int y) {

        ImageIcon icon = new ImageIcon("src/JPanelArrayTest/Jolly.png");
        Image image = icon.getImage();
        Image scaledImage = image.getScaledInstance(75, 75, Image.SCALE_SMOOTH);
        ImageIcon scaledIcon = new ImageIcon(scaledImage);

        Main.Frame frame = new Main.Frame("Box Colors");
        frame.setIconImage(scaledIcon.getImage());

        Tiles[] tile = new Tiles[x*y];

        int sizeX = frame.getWidth() / x;
        int sizeY = frame.getHeight() / y;

        int tileX = 0;
        int tileY = 0;

        for (int i = 0; i < x * y; i++) {
            tile[i] = new Tiles(sizeX, sizeY, tileX, tileY);
            frame.add(tile[i]);

            tileX += sizeX;

            if (tileX >= frame.getWidth()) {
                tileX = 0;
                tileY += sizeY;
            }

            System.out.println("Box #" + i + "\nX: " + tileX + "\nY: " + tileY);
            frame.repaint();
        }
    }

    public static class Frame extends JFrame {
        Frame(String title) {
            this.setTitle(title);
            this.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
            this.setResizable(false);
            this.setSize(500, 500);
            this.getContentPane().setBackground(Color.WHITE);
            this.setLocationRelativeTo(null);
            this.setLayout(null);
            this.setVisible(true);
        }
    }
}
```

---

## 📂 Downloads & Resources

<p align="center">
  <a href="https://sourceforge.net/u/nichefruit/profile/">
    <img src="https://img.shields.io/badge/Downloads-SourceForge-orange?style=for-the-badge&logo=sourceforge"/>
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Games-Coming%20Soon-blueviolet?style=for-the-badge&logo=unity"/>
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Websites-Coming%20Sooon-FFD700?style=for-the-badge&logo=google-chrome&logoColor=white"/>
  </a>
  <a href="#">
    <img src="https://img.shields.io/badge/Tutorials-Videos-red?style=for-the-badge&logo=youtube"/>
  </a>
  <a href="https://forms.gle/DVhy9jQ45dG45J7z7">
    <img src="https://img.shields.io/badge/Uploads-Forms-green?style=for-the-badge&logo=googleforms"/>
  </a>
</p>

---

<p align="center">
  Thanks for visiting!
</p>
