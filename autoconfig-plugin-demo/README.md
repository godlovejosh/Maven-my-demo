## 
* antx.properties 默认在项目根目录生成
* autoconfig是处于maven生命周期的打包环节,所以我们可以install,也可以package 看下效果
* mvn clean package -Dautoconfig.userProperties=antx.properties -DuserProp=antx.properties
* mvn package -P dev 多环境