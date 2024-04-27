# Basic Powershell Commands

What is cmdlet?
Now that we have PowerShell up and running, we can start looking at how things are going in the PowerShell world.

As we said in the introduction, PowerShell is a powerful command line shell and scripting language system that allows users to manage computers and networks. PowerShell comes with a large set of commands or "cmdlets" to perform a variety of system administration tasks.

Cmdlets are usually named in the "-VerbNoun" format and are used to perform a specific action. For example, the "Get-Process" cmdlet returns a list of all running processes, "Stop-Process" stops a specific process. For better understanding, let's give examples of basic cmdlets that come by default with a standard PowerShell installation:

You can see in the list that the PSCustomObject data type, which is specially designed for PowerShell, while other data types are data types we are familiar with from programming and scripting languages and databases. This data type allows users to create customized objects. A PSCustomObject is an object that has one or more properties of different types.

Used with @{} (Hashtable) to create a PSCustomObject.

```powershell                   
$myObject = [PSCustomObject]@{
FirstName = 'Lets'
LastName = 'Defend'
Rank = 1
}
```

```powershell   
$myObject.FirstName
$myObject.LastName
$myObject.Rank
```

In some cases, it may be necessary to create a variable with a specific type. In this case, the type can be specified when creating the variable:

```powershell                    
[string]$myString = "Hello World"
[int]$myNumber = 42
[array]$myArray = 1,2,3,4,5
```
In PowerShell, variables can store many different types of data, such as text, number, Boolean, array, hashtable, and even custom objects. These are a result of PowerShell being built on top of the .NET Framework, which means PowerShell can support almost any data type supported by .NET.