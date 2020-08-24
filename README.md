### Introduction to MongoDB

- Move to the mongodb folder and then start the MongoDB server by typing the following at the prompt:

  - mongod --dbpath=data --bind_ip 127.0.0.1

- Open another command window and then type the following at the command prompt to start the mongo REPL shell:

  - mongo

- he Mongo REPL shell will start running and give you a prompt to issue commands to the MongoDB server. At the Mongo REPL prompt, type the following commands one by one and see the resulting behavior:

  - db
  - use conFusion
  - db
  - db.help()

- You will now create a collection named dishes, and insert a new dish document in the collection:

  - db.dishes.insert({ name: "Uthappizza", description: "Test" });

- Then to print out the dishes in the collection, type:

      -  db.dishes.find().pretty();

#### Note the "\_id" assigned to the dish.

- Next, we will learn the information encoded into the ObjectId by typing the following at the prompt:

  - var id = new ObjectId();
  - id.getTimestamp();

- Type "exit" at the REPL prompt to exit the Mongo REPL.
