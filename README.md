# AspNetCache-AzureTableStorage
Use azure table storage for AspNet core 1.0 Distributed Cache.

Azure Table Storage is a very cheap, super fast key value store, and its much cheaper than the redis cluster in azure. This is not a true replacement for redis, and redis should be used if people have money, but this is designed to get people a very cheap cache in azure.


## How to use

install-package `AzureTableStorageCache`

In your startup.cs


```csharp

services.AddAzureTableStorageCache("!!!CONNECTIONSTRINGHERE!!!", "tablename", "cachedDataKey");


```