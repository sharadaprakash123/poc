# poc
Define a custom runner for Espresso framework, which get tests from excel sheets or json and start tests

Creating a custom runner for the Espresso testing framework to run tests from Excel sheets or JSON files requires extending the built-in AndroidJUnitRunner class and implementing the necessary logic to read test data from the specified sources. Here's a high-level outline of how you could achieve this:

Create a Custom Runner Class:
Start by creating a new class that extends AndroidJUnitRunner. This class will serve as your custom test runner.

Reading Test Data from Excel:
To read test data from Excel sheets, you'll need a library to parse Excel files. Apache POI is a popular choice for this purpose.

Reading Test Data from JSON:
To read test data from JSON files, you can use the built-in JSON parsing libraries in Java.

Integrate Test Data into Custom Runner:
Finally, in your custom runner class, you can override the getTestCases() method to provide the test data to Espresso tests. Depending on whether you're using Excel or JSON, you can call the appropriate method from the respective data reader classes.


