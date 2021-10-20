# linux_cli_tips

Replacing text in filename
```
# Can add an arbitrary number of extension types with more -o -names
find path/to/folder -type f -a \( -name "*.ext1" -o -name "ext2" \) -a -exec sed -i -e "s///g" {} +

# C++ example
find path/to/top/dir -type f -a \( -name "*.cc" -o -name ".h" \) -a -exec sed -i -e "s///g" {} + 
```

Remove a file suffix
```
find /some/dir/ -type f -name "*.SUFFIX" -delete 
```


