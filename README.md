# Science_Archives
## Introduction
Science Archives is an SQL database that is designed to hold various science archives within the database. This includes books, conference papers, thesis, and journal articles. The database also hold additional information including the names of authors, information about the users, reviews, editors, subjects, items and library.

## Tools used
phpMyAdmin was used to create the SQL database to store information. 

## Science Archives Relational Schema 
![image](https://github.com/user-attachments/assets/25b3cd2b-8a1d-4257-beaf-5fd466eceb16)
The image above shows the relation schema of Science Archives. It represents the relationship between its main entities, which includes the user, items, journal articles, books, conference paper, thesis, author, subject, and editor. Each entity contains attributes which further reveal information and its complexity. These entities are connected by various types of relationships such as one-to-one, one-to-many,many-to-one and many-to-many. 

# Entities
## Items stored within the database
![image](https://github.com/user-attachments/assets/75971068-92c0-4e25-afd3-31d466badf91)
The item entity contains attribute item id, avg score, publisher name, publication year, publication type, hyperlink and abstract. The item id acts as a primary key. The column avg score shows the average score which rates the paper based percentage. The publisher name shows the name of the individual who published the paper and the column publication year shows the year in which the item has been published. The entity also contains the column called publication_type which reveals the type of publication of the item. This can range between journal articles, books, thesis or conference papers. Due to the various types of publication, four entities have been created which connect to the item entity. These entities are thesis, book, conference paper and journal article. When an item is added onto the database, information is also inputted into one of these tables which establishes their type of publication. Each publication type has different attributes, and various entities were created to suit each one. For example, a conference paper is related to the name of the conference but a book is not involved in a conference but instead contains a book publication place. An item can be stored within the entity item and the entity journal article if the item itself is an article from a journal, both containing the same item id and are therefore connected. The same can be done if the item were a different publication type, such as if the item were a book or a thesis. This fulfils the requirement of the database being capable of containing items of different types of publication based on the client specification.

## Books stored within the database
![image](https://github.com/user-attachments/assets/94b88cdf-7a39-48e9-b6f2-4157dc4188ef)

## Conference papers stored within the database 
![image](https://github.com/user-attachments/assets/2fc9ecf8-559b-4eec-92d4-be69f9628584)

## Journal Articles stored within the database
![image](https://github.com/user-attachments/assets/b8424054-40c8-4e5d-a0b5-78690ca51901)

## Thesis stored within the database
![image](https://github.com/user-attachments/assets/c2b086cb-bc88-4486-94cb-8b497e99f030)


## Names of authors stored within the database
![image](https://github.com/user-attachments/assets/4bb8d45c-1352-46d9-95c2-5fd4192969b4)

## Names of editors stored within the database
![image](https://github.com/user-attachments/assets/10e8338d-ec1f-4f35-ab8c-f0436d63563c)

## list of users stored within database
![image](https://github.com/user-attachments/assets/208c4c45-5091-44fe-aa70-88f2d3e85c5e)
The user entity contains user's id, full name (first name, middle name and last name), email, phone, contact preference, username, password, capacity and author name. The user id acts as a primary key and the user's full name establishes the user's identity. The email and phone attributes contain information on how the user can be contacted, as well as their contact preference. A username and password is also contained within the entity and their capacity, which identifies if the user is a reader, author or both. The user entity is also connected to the author entity, establishing a one-to-one relationship if the user is one of the authors that has written an item (conference paper, thesis, book, article). These attributes satisfy the client’s specification.

## Reviews stored within database
![image](https://github.com/user-attachments/assets/5506b769-d93f-4687-841c-ecc7dea97e33)

