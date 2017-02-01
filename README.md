# Configure JUnit in IntelliJ IDEA

## Prerequisite

* [IntelliJ IDEA](https://www.jetbrains.com/idea/)

## Initialize JUnit in IntelliJ IDEA

1. Create a new project called ```Example```.
2. Select File > Project Structure, set Project SDK to ```1.8``` and Project language level to ```8```.
3. Create a new module under project called ```Example``` (File > New > Module).
4. Create a directory named ```tests``` under ```Example``` module (Right click at ```Example``` module > New > Directory).
5. Mark ```tests``` directory as ```Tests Sources Root``` (Right click at ```tests``` > Mark Directory as > Tests Sources Root).
6. Create a Java class under ```tests``` named ```TestExample```.
7. Create a test case in ```TestExample``` class starting with ```test```.
8. Add ```@Test``` annotation before test case implementation.
9. ```@Test``` will become red. Go there and light bulb icon will appear for suggestion, select ```Add 'JUnit4' to class path```.
10. Select ```Use 'JUnit4' from IntelliJ IDEA distribution```. ```@Test``` now should be grey.
11. Now you are good to go. Enjoy unit testing.

## First try with a RED test case

1. Create a test case named ```testShouldBeGreen```.
2. Add the following code and run.

   ```
    assertEqual(true, false);
   ```

3. Test result should fail.
4. Fix it by changing the code to the following and re-run the test.

   ```
    assertEqual(true, true);
   ```

5. Test result should pass.