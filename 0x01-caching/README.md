0x01. Caching - Back-end

Background Context
In this project, you will explore and implement different caching algorithms. Caching is a technique used in computer science to store data temporarily in order to speed up future access. By storing copies of frequently accessed data in cache memory, the system can reduce the time and resources required to retrieve that data from slower storage locations such as disk or network.

Resources
To better understand caching and its various algorithms, it's recommended to read or watch resources on the following topics:

Cache replacement policies - FIFO (First In, First Out)
Cache replacement policies - LIFO (Last In, First Out)
Cache replacement policies - LRU (Least Recently Used)
Cache replacement policies - MRU (Most Recently Used)
Cache replacement policies - LFU (Least Frequently Used)

What a caching system is
The principles behind different caching algorithms
The purpose and limitations of a caching system

Requirements
Python Scripts
All files will be interpreted/compiled on Ubuntu 18.04 LTS using python3 (version 3.7)
All files should end with a new line
The first line of all files should be exactly #!/usr/bin/env python3
A README.md file, at the root of the project folder, is mandatory
Code should follow the pycodestyle style (version 2.5)
All files must be executable
The length of your files will be tested using wc
All modules should have documentation (python3 -c 'print(__import__("my_module").__doc__)')
All classes should have documentation (python3 -c 'print(__import__("my_module").MyClass.__doc__)')
All functions (inside and outside a class) should have documentation (python3 -c 'print(__import__("my_module").my_function.__doc__)' and python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)')
Documentation should be a full sentence explaining the purpose of the module, class, or method
More Info
Parent class BaseCaching

All classes must inherit from BaseCaching defined below:

python
Copy code
#!/usr/bin/python3
""" BaseCaching module
"""

class BaseCaching():
    """ BaseCaching defines:
      - Constants of the caching system
      - Where data are stored (in a dictionary)
    """
    MAX_ITEMS = 4

    def __init__(self):
        """ Initializes the caching system
        """
        self.cache_data = {}

    def print_cache(self):
        """ Prints the cache
        """
        print("Current cache:")
        for key in sorted(self.cache_data.keys()):
            print("{}: {}".format(key, self.cache_data.get(key)))

    def put(self, key, item):
        """ Adds an item to the cache
        """
        raise NotImplementedError("put must be implemented in your cache class")

    def get(self, key):
        """ Retrieves an item from the cache
        """
        raise NotImplementedError("get must be implemented in your cache class")
Tasks
The project consists of the following tasks:

Basic dictionary: Create a class BasicCache that implements a basic caching system using a dictionary.
FIFO caching: Implement a caching system using the FIFO (First In, First Out) algorithm in a class FIFOCache.
LIFO caching: Implement a caching system using the LIFO (Last In, First Out) algorithm in a class LIFOCache.
LRU caching: Implement a caching system using the LRU (Least Recently Used) algorithm in a class LRUCache.
MRU caching: Implement a caching system using the MRU (Most Recently Used) algorithm in a class MRUCache.
LFU caching: Implement a caching system using the LFU (Least Frequently Used) algorithm in a class LFUCache.

License
This project is licensed under the MIT License - see the LICENSE file for details.
