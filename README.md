# users-in-github


    <h2>written by :</h2>
    <h4>Meir Vizan</h4>
   
    
        install:npm install<br>
        SERVER:npm start<br>
        URL:locallhost:3000/login<br>
        Name:admin<br>
        password:1234
        firs log in then you get an access for admin.ejs
    
    Design
    
        Folowing the MVC model <br>
        View folder: all client side files login.ejs,admin.ejs header.ejs and footer.ejs<br>
        Controlers: routs functions <br>
        DB: using sqlite the fields are: the names of github who were saved by user.<br>

    
    <h4>LOGIN</h4>
    
           Using cookies and session to save browser id and to recognize if user already loged.<br>
           Name:admin<br>
           password:1234

    
    <H4>ADMIN.ejs</H4>
  <h5>Search button</h5>
           Hard coded url to github and get gits json. <br>
           When  a name is typed and the name exist, then there is an option to save it including his repo and followers <br>
    

   <h5> Save button</h5>
          When save button is clicked then the name is saved in an array in the level of js client side <br>
          but also passed to server side by using the main server. App.js. app.js calls to users.js and call to the save function<br>
          Save function deals with DB sqlite and stores it inn that DB<br>
    
    <h5>Delete</h5>
          When delete button is clicked on the client side, it deletes the name (a url to the names account in github)<br>
          From client side and also from server side by interacting  with the main server app.js. app.js calls to users.js and call to the delete function.
          Delete function deletes the name from DB sqlite

    






