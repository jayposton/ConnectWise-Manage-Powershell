# Update-CWMCompanyTypeAssociation
## SYNOPSIS
This will update a company type association.
## SYNTAX
```powershell
Update-CWMCompanyTypeAssociation [-CompanyID] <Int32> [-TypeAssociationID] <Int32> [-Operation] <Object> [-Path] <String> [-Value] <String> [<CommonParameters>]
```
## PARAMETERS
### -CompanyID &lt;Int32&gt;
The ID of the company that you are updating. Get-CWMCompanies
```
Required                    true
Position                    1
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -TypeAssociationID &lt;Int32&gt;
The TypeAssociationID of the company that you are updating. Get-CWMCompanyTypeAssociation
```
Required                    true
Position                    2
Default value                0
Accept pipeline input       false
Accept wildcard characters  false
```
### -Operation &lt;Object&gt;
What you are doing with the value. 

replace
```
Required                    true
Position                    3
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -Path &lt;String&gt;
The value that you want to perform the operation on.
```
Required                    true
Position                    4
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
### -Value &lt;String&gt;
The value of that operation.
```
Required                    true
Position                    5
Default value
Accept pipeline input       false
Accept wildcard characters  false
```
## EXAMPLES
### EXAMPLE 1
```powershell
PS C:\>$UpdateParam = @{

CompanyID = $Company.id
    TypeAssociationID = $TypeAssoc.id
    Operation = 'replace'
    Path = 'name'
    Value = $NewName
}
Update-CWMCompanyTypeAssociation @UpdateParam
```

## NOTES
Author: Chris Taylor

Date: 10/10/2018 
## LINKS
http://labtechconsulting.com

https://developer.connectwise.com/Products/Manage/REST?a=Company&e=CompanyCompanyTypeAssociations&o=UPDATE
