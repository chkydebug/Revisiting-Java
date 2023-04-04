import java.awt.Color;
import java.awt.Dimension;
import java.util.Scanner;
import javax.swing.JFrame;
import javax.swing.JPanel;

public class HexToColor {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a hexadecimal value of maximum 6 characters to generate its corresponding RGB values: ");
        String hex = sc.nextLine();
        Color color = Color.decode("#" + hex);
        JFrame frame = new JFrame();
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        
        JPanel panel = new JPanel();
        panel.setBackground(color);
        panel.setPreferredSize(new Dimension(500, 500));
        
        frame.getContentPane().add(panel);
        frame.pack();
        frame.setVisible(true);
        int r = Integer.parseInt(hex.substring(0, 2), 16);
        int g = Integer.parseInt(hex.substring(2, 4), 16);
        int b = Integer.parseInt(hex.substring(4, 6), 16);
        System.out.println("The RGB values are: " + r + ", " + g + ", " + b);
    }
}
