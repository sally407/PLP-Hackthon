# PLP-Hackthon
The repository contains a hackthon activity
The following project was made successful by two devoted student developers Fadhili Mumo (fadhilimumo3673@gmail.com) and Salome Ogeya  (salomeogeya@gmail.com)
The following simple project is a portfolio developed in html.
It is divided into five major sections;   
    The first section contains the details of the subject owner.
    The second section contains the education background
    the Trird contains the interests of the owner
    The fourth contains the Projects in development.

    1. The user interface
The user interface is developed to be user friendly that most of the users attention with the ease of use and visual presentation.
The user inteface is logically architectured for ease of use.  
five colors were used all visually related and gives the user general satisfaction and the urge to interact with the product.
The product is made very interactive by the introduction of mouse change and visual presentating changes like text size and color changes when hovering over objects within the page. 


    2.Design of the product
The html is designed to only dispalay content on clicking relevant tablinks.
The tablinks are designated or designed as divisions with the tag (<div></div>)
Each division has a unique id(id="")
The five tablinks are grouped to belong to the same class (tablinks).
The navigation through the tablinks is made possible by a javasript function below.
<!-- creating a function called opentab with parameters (tabId) -->
<script>              
                  function opentab(tabId){
                   // Decalring a variable and storing the tabcontent value into it using method document.getElementsByClassName() -->
                      var tabContents=document.getElementsByClassName('tab-content');
                      var hide=document.getElementsByClassName('default');                      
                        //incrementing the value of the tab dispaly on each click using the for function
                        //assigning the value of i to the tabContents and hidding the previous values of the 
                        //[i] containing the tab contents using tabContents[i].style.display='none'; -->  
                      for(var i=0;i<tabContents.length; i++){
                            tabContents[i].style.display='none';                            
                       }
                       for(var i=0;i<hide.length; i++){
                        hide[i].style.display='none';
                   }
                        var tabs=document.getElementsByClassName('active-tab');
                        //incrementing the value of the tab display on each click using the for function
                        //assigning the value of i to the tabContents and removing the current content of active tab of the 
                        for(var i=0;i<tabs.length;i++){
                            tabs[1].classList.remove('tab-content');
                        }
                        document.getElementById(tabId).style.display='block';                        
                        //creating the connection between the function and the onlick action listerner.
                        document.querySelector('onclick="openTab(\''+tabId+'\')"]').classList.add('active-tab');
                    }
                    function hide(){
                      if(opentab(tabId)){
                        document.getElementById('open').style.display='none'
                      }
                    }
            </script>
The script function is then called to take effect on the tablinks using {
    <div class="tablinks" onclick="opentab('tab ID')"><f>Tab name</f></div>} 
The javascript function is made to coordinate the apperarnce and disapearnce of the division contents("tab-contents) on every action click on the tablinks.    

            3. External links
The html documents contain external links to our emails, our downloadable CVs, github repositories with our current progress and our telephone numbers.           
          

       
