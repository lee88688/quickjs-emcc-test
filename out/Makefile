CFLAGS_EMCC += -s EXPORTED_FUNCTIONS='["_eval"]'
CFLAGS_EMCC += -s EXTRA_EXPORTED_RUNTIME_METHODS='["ccall", "cwrap"]'

QUICKJS_CONFIG_VERSION = 1.0.0
QUICKJS_DEFINES:=-D_GNU_SOURCE -DCONFIG_VERSION=\"$(QUICKJS_CONFIG_VERSION)\"

index:
	$(CC) -o index.html ../quickjs-eval.c ../quickjs.c ../cutils.c ../libregexp.c ../libbf.c ../libunicode.c $(QUICKJS_DEFINES) $(CFLAGS_EMCC)