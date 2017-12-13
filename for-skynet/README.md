
makefile文件里添加
$(LUA_CLIB_PATH)/codec.so : lualib-src/lua-codec.c | $(LUA_CLIB_PATH)
	$(CC) $(CFLAGS) $(SHARED)  -lcrypto -Iskynet-src $^ -o $@	


make luaclib/codec.so  生成so文件
