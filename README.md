# Create a SQL Server 2017 Failover Cluster using Windows Server 2016 Storage Spaces Direct (S2D)
This template will create a SQL 2017 Failover Cluster using Windows Server 2016 Storage Spaces Direct (S2D) in an existing VNET and Active Directory environment.

This template creates the following resources:

+	One SQL Server 2017 failover cluster 
    +    Windows Server 2016 
    +    Storage Spaces Direct (S2D)
    +    Premium Managed Disks
+	One Availability Set for the cluster nodes
+   One internal load balancer
+   One Standard Storage Account for the Cloud Witness

[![Deploy to Azure](http://azuredeploy.net/deploybutton.png)](https://azuredeploy.net/)

To deploy via the cli:
```bash
az group deployment create --name deployfci --resource-group sqlfci01 --template-file azuredeploy.json --parameters @azuredeploy.parameters.json
```


