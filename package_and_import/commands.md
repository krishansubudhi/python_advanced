Package without __init__ or __main__
    import package1
    print(package1.__path__)

# Path
Directory of the file which the python applicaiton calls is only added to the path

    (tutorial) C:\Users\krkusuk.REDMOND\OneDrive\study\python\pluralsight>python package1/__init__.py
    ['C:\\Users\\krkusuk.REDMOND\\OneDrive\\study\\python\\pluralsight\\package1', 

    (tutorial) C:\Users\krkusuk.REDMOND\OneDrive\study\python\pluralsight>python package1
    ['package1', 

The following only adds the directory of test.py to path. Hence import in __init__.py fails.

    (tutorial) C:\Users\krkusuk.REDMOND\OneDrive\study\python\pluralsight>python test.py
    ['C:\\Users\\krkusuk.REDMOND\\OneDrive\\study\\python\\pluralsight', 

If __main__.py is present in the directory, then no need to specify file name
    
    (tutorial) C:\Users\krkusuk.REDMOND\OneDrive\study\python\pluralsight>python package1
    ['package1', 

Here the __main__.py file directory is added to the path
