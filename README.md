# JAM-Sharepoint
This is our code for sharpoint.

/**
 * Your application code goes here
 */

package userclasses;

import java.net.*;

import generated.StateMachineBase;

import com.codename1.ui.*; 
import com.codename1.ui.events.*;
import com.codename1.ui.util.Resources;

/**
 *
 * @author Your name here
 */
public class StateMachine extends StateMachineBase {
    public StateMachine(String resFile) {
        super(resFile);
        // do not modify, write code in initVars and initialize class members there,
        // the constructor might be invoked too late due to race conditions that might occur
    }
    
    /**
     * this method should be used to initialize variables instead of
     * the constructor/class scope to avoid race conditions
     */
	protected void initVars(Resources res){
	}

    @Override
    protected void beforeHomePage(Form f) {
    
    }

    @Override
    protected void onLoginPage_LoginAction(Component c, ActionEvent event) {

    
    }

    @Override
    protected void onMain_MultiListAction(Component c, ActionEvent event) {

    
    }

    @Override
    protected void onMain_LogoutButtonAction(Component c, ActionEvent event) {

    
    }

    @Override
    protected void onResources_MultiListAction(Component c, ActionEvent event) {

    
    }

    @Override
    protected void onCalendar_ButtonAction(Component c, ActionEvent event) {

    
    }

    @Override
    protected void onMain_TeachersAction(Component c, ActionEvent event) {

    
    }

    @Override
    protected void onMain_CalendarAction(Component c, ActionEvent event) {

    
    }

    @Override
    protected void onMain_ResourcesAction(Component c, ActionEvent event) {
    	
    
    }

    @Override
    protected void onCalendar_Calendar1Action(Component c, ActionEvent event) {

    
    }

    public static void openWebpage(URI uri) {
        Desktop desktop = Desktop.isDesktopSupported() ? Desktop.getDesktop() : null;
        if (desktop != null && desktop.isSupported(Desktop.Action.BROWSE)) {
            try {
                desktop.browse(uri);
            } catch (Exception e) {
                e.printStackTrace();
            }
        }
    }

    public static void openWebpage(URL url) {
        try {
            openWebpage(url.toURI());
        } catch (URISyntaxException e) {
            e.printStackTrace();
        }
    }
    
    @Override
    protected void onResources_ButtonAction(Component c, ActionEvent event) {
    	{
    		URI hna = new URI("http://www.holynames-sea.org/");
    		openWebpage(hna);

    	}
    
    }

    @Override
    protected void onResources_Button1Action(Component c, ActionEvent event) {
    		
    
    }

    @Override
    protected void onResources_Button2Action(Component c, ActionEvent event) {

    
    }
}
