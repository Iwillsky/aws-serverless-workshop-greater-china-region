## AWS Serverless Workshop Greater China Region

AWS Serverless Workshop for Greater China Region  
AWS 无服务器沉浸日动手实验（中国区）  

## Lambda 的注意事项

* Lambda 角色权限生效时间的问题  
Lambda运行一次后，然后在IAM中修改了Lambda的Role，再执行Lambda如果还是运行之前那个Lambda的Container的话，Lambda的权限并不会改变。只有运行新的Container才会使用新的权限。  
例如：调试Lambda时，去IAM里面修改了角色，立刻再运行Lambda会发现权限没生效。这时候要么等一段时间，等Lambda释放Container，要么随便修改一个地方重新保存Lambda，也就是强制其更新Container，再运行的时候新权限就会生效。  


## License Summary

This sample code is made available under the MIT-0 license. See the LICENSE file.
