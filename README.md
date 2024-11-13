# MongoDB-lesson-1
Install MongoDB Compass and MongoShell
Click on Cluster and click M0(Free) yhis is for the configurations
username:clentanchauke9089
Password:iDT2YcaUPj03pLa8
Once Cluster is created then Connect Atlas with MongoDB Compass( 
1.firstly:choose the version of compass.
2.Copy the connection string,then open MongoDB Compass)
.In the Cluster Create a New Project and Name them
Open Terminal and Paste Url:Address
Paster:password
get inside the directory using:use (Folder_Name)
then use :db.(folder_name).find() to print what is inside the folder


Mongo DB
using a terminal .

initialize Mongo Db by using (Mongosh on terminal)


For Lesson 3 :
Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.

Install the latest PowerShell for new features and improvements! https://aka.ms/PSWindows

PS C:\Users\clent> monagosh
monagosh : The term 'monagosh' is not recognized as the name of a cmdlet, function, script file, or operable program.
Check the spelling of the name, or if a path was included, verify that the path is correct and try again.
At line:1 char:1
+ monagosh
+ ~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (monagosh:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS C:\Users\clent> mongosh
Current Mongosh Log ID: 6734a14e34767d6aaf0d818f
Connecting to:          mongodb://127.0.0.1:27017/?directConnection=true&serverSelectionTimeoutMS=2000&appName=mongosh+2.3.3
Using MongoDB:          8.0.3
Using Mongosh:          2.3.3

For mongosh info see: https://www.mongodb.com/docs/mongodb-shell/

------
   The server generated these startup warnings when booting
   2024-11-13T14:42:13.736+02:00: Access control is not enabled for the database. Read and write access to data and configuration is unrestricted
------

test> show collection
MongoshInvalidInputError: [COMMON-10001] 'collection' is not a valid argument for "show".
test> show collections

test> show dbs
Clentan   8.00 KiB
admin    40.00 KiB
config   72.00 KiB
local    72.00 KiB
test> show Codetribe
MongoshInvalidInputError: [COMMON-10001] 'Codetribe' is not a valid argument for "show".
test> use Codetribe
switched to db Codetribe
Codetribe> db.Facililitator.insertOne({Name:"Refilwe",Location:"Polokwane",Course:"Mongo"})
{
  acknowledged: true,
  insertedId: ObjectId('6734a24d34767d6aaf0d8190')
}
Codetribe> show collections
Facililitator
Codetribe> db.Facilitator.find()

Codetribe> use Facilitator
switched to db Facilitator
Facilitator> db.Facilitator.find()

Facilitator> use Codetribe
switched to db Codetribe
Codetribe> db.Facilitator.insertOne({name:"refilwe",location:"polokwane",course:"react"})
{
  acknowledged: true,
  insertedId: ObjectId('6734a39834767d6aaf0d8191')
}
Codetribe> db.Facilitator.find()
[
  {
    _id: ObjectId('6734a39834767d6aaf0d8191'),
    name: 'refilwe',
    location: 'polokwane',
    course: 'react'
  }
]
Codetribe> db.Traniee.insertOne({name:"clentan",location:"polokwane",facilitator:"refilwe"})
{
  acknowledged: true,
  insertedId: ObjectId('6734a43d34767d6aaf0d8192')
}
Codetribe> db.Traniee.find()
[
  {
    _id: ObjectId('6734a43d34767d6aaf0d8192'),
    name: 'clentan',
    location: 'polokwane',
    facilitator: 'refilwe'
  }
]
Codetribe> show collections
Facililitator
Facilitator
Traniee
Codetribe> db.projects.insertOne({name:"mongo",course:"react",lesson:"Mongo"})
{
  acknowledged: true,
  insertedId: ObjectId('6734a4d834767d6aaf0d8193')
}
Codetribe> show collections
Facililitator
Facilitator
projects
Traniee
Codetribe> clo
ReferenceError: clo is not defined
Codetribe> quit
PS C:\Users\clent> mongosh
Current Mongosh Log ID: 6734a65f538bf9dc670d818f
Connecting to:          mongodb://127.0.0.1:27017/?directConnection=true&serverSelectionTimeoutMS=2000&appName=mongosh+2.3.3
Using MongoDB:          8.0.3
Using Mongosh:          2.3.3

For mongosh info see: https://www.mongodb.com/docs/mongodb-shell/

------
   The server generated these startup warnings when booting
   2024-11-13T14:42:13.736+02:00: Access control is not enabled for the database. Read and write access to data and configuration is unrestricted
------

test> show collections

test> show dbs
Clentan      8.00 KiB
Codetribe  160.00 KiB
admin       40.00 KiB
config      96.00 KiB
local       72.00 KiB
test> use Library
switched to db Library
Library> db.BookCollection.insertMany([ { _id: 1, title: "1984", author_id: 1, genres: ["Dystopian", "Political Fiction"], published_year: 1949, available: true }, { _id: 2, title: "To Kill a Mockingbird", author_id: 2, genres: ["Southern Gothic", "Bildungsroman"], published_year: 1960, available: true }, { _id: 3, title: "The Great Gatsby", author_id: 3, genres: ["Tragedy"], published_year: 1925, available: true }, { _id: 4, title: "Brave New World", author_id: 4, genres: ["Dystopian", "Science Fiction"], published_year: 1932, available: true }, { _id: 5, title: "The Catcher in the Rye", author_id: 5, genres: ["Realist Novel", "Bildungsroman"], published_year: 1951, available: true }, { _id: 6, title: "Moby-Dick", author_id: 6, genres: ["Adventure Fiction"], published_year: 1851, available: true }, { _id: 7, title: "Pride and Prejudice", author_id: 7, genres: ["Romantic Novel"], published_year: 1813, available: true }, { _id: 8, title: "War and Peace", author_id: 8, genres: ["Historical Novel"], published_year: 1869, available: true }, { _id: 9, title: "Crime and Punishment", author_id: 9, genres: ["Philosophical Novel"], published_year: 1866, available: true }, { _id: 10, title: "The Hobbit", author_id: 10, genres: ["Fantasy"], published_year: 1937, available: true } ])
{
  acknowledged: true,
  insertedIds: {
    '0': 1,
    '1': 2,
    '2': 3,
    '3': 4,
    '4': 5,
    '5': 6,
    '6': 7,
    '7': 8,
    '8': 9,
    '9': 10
  }
}
Library> db.authors.insertMany([ { _id: 1, name: "George Orwell", nationality: "British", birth_year: 1903, death_year: 1950 }, { _id: 2, name: "Harper Lee", nationality: "American", birth_year: 1926, death_year: 2016 }, { _id: 3, name: "F. Scott Fitzgerald", nationality: "American", birth_year: 1896, death_year: 1940 }, { _id: 4, name: "Aldous Huxley", nationality: "British", birth_year: 1894, death_year: 1963 }, { _id: 5, name: "J.D. Salinger", nationality: "American", birth_year: 1919, death_year: 2010 }, { _id: 6, name: "Herman Melville", nationality: "American", birth_year: 1819, death_year: 1891 }, { _id: 7, name: "Jane Austen", nationality: "British", birth_year: 1775, death_year: 1817 }, { _id: 8, name: "Leo Tolstoy", nationality: "Russian", birth_year: 1828, death_year: 1910 }, { _id: 9, name: "Fyodor Dostoevsky", nationality: "Russian", birth_year: 1821, death_year: 1881 }, { _id: 10, name: "J.R.R. Tolkien", nationality: "British", birth_year: 1892, death_year: 1973 } ])
{
  acknowledged: true,
  insertedIds: {
    '0': 1,
    '1': 2,
    '2': 3,
    '3': 4,
    '4': 5,
    '5': 6,
    '6': 7,
    '7': 8,
    '8': 9,
    '9': 10
  }
}
Library> db.inssertMany([ { _id: 1, name: "Alice Johnson", email: "alice@example.com", borrowed_books: [] }, { _id: 2, name: "Bob Smith", email: "bob@example.com", borrowed_books: [1, 2] }, { _id: 3, name: "Carol White", email: "carol@example.com", borrowed_books: [] }, { _id: 4, name: "David Brown", email: "david@example.com", borrowed_books: [3] }, { _id: 5, name: "Eve Davis", email: "eve@example.com", borrowed_books: [] }, { _id: 6, name: "Frank Moore", email: "frank@example.com", borrowed_books: [4, 5] }, { _id: 7, name: "Grace Miller", email: "grace@example.com", borrowed_books: [] }, { _id: 8, name: "Hank Wilson", email: "hank@example.com", borrowed_books: [6] }, { _id: 9, name: "Ivy Taylor", email: "ivy@example.com", borrowed_books: [] }, { _id: 10, name: "Jack Anderson", email: "jack@example.com", borrowed_books: [7, 8] } ])
TypeError: db.inssertMany is not a function
Library> db.patrons.insrtMany([ { _id: 1, name: "Alice Johnson", email: "alice@example.com", borrowed_books: [] }, { _id: 2, name: "Bob Smith", email: "bob@example.com", borrowed_books: [1, 2] }, { _id: 3, name: "Carol White", email: "carol@example.com", borrowed_books: [] }, { _id: 4, name: "David Brown", email: "david@example.com", borrowed_books: [3] }, { _id: 5, name: "Eve Davis", email: "eve@example.com", borrowed_books: [] }, { _id: 6, name: "Frank Moore", email: "frank@example.com", borrowed_books: [4, 5] }, { _id: 7, name: "Grace Miller", email: "grace@example.com", borrowed_books: [] }, { _id: 8, name: "Hank Wilson", email: "hank@example.com", borrowed_books: [6] }, { _id: 9, name: "Ivy Taylor", email: "ivy@example.com", borrowed_books: [] }, { _id: 10, name: "Jack Anderson", email: "jack@example.com", borrowed_books: [7, 8] } ])
TypeError: db.patrons.insrtMany is not a function
Library> db.patrons.insertMany([ { _id: 1, name: "Alice Johnson", email: "alice@example.com", borrowed_books: [] }, { _id: 2, name: "Bob Smith", email: "bob@example.com", borrowed_books: [1, 2] }, { _id: 3, name: "Carol White", email: "carol@example.com", borrowed_books: [] }, { _id: 4, name: "David Brown", email: "david@example.com", borrowed_books: [3] }, { _id: 5, name: "Eve Davis", email: "eve@example.com", borrowed_books: [] }, { _id: 6, name: "Frank Moore", email: "frank@example.com", borrowed_books: [4, 5] }, { _id: 7, name: "Grace Miller", email: "grace@example.com", borrowed_books: [] }, { _id: 8, name: "Hank Wilson", email: "hank@example.com", borrowed_books: [6] }, { _id: 9, name: "Ivy Taylor", email: "ivy@example.com", borrowed_books: [] }, { _id: 10, name: "Jack Anderson", email: "jack@example.com", borrowed_books: [7, 8] } ])
{
  acknowledged: true,
  insertedIds: {
    '0': 1,
    '1': 2,
    '2': 3,
    '3': 4,
    '4': 5,
    '5': 6,
    '6': 7,
    '7': 8,
    '8': 9,
    '9': 10
  }
}
Library> db.BookCollection.find()
[
  {
    _id: 1,
    title: '1984',
    author_id: 1,
    genres: [ 'Dystopian', 'Political Fiction' ],
    published_year: 1949,
    available: true
  },
  {
    _id: 2,
    title: 'To Kill a Mockingbird',
    author_id: 2,
    genres: [ 'Southern Gothic', 'Bildungsroman' ],
    published_year: 1960,
    available: true
  },
  {
    _id: 3,
    title: 'The Great Gatsby',
    author_id: 3,
    genres: [ 'Tragedy' ],
    published_year: 1925,
    available: true
  },
  {
    _id: 4,
    title: 'Brave New World',
    author_id: 4,
    genres: [ 'Dystopian', 'Science Fiction' ],
    published_year: 1932,
    available: true
  },
  {
    _id: 5,
    title: 'The Catcher in the Rye',
    author_id: 5,
    genres: [ 'Realist Novel', 'Bildungsroman' ],
    published_year: 1951,
    available: true
  },
  {
    _id: 6,
    title: 'Moby-Dick',
    author_id: 6,
    genres: [ 'Adventure Fiction' ],
    published_year: 1851,
    available: true
  },
  {
    _id: 7,
    title: 'Pride and Prejudice',
    author_id: 7,
    genres: [ 'Romantic Novel' ],
    published_year: 1813,
    available: true
  },
  {
    _id: 8,
    title: 'War and Peace',
    author_id: 8,
    genres: [ 'Historical Novel' ],
    published_year: 1869,
    available: true
  },
  {
    _id: 9,
    title: 'Crime and Punishment',
    author_id: 9,
    genres: [ 'Philosophical Novel' ],
    published_year: 1866,
    available: true
  },
  {
    _id: 10,
    title: 'The Hobbit',
    author_id: 10,
    genres: [ 'Fantasy' ],
    published_year: 1937,
    available: true
  }
]
Library> db.BookCollection.find(title: "To Kill a Mockingbird")
Uncaught:
SyntaxError: Unexpected token, expected "," (1:28)

> 1 | db.BookCollection.find(title: "To Kill a Mockingbird")
    |                             ^
  2 |

Library> db.BookCollection.find(title:"To Kill a Mockingbird")
Uncaught:
SyntaxError: Unexpected token, expected "," (1:28)

> 1 | db.BookCollection.find(title:"To Kill a Mockingbird")
    |                             ^
  2 |

Library> db.BookCollection.find({title: "To Kill a Mockingbird"})
[
  {
    _id: 2,
    title: 'To Kill a Mockingbird',
    author_id: 2,
    genres: [ 'Southern Gothic', 'Bildungsroman' ],
    published_year: 1960,
    available: true
  }
]
Library> db.authors.find({author_id:5})

Library> db.authors.find({id:5})

Library> db.authors.find({author_id:5)}
Uncaught:
SyntaxError: Unexpected token, expected "," (1:28)

> 1 | db.authors.find({author_id:5)}
    |                             ^
  2 |

Library>  db.authors.find({author_id:5})

Library>  db.authors.find({"author_id":5})

Library> db.books.find({ author_id: 5 })

Library> db.BookCollection.find({ author_id: 5 })
[
  {
    _id: 5,
    title: 'The Catcher in the Rye',
    author_id: 5,
    genres: [ 'Realist Novel', 'Bildungsroman' ],
    published_year: 1951,
    available: true
  }
]
Library> db.BookCollection.find()
[
  {
    _id: 1,
    title: '1984',
    author_id: 1,
    genres: [ 'Dystopian', 'Political Fiction' ],
    published_year: 1949,
    available: true
  },
  {
    _id: 2,
    title: 'To Kill a Mockingbird',
    author_id: 2,
    genres: [ 'Southern Gothic', 'Bildungsroman' ],
    published_year: 1960,
    available: true
  },
  {
    _id: 3,
    title: 'The Great Gatsby',
    author_id: 3,
    genres: [ 'Tragedy' ],
    published_year: 1925,
    available: true
  },
  {
    _id: 4,
    title: 'Brave New World',
    author_id: 4,
    genres: [ 'Dystopian', 'Science Fiction' ],
    published_year: 1932,
    available: true
  },
  {
    _id: 5,
    title: 'The Catcher in the Rye',
    author_id: 5,
    genres: [ 'Realist Novel', 'Bildungsroman' ],
    published_year: 1951,
    available: true
  },
  {
    _id: 6,
    title: 'Moby-Dick',
    author_id: 6,
    genres: [ 'Adventure Fiction' ],
    published_year: 1851,
    available: true
  },
  {
    _id: 7,
    title: 'Pride and Prejudice',
    author_id: 7,
    genres: [ 'Romantic Novel' ],
    published_year: 1813,
    available: true
  },
  {
    _id: 8,
    title: 'War and Peace',
    author_id: 8,
    genres: [ 'Historical Novel' ],
    published_year: 1869,
    available: true
  },
  {
    _id: 9,
    title: 'Crime and Punishment',
    author_id: 9,
    genres: [ 'Philosophical Novel' ],
    published_year: 1866,
    available: true
  },
  {
    _id: 10,
    title: 'The Hobbit',
    author_id: 10,
    genres: [ 'Fantasy' ],
    published_year: 1937,
    available: true
  }
]
Library>


