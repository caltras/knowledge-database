# CSS

1. Use var() function to change properties easily.

    Ex.:
    
        //style.css
        :root { 
            --bg-color: #ddd;
        }
        .container {    
            background-color: var(--bg-color);
        }
        
        //javascript
        document.documentElement.style.setProperty("--bg-color", "#333"
    
  
  
  
