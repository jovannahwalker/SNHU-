import javafx.application.Application;
import javafx.scene.Scene;
import javafx.scene.control.ListView;
import javafx.scene.layout.VBox;
import javafx.stage.Stage;
import javafx.scene.image.Image;
import javafx.scene.image.ImageView;
import javafx.scene.control.Hyperlink;
import javafx.scene.text.Text;
import javafx.scene.text.Font;

// Main class of the JavaFX application
public class DestinationApp extends Application {
    @Override
    public void start(Stage primaryStage) {
        // Set the title of the primary stage
        primaryStage.setTitle("Top Five Destinations");

        // Create a ListView to hold VBoxes for each destination
        ListView<VBox> listView = new ListView<>();
        listView.getItems().addAll(
            createItem("Paris", "The City of Light, known for its art and culture.", "paris.jpg", "https://travel.example.com/paris"),
            createItem("Tokyo", "A bustling metropolis with a unique blend of traditional and modern.", "tokyo.jpg", "https://travel.example.com/tokyo"),
            createItem("New York", "The city that never sleeps, offering endless activities.", "newyork.jpg", "https://travel.example.com/newyork"),
            createItem("London", "Famous for its history and landmarks like the Big Ben.", "london.jpg", "https://travel.example.com/london"),
            createItem("Sydney", "Known for its Sydney Opera House and beautiful beaches.", "sydney.jpg", "https://travel.example.com/sydney")
        );

        // Set the scene with the listView and fixed size
        Scene scene = new Scene(listView, 400, 500);
        primaryStage.setScene(scene);
        primaryStage.show();
    }

    // Helper method to create a VBox containing destination details
    private VBox createItem(String name, String description, String imagePath, String url) {
        // Text component for the destination name with specific styling
        Text destinationName = new Text(name);
        destinationName.setFont(Font.font("Arial", 20));

        // Text component for the short description of the destination
        Text shortDescription = new Text(description);

        // Image component representing the destination
        Image image = new Image(getClass().getResourceAsStream(imagePath));
        ImageView imageView = new ImageView(image);
        imageView.setFitHeight(100); // Set image height
        imageView.setFitWidth(200);  // Set image width

        // Hyperlink to a top-selling travel package for the destination
        Hyperlink link = new Hyperlink("View package");
        link.setOnAction(e -> getHostServices().showDocument(url)); // Action to open the link in a browser

        // VBox layout to stack each element vertically
        VBox box = new VBox(10, destinationName, shortDescription, imageView, link);
        return box;
    }

    public static void main(String[] args) {
        launch(args); // Launch the JavaFX application
    }
}
