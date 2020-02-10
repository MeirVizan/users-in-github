# users-in-github


    written by :
    Meir Vizan
   
    
        install:npm install
        SERVER:npm start
        URL:locallhost:3000/login
        Name:admin
        password:1234
        firs log in then you get an access for admin.ejs
    
    Design
    
        Folowing the MVC model
        View folder: all client side files login.ejs,admin.ejs header.ejs and footer.ejs
        Controlers: routs functions
        DB: using sqlite the fields are: the names of github who were saved by user.

    
    <h4>LOGIN</h4>
    
           Using cookies and session to save browser id and to recognize if user already loged.
           Name:admin
           password:1234

    
    ADMIN.ejs
    Search button
           Hard coded url to github and get gits json. 
           When  a name is typed and the name exist, then there is an option to save it including his repo and followers
    

    Save button
          When save button is clicked then the name is saved in an array in the level of js client side <br>
          but also passed to server side by using the main server. App.js. app.js calls to users.js and call to the save function<br>
          Save function deals with DB sqlite and stores it inn that DB<br>
    
    Delete
          When delete button is clicked on the client side, it deletes the name (a url to the names account in github)
          From client side and also from server side by interacting  with the main server app.js. app.js calls to users.js and call to             the delete function.
           Delete function deletes the name from DB sqlite

    






