# Scala_Daily_Works

Introduction to Scala Version # 2.12.2

# Learning Scala: Fundamentals



val id=10
val applicationName="dqa"
val jobId=97889

println("id==> "+id+"\n applicationName=>  "+applicationName+" \n jobId=> """+jobId+""")

==============================================================
val my:String="""{"id":"ms"}"""
val ids:String= """ {"x":"ws"}"""

scala>  println("name=>"+"\""+name+"\"")
name=>"mmc"
https://stackoverflow.com/questions/3844595/how-can-i-make-java-print-quotes-like-hello

==============================================================

val donutJson3: String = s"""{"donut_name":"Glazed Donut","taste_level":"Very Tasty","price":2.50}"""

val donutJson3: String = {"donut_name":"Glazed Donut","taste_level":"Very Tasty","price":2.50}
println(s"donutJson3 = $donutJson3")

==============================================================

val donutJson4: String ="""{"donut_name":"Glazed Donut","taste_level":"Very Tasty","price":2.50}

""".stripMargin

==============================================================

val donutJson4: String =
    """
      {
      "donut_name":"Glazed Donut",
      "taste_level":"Very Tasty",
  
        "price":2.50
      }
      """
 .stripMargin

 
 void : nothing return
 
 Unit
 
 def main(Array[String]:Args):Unit={
 
 }
 
 spark-shell $1 $2 $3 $4
 
 
 $1 $2 $3 $4===>String
 
 val jobId=$1.toLong
 val pressionDouble=$2.toDouble 
 val checkYesOrNot=$3.toChar;
 
 
 for(numberOfDonuts <- 1 to 5){
  println(s"Number of donuts to buy = $numberOfDonuts")
}
==============================================================
for(int i=1;i<=5;i++){
  println(i)
}

==============================================================
for(id <- 1 to 5){
}
int i=1 : Step1
i<-5;Step 2
println(i): Display Step 3
i++: Step 4
==============================================================

i<=5  1,2,3,4,5  1 to 5

i<5 1,2,3,4 1 until 5

==============================================================
val donutIngredients = List("flour", "sugar", "egg yolks", "syrup", "flavouring")

for(ingredient <- donutIngredients if ingredient == "sugar"){
  println(s"Found sweetening ingredient = $ingredient")
}

println("\nStep 4: Filter values using if conditions in for loop and return the result back using the yield keyword")
val sweeteningIngredients = for {
  ingredient <- donutIngredients
  if (ingredient == "sugar" || ingredient == "syrup")
} yield ingredient
==============================================================
val mList=List(1,2,3,4,5,5)
scala> for(num<-mList if num>=1){
     | println(num)
     | }
1
2
3
4
5
5
==============================================================

Varibles

var id:Int=1 (only only )
var myArray:Array=new Array[Int](10);
myArray holding 10
Collection 
i)mmutable collection 
ii)Immutbale collection 

==============================================================


Data Strcures (Query Optmisit)

List: Single: Holding Duplicates : Our Order 
Seq: user given order
Set: Single: We can't hold or store duplicates: hashing 
Map : key and Value

Map<Key,Value>= new Map<Key,Value>


Stack
Vector
LinkedList
DoubleList
BFS
DFS:Deaf
Graph
 

   1
 2    3
4 5  6  7
  
  
# Learning Scla #Day 3 

  Tuple   
====================================== Learning Scala Fundementails ====================
val dbDetails=("com.db2.Driver","jdbc:db2:@host:","hedisdb","chhhhdfh");

scala> val dbDetails=("com.db2.Driver","jdbc:db2:@host:","hedisdb","chhhhdfh");
dbDetails: (String, String, String, String) = (com.db2.Driver,jdbc:db2:@host:,hedisdb,chhhhdfh)

scala> dbDetails._1
res6: String = com.db2.Driver

scala> dbDetails._2
res7: String = jdbc:db2:@host:

scala> dbDetails._3
res8: String = hedisdb

scala> dbDetails._4
res9: String = chhhhdfh

scala> val passwod=dbDetails._4
passwod: String = chhhhdfh

Arrays : 0
Tuple : 1

val x=Tuple1("akdkf","adkfadk")
val glazedDonut = Tuple3("Glazed Donut", "Very Tasty", 2.50)
val strawberryDonut = Tuple3("Strawberry Donut", "Very Tasty", 2.50)
val plainDonut = Tuple3("Plain Donut", "Tasty", 2)

val donutList = List(glazedDonut, strawberryDonut, plainDonut)

val priceOfPlainDonut = donutList.foreach { tuple => {
  tuple match {
    case ("Plain Donut", taste, price) => println(s"Donut type = Plain Donut, price = $price")
    case d if d._1 == "Glazed Donut" => println(s"Donut type = ${d._1}, price = ${d._3}")
    case _ => None
    }
  }
}
  
  
  val priceOfPlainDonut = donutList.foreach { tuple => {
  tuple match {
   case d =>println(d)
  }
  }
  
  val priceOfDonut: Any = 2.50
val priceType = priceOfDonut match {
  case price: Int => "Int"
  case price: Double => "Double"
  case price: Float => "Float"
  case price: String => "String"
  case price: Boolean => "Boolean"
  case price: Char => "Char"
  case price: Long => "Long"
}
  
  
  
  val x=(1,"hello")

  x.productIterator
  .foreach {
       println   
   }  
  
  x.productIterator
  .foreach {
    case s: String => println("string: " + s)
    case i: Int => println("int: " + i)
  }
  
  Tuple Methods 
  scala> myTuple.
_1   canEqual   hashCode       productElement(Element Wise Like Position checking)    toString
_2   copy       invert         productIterator   zipped
_3   equals     productArity   productPrefix(Perfix of what is tuple )

scala> myTuple.


                Any 
	AnyValue           AnyRef	
	 Int,Float,Double    List,Set,Seq,
	 
	 val x:Any=10
	 val y:AnyValue=20.5
	 val p:AnyRef=List("anji","adfadf")
	 
		
       Option
Some          None 

		
# ################################################################################################

# Scala Classes & Objects (OOPS) 
 1::class
 2::Object

