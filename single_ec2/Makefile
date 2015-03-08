BUILD_DST=$(shell agc where)
BUILD_ID=$(shell agc id)

all: build after

inspect:
	agc inspect

build:
	agc build

after:
	chmod 0500 $(BUILD_DST)/*.sh