## maven多模块打包

如果一个project里有多个module，它们之间又互相依赖，那么打包的时候，应该使用idea先建立打包依赖

右键点要打包的模块的lifecycle的package，选择edit xxxxx（模块名称）

然后在下方的before launch中添加依赖模块，每一个Module均添加一个clean和install，添加的顺序要与依赖循序一致，先clean清除原来的打包，再install生成新的，并打包到maven的本地仓库。

确认后会有一个蓝色的m，下次打包的时候双击那个m即可。

如果还是不行，就install一下root项目。

install某个包到本地仓库时，发生错误，也是先install一下root项目就可以了。