

import java.io.File;
import java.io.FileInputStream;
import java.io.InputStream;
import java.util.Properties;
import java.util.*;
import java.io.*;

public class ConfigWriter {
	
	public  void changeVideoURL(String elementID, String resourceVal){
		Properties props = new Properties();
	    InputStream is = null;
	 
	    	 
	    try {
	        if ( is == null ) {
	            // Try loading from classpath
	            is = getClass().getResourceAsStream("/videoResources.properties");
	        }
	 
	        // Try loading properties from the file (if found)
	        props.load( is );
			is.close();
	    }
	    catch ( Exception e ) { 
	    	
	    	System.out.println(e.getMessage());;
	    	}
		File configFile=getClass().getResource("/videoResources.properties");
		FileOutputStream out = new FileOutputStream(configFile);
		props.setProperty(elementID, resourceVal);
		props.store(out, null);
		out.close();
	    
	}

		
	}


