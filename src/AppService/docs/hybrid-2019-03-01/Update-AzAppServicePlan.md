---
external help file:
Module Name: Az.WebSite
online version: https://docs.microsoft.com/en-us/powershell/module/az.website/update-azappserviceplan
schema: 2.0.0
---

# Update-AzAppServicePlan

## SYNOPSIS
Creates or updates an App Service Plan.

## SYNTAX

### Update (Default)
```
Update-AzAppServicePlan -Name <String> -ResourceGroupName <String> -SubscriptionId <String>
 [-AppServicePlan <IAppServicePlanPatchResource>] [-DefaultProfile <PSObject>] [-Confirm] [-WhatIf]
 [<CommonParameters>]
```

### UpdateExpanded
```
Update-AzAppServicePlan -Name <String> -ResourceGroupName <String> -SubscriptionId <String>
 [-FreeOfferExpirationTime <DateTime>] [-HostingEnvironmentProfileId <String>] [-HyperV] [-IsSpot] [-IsXenon]
 [-Kind <String>] [-MaximumElasticWorkerCount <Int32>] [-PerSiteScaling] [-Reserved]
 [-SpotExpirationTime <DateTime>] [-TargetWorkerCount <Int32>] [-TargetWorkerSizeId <Int32>]
 [-WorkerTierName <String>] [-DefaultProfile <PSObject>] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### UpdateViaIdentityExpanded
```
Update-AzAppServicePlan -InputObject <IWebSiteIdentity> [-FreeOfferExpirationTime <DateTime>]
 [-HostingEnvironmentProfileId <String>] [-HyperV] [-IsSpot] [-IsXenon] [-Kind <String>]
 [-MaximumElasticWorkerCount <Int32>] [-PerSiteScaling] [-Reserved] [-SpotExpirationTime <DateTime>]
 [-TargetWorkerCount <Int32>] [-TargetWorkerSizeId <Int32>] [-WorkerTierName <String>]
 [-DefaultProfile <PSObject>] [-Confirm] [-WhatIf] [<CommonParameters>]
```

### UpdateViaIdentity
```
Update-AzAppServicePlan -InputObject <IWebSiteIdentity> [-AppServicePlan <IAppServicePlanPatchResource>]
 [-DefaultProfile <PSObject>] [-Confirm] [-WhatIf] [<CommonParameters>]
```

## DESCRIPTION
Creates or updates an App Service Plan.

## EXAMPLES

### Example 1: {{ Add title here }}
```powershell
PS C:\> {{ Add code here }}

{{ Add output here }}
```

{{ Add description here }}

### Example 2: {{ Add title here }}
```powershell
PS C:\> {{ Add code here }}

{{ Add output here }}
```

{{ Add description here }}

## PARAMETERS

### -AppServicePlan
ARM resource for a app service plan.
To construct, see NOTES section for APPSERVICEPLAN properties and create a hash table.

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.WebSite.Models.Api20180201.IAppServicePlanPatchResource
Parameter Sets: Update, UpdateViaIdentity
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
Dynamic: False
```

### -DefaultProfile
The credentials, account, tenant, and subscription used for communication with Azure.

```yaml
Type: System.Management.Automation.PSObject
Parameter Sets: (All)
Aliases: AzureRMContext, AzureCredential

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -FreeOfferExpirationTime
The time when the server farm free offer expires.

```yaml
Type: System.DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -HostingEnvironmentProfileId
Resource ID of the App Service Environment.

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -HyperV
If Hyper-V container app service plan <code>true</code>, <code>false</code> otherwise.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -InputObject
Identity Parameter

```yaml
Type: Microsoft.Azure.PowerShell.Cmdlets.WebSite.Models.IWebSiteIdentity
Parameter Sets: UpdateViaIdentityExpanded, UpdateViaIdentity
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
Dynamic: False
```

### -IsSpot
If <code>true</code>, this App Service Plan owns spot instances.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -IsXenon
Obsolete: If Hyper-V container app service plan <code>true</code>, <code>false</code> otherwise.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -Kind
Kind of resource.

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -MaximumElasticWorkerCount
Maximum number of total workers allowed for this ElasticScaleEnabled App Service Plan

```yaml
Type: System.Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -Name
Name of the App Service plan.

```yaml
Type: System.String
Parameter Sets: Update, UpdateExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -PerSiteScaling
If <code>true</code>, apps assigned to this App Service plan can be scaled independently.If <code>false</code>, apps assigned to this App Service plan will scale to all instances of the plan.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -Reserved
If Linux app service plan <code>true</code>, <code>false</code> otherwise.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -ResourceGroupName
Name of the resource group to which the resource belongs.

```yaml
Type: System.String
Parameter Sets: Update, UpdateExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SpotExpirationTime
The time when the server farm expires.
Valid only if it is a spot server farm.

```yaml
Type: System.DateTime
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -SubscriptionId
Your Azure subscription ID.
This is a GUID-formatted string (e.g.
00000000-0000-0000-0000-000000000000).

```yaml
Type: System.String
Parameter Sets: Update, UpdateExpanded
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -TargetWorkerCount
Scaling worker count.

```yaml
Type: System.Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -TargetWorkerSizeId
Scaling worker size ID.

```yaml
Type: System.Int32
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: 0
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -WorkerTierName
Target worker tier assigned to the App Service plan.

```yaml
Type: System.String
Parameter Sets: UpdateExpanded, UpdateViaIdentityExpanded
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: System.Management.Automation.SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
Dynamic: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### Microsoft.Azure.PowerShell.Cmdlets.WebSite.Models.IWebSiteIdentity

### Microsoft.Azure.PowerShell.Cmdlets.WebSite.Models.Api20180201.IAppServicePlanPatchResource

## OUTPUTS

### Microsoft.Azure.PowerShell.Cmdlets.WebSite.Models.Api20180201.IAppServicePlan

## ALIASES

## NOTES

### COMPLEX PARAMETER PROPERTIES
To create the parameters described below, construct a hash table containing the appropriate properties. For information on hash tables, run Get-Help about_Hash_Tables.

#### APPSERVICEPLAN <IAppServicePlanPatchResource>: ARM resource for a app service plan.
  - `[Kind <String>]`: Kind of resource.
  - `[FreeOfferExpirationTime <DateTime?>]`: The time when the server farm free offer expires.
  - `[HostingEnvironmentProfileId <String>]`: Resource ID of the App Service Environment.
  - `[HyperV <Boolean?>]`: If Hyper-V container app service plan <code>true</code>, <code>false</code> otherwise.
  - `[IsSpot <Boolean?>]`: If <code>true</code>, this App Service Plan owns spot instances.
  - `[IsXenon <Boolean?>]`: Obsolete: If Hyper-V container app service plan <code>true</code>, <code>false</code> otherwise.
  - `[MaximumElasticWorkerCount <Int32?>]`: Maximum number of total workers allowed for this ElasticScaleEnabled App Service Plan
  - `[PerSiteScaling <Boolean?>]`: If <code>true</code>, apps assigned to this App Service plan can be scaled independently.         If <code>false</code>, apps assigned to this App Service plan will scale to all instances of the plan.
  - `[Reserved <Boolean?>]`: If Linux app service plan <code>true</code>, <code>false</code> otherwise.
  - `[SpotExpirationTime <DateTime?>]`: The time when the server farm expires. Valid only if it is a spot server farm.
  - `[TargetWorkerCount <Int32?>]`: Scaling worker count.
  - `[TargetWorkerSizeId <Int32?>]`: Scaling worker size ID.
  - `[WorkerTierName <String>]`: Target worker tier assigned to the App Service plan.

## RELATED LINKS
