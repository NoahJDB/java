package me.boydsmit.les8;

//Importeren van gebruikte classes
import javafx.animation.*;
import javafx.application.Application;
import javafx.scene.control.TextField;
import javafx.scene.paint.Color;
import javafx.scene.shape.Circle;
import javafx.scene.text.Text;
import javafx.stage.Stage;
import javafx.scene.Scene;
import javafx.scene.Group;
import javafx.scene.control.Button;
import javafx.scene.image.ImageView;
import javafx.scene.image.Image;
import javafx.util.Duration;

public class Template extends Application {  //zorg dat de class overerft van Application

    public void start(Stage stage) {   //geef de stage mee als argument
        //creeer de "root node" Group
        Group rootNode = new Group();
        //Maak een nieuwe Scene met daarin de "root node" Group (verzameling nodes)
        Scene scene = new Scene(rootNode, 800, 600);
        //plaats de Scene op de Stage
        stage.setScene(scene);

        //inladen van een Image in een ImageView
        Image image = new Image("http://www.zombieplace.com/zombiecats/your-child-watched-too-many-zombie-movies.jpg", true);
        ImageView iv = new ImageView();
        iv.setImage(image);

        //een extra group is optioneel als je meer groepen wilt hebben
        Group group1 = new Group();

        rootNode.getChildren().add(group1);

        group1.getChildren().add(iv);

        Button button = new Button("ik ben een Button");
        button.relocate(50,50);
        rootNode.getChildren().add(button);



        Circle newCircle = new Circle();
        newCircle.relocate(80, 80);
        newCircle.setCenterX(30);
        newCircle.setCenterY(30);
        newCircle.setRadius(90);
        newCircle.setFill(Color.BLUE);
        group1.getChildren().add(newCircle);


        TextField newTextField = new TextField();
        newTextField.relocate(60, 90);
        group1.getChildren().add(newTextField);


        Text newText = new Text("Opdracht 3 Node");
        newText.relocate(60, 120);
        newText.setFill(Color.WHITE);
        group1.getChildren().add(newText);



        TranslateTransition translateTransition = new TranslateTransition(Duration.millis(750));
        translateTransition.setToX(70);
        translateTransition.setToY(390);

        FillTransition fill = new FillTransition(Duration.millis(750), Color.RED, Color.YELLOW); //voor transition


        ParallelTransition transition = new ParallelTransition(newCircle, translateTransition, fill);
        transition.setCycleCount(Timeline.INDEFINITE);
        transition.setAutoReverse(true);

        transition.play();

        //laat de stage en inhoud renderen met de show() method
        stage.show();

        //Opdracht 0
        //Lees in de javafx API reference wat alle geimporteerde classes doen.
        //Stel vragen als je iets niet begrijpt.

        //Opdracht 1
        //Wat gebeurt er als je de ImageView iv aan de group1 Group toevoegt,
        //en je de button toevoegt aan de rootNode Group?
        //Probeer het uit en verklaar wat er gebeurt en waarom dat zo is...
        //Zet je verklaring in een comment hieronder...
        // Er veranderd niks




        //Opdracht 2
        //Zoek uit in de javafx API reference naar de class TextField
        //Kijk in welke package de class zit en importeer deze
        //Maak in de start method een textField aan en plaats deze in de group1 Group
        //Gebruik de relocate() method om het textveld netjes onder de knop te plaatsen


        //Opdracht 3
        //Kies nog een ongebruikt type node uit en plaats deze in het scherm onder het TextField


        //Opdracht 4
        //Teken een cirkel achter je knop en je textField


        //Opdracht 5
        //Lees de volgende tutorial door en laat de cirkel stuiteren tussen de onder- en bovenkant van je scherm
        //Tutorial: http://docs.oracle.com/javase/8/javafx/scene-graph-tutorial/scenegraph.htm#JFXSG107


        //Extra Opdracht 6
        //Zorg dat de cirkel tijdens het stuiteren van kleur verandert

        //Extra Opdracht 7
        //Voor een 10!
        //Zie de uitleg in de presentatie

    }
}
