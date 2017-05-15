# scala_diary
Archiving my ascent up the stairway to Scala heaven.  

## Setup

https://medium.com/@faizanahemad/machine-learning-with-jupyter-using-scala-spark-and-python-the-setup-62d05b0c7f56
https://github.com/alexarchambault/jupyter-scala

1. Setup Scala

  A) Download
  ```bash
  wget https://downloads.lightbend.com/scala/2.12.2/scala-2.12.2.tgz
  ```
  B) Extract
  ```bash
  tar -xvzf scala-2.12.2.tgz
  ```
  C) Export PATH
  ```bash
  export PATH="~/projects/scala_diary/scala-2.12.2/bin:$PATH"
  ```
  
2. Setup Spark

  A) Download
  ```bash
  wget https://d3kbcqa49mib13.cloudfront.net/spark-2.1.1-bin-hadoop2.7.tgz
  ```
  B) Extract
  ```bash
  tar -xvzf spark-2.1.1-bin-hadoop2.7.tgz
  ```
  C) Export PATH
  ```
  export PATH="~/projects/scala_diary/spark-2.1.1-bin-hadoop2.7/bin:$PATH"
  ```
  
 3. Clone jupyter-scala
 ```bash
   git clone https://github.com/alexarchambault/jupyter-scala.git
   cd jupyter-scala
   ```
   
 4. Compile and publish sources
 ```bash
 sbt publishLocal
 ```
 
 5. Define Kernel
 ```bash
 ./jupyter-scala --id scala-develop --name "Scala (develop)" --force
 ```
