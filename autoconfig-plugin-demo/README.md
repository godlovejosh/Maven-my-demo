## 
* autoconfig是处于maven生命周期的打包环节,所以我们可以install,也可以package 看下效果
* mvn clean package
* 不指定antx.properties,就不会自动生成antx.properties文件
* antx.properties用于保存配置项  antx.properties 默认在项目根目录生成
* mvn clean package -Dautoconfig.userProperties=antx.properties -DuserProp=antx.properties
* mvn clean install -Dmaven.test.skip=true -Dautoconfig.userProperties=antx.properties -DuserProp=antx.properties 
* mvn package -P dev 多环境