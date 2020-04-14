# 介绍

工程为通用数据库逆向工程，自动生成数据库表对应的逻辑对象，访问接口，还有mapper.xml

# 使用步骤

1. 修改数据库连接串 generator.properties
2. 修改generatorConfig.xml里的javaModelGenerator，sqlMapGenerator，javaClientGenerator对应的targetPackage和targetProject
3. targetProject+targetPackage 指的是自动生成的文件存放的位置
4. targetPackage就是生成的java文件对应的保包名
5. 指定自动生成哪些表的代码，在generatorConfig.xml里搜索tableName，%代表生成所有表，也可以指定前缀，例如order%，就只生成前缀是order的表的代码

# 注意事项

使用的时候如果效果不理想，可以先看一下generatorConfig.xml里的注释，再稍作修改即可