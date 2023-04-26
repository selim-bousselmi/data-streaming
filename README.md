# data-streaming
The following code utilizes the Apache Flink streaming framework to create an HTTP streaming application. It retrieves stock data from the RapidAPI service provider for the companies Google (GOOGL), Microsoft (MSFT) and Amazon (AMZN) and displays it on the console.
# Visualization
Interpreting raw stock data can be challenging, hence we employed the Matplotlib library to transform the data into a visual representation. By plotting the data in the form of graphs, we were able to gain a better understanding of the trends and patterns present in the data.
![alt text](https://github.com/selim-bousselmi/data-streaming/blob/main/Screenshot%202023-04-26%20140442.png?raw=true)

# Description
This application uses the Apache Flink streaming framework to collect data (stock prices over time) from the endpoint of the API (realstonks), and emits it as a string to the Flink data stream. The run method continues to execute until the cancel method is invoked, and it sleeps for a specified time interval between requests. The main method configures the Flink execution environment, adds the HTTP data source, and outputs the data to the console using the print method.

# Instructions
Running the code is very simple. You clone the project with git to download it locally, and then run data-streaming/src/main/scala/api-requests.scala file.
You need to have Java 8, Apache Flink and Scala.
