# Uebung08_01

package org.hsd.inflab.Uebung08;

import javafx.application.Application;
import javafx.scene.Scene;
import javafx.scene.layout.BorderPane;
import javafx.scene.paint.Color;
import javafx.scene.shape.Rectangle;
import javafx.stage.Stage;


public class App extends Application {

    @Override
    public void start(Stage stage) {
        
    	try {
    		
    		BorderPane fenster = new BorderPane();
    		Scene buehne = new Scene(fenster,400,400);
    		
    		//Figuren
    		Rectangle flaggenmast =  new Rectangle();
    		Rectangle flaggeAbschnitt_1 =  new Rectangle();
    		Rectangle flaggeAbschnitt_2 =  new Rectangle();
    		Rectangle flaggeAbschnitt_3 =  new Rectangle();
    		
    		//Größer der Figuren
    		flaggenmast.setX(100);
    		flaggenmast.setY(100);
    		flaggenmast.setWidth(5);
    		flaggenmast.setHeight(400);
    		
    		flaggeAbschnitt_1.setX(105);
    		flaggeAbschnitt_1.setY(100);
    		flaggeAbschnitt_1.setWidth(200);
    		flaggeAbschnitt_1.setHeight(50);
    		
    		flaggeAbschnitt_2.setX(105);
    		flaggeAbschnitt_2.setY(150);
    		flaggeAbschnitt_2.setWidth(200);
    		flaggeAbschnitt_2.setHeight(50);	
    		
    		flaggeAbschnitt_3.setX(105);
    		flaggeAbschnitt_3.setY(200);
    		flaggeAbschnitt_3.setWidth(200);
    		flaggeAbschnitt_3.setHeight(50);
    		
    		//Farben der Figuren
    		flaggenmast.setFill(Color.GRAY);
    		flaggeAbschnitt_1.setFill(Color.BLACK);
    		flaggeAbschnitt_2.setFill(Color.RED);
    		flaggeAbschnitt_3.setFill(Color.YELLOW);
    		
    		//Figuren einbinden
    		fenster.getChildren().add(flaggenmast);
    		fenster.getChildren().add(flaggeAbschnitt_1);
    		fenster.getChildren().add(flaggeAbschnitt_2);
    		fenster.getChildren().add(flaggeAbschnitt_3);
    		
    		//Figuren anzeigen
    		stage.setTitle("Flagge");
    		stage.setScene(buehne);
    		stage.show();
    		
    	}
    	catch (Exception e) {
    		e.printStackTrace();    		
    	}
    }

    public static void main(String[] args) {
        launch();
    }

}
