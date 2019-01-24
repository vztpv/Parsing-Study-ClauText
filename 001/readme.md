1. C-String

    ```c
    char str[] = "hello world!";
    char str2[5] = "hell"; // '\0' added..
    ```

// todo..
strcpy, strlen, and etc <- using '\0' (delimiter)
strcmp <- cost of comparision for two string is not cheap.? - so we should reduce comparisions for two string.


```c
    void func(const char* str1, const char* str2)
    {
        if (strcmp(str1, str2) < 0) {
            // do something..
        }
        else if (strcmp(str1, str2) > 0) {
            // do something..
        }
    }
```
    
    =>
    
```c
    void func(const char* str1, const char* str2) 
    {
        int chk = strcmp(str1, str2);
        
        if (chk < 0) {
            // do something...
        }
        else if (chk > 0) {
            // do something..
        }
    }
```

check c++ version?

```cpp
    void func(const std::string& str1, const std::string& str2)
    {
        if (str1 < str2) 
        {
            // do something..
        }
        else if (str1 > str2)
        {
            // do something..
        }
    }
```

=> 

??
