
# MysqlQuest_simple
##useage
    db = MysqlQuest(host='localhost', user='root', password='root', port=3306)
    db.do_quest(colum_like=[], value=['40733'])

##Introduce
This can be solved. When you have a value, but do not know the specific information of the database, perform all database queries
Like this
![Snipaste_2022-02-18_01-02-25](https://user-images.githubusercontent.com/66716069/154540314-8b7758e8-b771-4081-a095-59d2479a9515.jpg)
When you know a spell ID is 30407, but you need to know the location in the database to modify it, and you just don't know this location, you can use it at this time

It is strongly recommended to enter only one value of column_like at a time, as it has not been determined whether multiple values are appropriate
##Theory
It will get all the information of the database at init time, and then make a lot of SELECT statements at the time of query, like this, 
![Snipaste_2022-02-18_01-03-34](https://user-images.githubusercontent.com/66716069/154540456-5bae6bae-de7f-4403-89a0-c8ad8010bdd5.jpg)

and then query

Then you can get an excel result like this!
![Snipaste_2022-02-18_00-54-41](https://user-images.githubusercontent.com/66716069/154540477-9b12c15d-9345-4001-b829-3694571ad221.jpg)

