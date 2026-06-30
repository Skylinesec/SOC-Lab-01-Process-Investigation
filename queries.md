# SPL Queries Used

## View all Process Creation Events

```spl
index=main EventCode=1
```

## PowerShell Events

```spl
index=main EventCode=1 Image="*powershell.exe"
```

## Timeline

```spl
index=main EventCode=1
| table _time Image ParentImage CommandLine User
| sort _time
```
