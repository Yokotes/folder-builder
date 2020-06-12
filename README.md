# Overview
My first python script that can create any folders hierarchy.
Folder builder is a script that generates tree of folders.

# How to use
Folder builder is a very simple script.
At first you need to create a new instance of Folder class.
```python
f1 = fb.Folder(name='Test folder', path='./')
```
There are 2 parameters:
  * name - Folder's name
  * path - Path to folder

You can don't enter parameters, in that case name will be 'New Folder' and folder's path will be your current path
```python
f1 = fb.Folder()

print(f1.name)
# Output: 'New Folder'

print(f1.path)
# Output: '*Your current absolute path*'
```
To add new object in folder, use script below
```python
# Adding folder inside other folder
f2 = Folder(name='Sub Folder')
f1.add(f2)
```
To remove object from folder use:
```python
f1.remove(f2)
```
To create your folder on the driver with inner subfolders and text files use:
```python
# Build function will create on your driver folder and will fill it with subfolders
f1.build()
```
If you want to delete folder from the driver, you can use script below
```python
# This function will delete folder from your driver
f1.delete()
```