# Sequences
- Simplest way to create a sequence in R is >> 1:20  O/P is 1 2 3 4 5 6 .....19 20 & we can do it reverse too. 15:1>> 15 14 13 12........2 1
- For pi :10, its o/p 3.14 4.14 5.14......9.141593 These all are vectors
- ?`:` >> pull out documentation
- seq(1,20) does same thing as 1:20  
- To bring a gap is sequence we use seq(0,10, by = 0.5) does same as seq(0,10,0.5)
- To get many no. in a sequence like 100 no, between 7 and 10, seq(7,10,length = 100)
- Replication is done via >> rep(0, times = 40); we can also do this by using >> rep(c(0,1,2), each = 10)


# Vectors
- 2 different flavors : Atomic vectors(contains 1 data type) and Lists(multiple data types)
- Logical vectors containvalues like True or False and NA for null values.
- We can add conditions too to the vectors and use Logics like < , > , <=, >= , ==, != for inequality
- Logical OR | does UNiON tasks and Logical AND & does all intersection tasks.
- ((111 >= 111) | !(TRUE)) & ((4 +1) == 5)  >> This is TRue as o/P is 1,1 >> TRUE
- Chracter Vectors are availablle in double quotes and are chracter strings acc to R
- Sep() argument tells us , we want to seperate joined elements with single spaces.     n bvghbnm
